RSA - Rivest, Shamir, Adleman
Алгоритм использует [[Функция Эйлера|функцию Эйлера]]

Алгоритм использует два ключа:
- e - открытый
- d - секретный
Причём, ключи связаны сравнением: $$e \cdot d \equiv 1 \ (mod \ \varphi(m))$$
Для шифрования используется открытый ключ, а для расшифровки приватный.

Сам алгоритм:
1. Пусть p и q - простые числа, их произведение $m = p \cdot q$
2. Наше сообщение - s. $s^e \equiv c \ (mod \ m)$, где с - зашифрованное сообщение
3. Расшифровка: 
	1. $c^d \equiv (s^e)^d \ (m)$
	2. $s^{e \cdot d} \equiv s^{1 + k \cdot \varphi(m)} \ (m)$
	3. $s \cdot (s^{\varphi(m)})^k \equiv s \cdot 1^k \equiv s \ (mod \ m)$
# Чужой конспект
![[Pasted image 20240324001825.png|700]]