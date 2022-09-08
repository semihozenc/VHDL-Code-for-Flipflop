library ieee;
use ieee.std_logic_1164.all;
entity jkflipflop is
PORT(J,K,clk: in std_logic;
		Q,Qd: out std_logic);
end jkflipflop;
architecture behavioral of jkflipflop is 
begin
process(clk)
variable temp: std_logic;
begin
	if rising_edge(clk) then
		if(j='0' and k='0') then
			temp := temp; 
		end if;
		if(j='0' and k='1') then
			temp := '0'; 
		end if;
		if(j='1' and k='0') then
			temp := '1'; 
		end if;
		if(j='1' and k='1') then
			temp := not temp; 
		end if;
	Q <= temp;
	Qd <= not temp;
	end if;
end process;
end behavioral;