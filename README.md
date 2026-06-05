--[[
 .____                  ________ ___.    _____                           __                
 |    |    __ _______   \_____  \\_ |___/ ____\_ __  ______ ____ _____ _/  |_  ___________ 
 |    |   |  |  \__  \   /   |   \| __ \   __\  |  \/  ___// ___\\__  \\   __\/  _ \_  __ \
 |    |___|  |  // __ \_/    |    \ \_\ \  | |  |  /\___ \\  \___ / __ \|  | (  <_> )  | \/
 |_______ \____/(____  /\_______  /___  /__| |____//____  >\___  >____  /__|  \____/|__|   
         \/          \/         \/    \/                \/     \/     \/                   
          \_Welcome to LuaObfuscator.com   (Alpha 0.10.9) ~  Much Love, Ferib 

]]--

local a_0 = 16164 + (((3864 + 364101) - 274396) - 67600) + (190952 - 110638); -- xrefs: 12 13
a_1 = a_0 + (113 - (26 + 67)) + (1219 - (119 + 997)); -- xrefs: 13
local b_0 = 1203456; -- xrefs: 14 17
local c_0 = 1230471; -- xrefs: 15 17 20
local d_0 = 8023481; -- xrefs: 16 20
if (c_0 > b_0) then
	print("true");
end
if ((1 + d_0) > c_0) then
	print("obfuscate the conditions!");
end
print("Clicking [Strings] will completely hide this string!");
do
	function sieve_of_eratosthenes(n_0) -- xrefs: 25 27 30 32
		local is_prime_0 = {}; -- xrefs: 26 28 31 33 37
		for i_0 = 1, n_0 do -- xrefs: 27 28 28
			is_prime_0[i_0] = 1 ~= i_0; -- xrefs:
		end
		for i_0 = 2, math.floor(math.sqrt(n_0)) do -- xrefs: 30 31 32 32 32
			if is_prime_0[i_0] then
				for j_0 = i_0 * i_0, n_0, i_0 do -- xrefs: 32 33
					is_prime_0[j_0] = false; -- xrefs:
				end
			end
		end
		return is_prime_0;
	end
	local primes_0 = sieve_of_eratosthenes(420); -- xrefs: 39 40
	for key_0, value_0 in pairs(primes_0) do -- xrefs: 40 42 -- xrefs: 40 41
		if value_0 then
			print("Prime found: " .. key_0);
		end
	end
end
print("How to obfuscate best?");
