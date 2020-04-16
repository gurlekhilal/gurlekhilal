--# gurlekhilal
--Sayısal Tasarım Lab. 8-3encoder
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

entity Encoder_83 is
  Port(datain: in std_logic_vector(7 downto 0);
       dataout: out std_logic_vector(2 downto 0));
     end Encoder_83;
     
     Architecture behv of Encoder_83 is
       begin
         process(datain)
           begin
             if(datain(7)='1') then
               dataout<="111";
               elsif(datain(6)='1') then
               dataout<="110";
               elsif(datain(5)='1') then
               dataout<="101";
               elsif(datain(4)='1') then
               dataout<="100";
               elsif(datain(3)='1') then
               dataout<="011";
               elsif(datain(2)='1') then
               dataout<="010";
               elsif(datain(1)='1') then
               dataout<="001";
               elsif(datain(0)='1') then
               dataout<="000;
               end if;
           end process;
         end behv;


