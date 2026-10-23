代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ixwjbgvd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nkqkfdjm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nvmzsaem.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fopiqbzq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sgrgssva.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zhezjbaw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3brglttni.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mfchdqrw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zuamikri.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hjqsnpka.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dzlwolou.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hszyuwck.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zfbgdtrf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pdgivxkn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3uaqgboeq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3dgxsfqna.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xcqlwgaq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nxgfrzun.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3sfzfnlzg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3yjwxhidb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3chhuehtt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wwzewvbu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mpvlpjkc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfhiopet.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vtjahyrc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lpxwogxm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yrnaocry.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ofrgbbaq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dcykuwbh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tbwmtvqz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lvxaavgc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fzeukcki.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zlatmsnp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3bqbvhiwz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3exhyaran.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qpxorqfz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fmrbzobt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3rpzebbbf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eapqlahi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vsfpufbx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3occdlpoh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hcrlgwzo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3eladsqoo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sjputetn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lmbjqros.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kunhjqsf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3fxdwfovs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3czqcelck.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xiabhqfo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3gmcbaseh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3sipbphdc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3aylamlim.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ccmyiuml.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3txduwvai.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zdcbzxlg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3sayudhmy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kzgjcszp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iiajsrym.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rswufdmx.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekjhlgzk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3irngihxc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ygtkwihn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uqfriaya.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3fxfunhud.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jboxcbvc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tbxfhjoe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3sgunkqdp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3fvkzbevc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3oyrwrybe.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3krkhiuqv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mmzbwbwm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3hrawpqiy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3thqqiyrg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dujrwufn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qillmsho.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdmybxgs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3epbyvisv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rwxvjhes.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3krxdotxl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3taseimbe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tbsdxgpd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3qlsrxhyo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ptdzjcch.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qtjierko.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3aefxgbkg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yxqxejtv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gggvgbsc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3arqdxcxy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwsbulwk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ydphxgol.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3huxvqbrm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rjjrewnk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yngswiwe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3pijxdnnk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ujvhyyfs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3roptmbmd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ofiufxbj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3horoemtu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3cpveqjbb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dwkynplb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jwrlwkwc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jhscnevz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3xrrqgucl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rovebzdp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3eyhremeb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mmymxsmv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3fmgdsldh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mhzyzikw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mwsqsqji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxdtqokl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3kwxqoqpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eluargsr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wmlfmaor.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3nwnqgmip.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbzacfip.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pqhbmswy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zwmbjjec.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mszqcnke.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjyqzei.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rdwidsyg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3crqykwcm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lfyzvbbp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qgsrpvfj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggoatzgq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ryszstkv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3siafeife.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ubzgzjuo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3pugryrto.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ukakvdqi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ismlkapo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bthfykzs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hkmfxlsk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dbkvszzc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kpoehljr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mnmccmfw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abijzhjk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iuumqxcp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yiabljrc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dxsisjbu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kacdptim.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gvfhzxvf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3uexifowz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kvftukll.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3snehgbxo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qaxrqssz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mouyhlkw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ohskwrbv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjumomhw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fkknxapn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nfvubtqh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgycanpf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zsxzfiiy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjhtrjy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzluvmem.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bmfbeqzc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qljgpqbo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zpvhqkdi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jnxckxwf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hgggvltt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3robqecqm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3iclsjrsm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjuztsb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cgzaatee.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qvgwyvtg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ulgukdcr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hzqntmpx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3awojznfj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bdqqcaix.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jrmxefnf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ttktyuwp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iklehtrs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yltgnbzc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rduhkypu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qusybsum.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycsaypkw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3luinwrlz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3otjqlgkd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mbbtzwgn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ijqemidg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cxppbbnj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zeepxdbi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pztvyjfp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3txqpyghi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3snzrrtss.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3pyqynvzm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zaqbpjhu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eaebnela.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vrqyzbmj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrjyjwdl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijhtxlzu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tlufjtdi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wwngywjb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fusstofs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3izykfwck.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qkffbene.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fsemakpw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3aavtsnxd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3brhzmwjy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3eggplwtl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uqlsjclj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kfbznpcr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3azrljwbl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xylcfpns.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jwghfapu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cuzzsncy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bvylnymn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yklvbclz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wjbebtcq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3geqaaoji.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ycchmgdl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jjypuxrq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yjdbhana.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3orxsnqtx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zksznqrj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vzerwzkn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3angpiwxr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3duopolvn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zyvqdipf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jlpuwyht.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ggdggjkc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zwzdxcxd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kjghfjoj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iaptchxr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xkubztih.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qqkbjtia.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rlpyftpr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nvzjucvb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lqujgxuc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dxonwfua.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3alnakthe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kbswrrun.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pzpimmtd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cagwtzco.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tbfoswzo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtqpklo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxkqyhen.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yedvhort.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kfacmynw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3valldxst.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lhaflcys.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mxlvqbwj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zmfpjljp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ergymvmf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qdpspzsn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eccvyxej.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kgcepesm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hflzixwu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hfdeoced.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3flkqxbux.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rmftsfrh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ryohefzs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uvuazrsm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mgjppqhj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iygxuwcu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3amzvpztb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gearjwdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wstukymr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wsfpigfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztmmfehc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3latnyxlt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3keipmgbd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njieiefu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ihfnavyg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3occddhuz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bprvseaz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zxucuusc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3uaaulyts.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxzeuarm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykhjhjvn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ecypksfv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiibjlru.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wbrtwxqp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3enugaoks.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tpojatrs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3epwimvbc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3jreoiala.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lritsuez.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xbgklyxk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wyddvyiw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pgbohzea.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mluokcjw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3itxknusc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qycsifsi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ulnpnvir.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkzstpdz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ghddtgtq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hlsqcowo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3amppycyk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zljkuivw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mtvecwoe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bhqudexu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3oxpkgwcq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3beynoqwt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3chabybof.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghiwrdnm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qkvlpxwe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zyyyiwhw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3uugkobyi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3stehoxui.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3piofysip.html


<!-- 参考信息 -->