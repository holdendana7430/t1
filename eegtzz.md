代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lawkogsd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vjpkcoij.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3durqnyut.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wkfpqdoo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kvbztdob.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3reyuzjgu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ayknqawo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ypnbdqqs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iewoefaa.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pimnemqn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kcsmodty.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ldgkjaoy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3aekshylr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3hsrlljdr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ulzbbndw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3pmszqqhq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3kekprfxp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pqhpfruy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfhuinio.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ufqkqthj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yyhuoidx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3igqyvawo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zxpwllzs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uyvowybu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjfaajpa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tupzzrfq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bbcqivkx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yabrgqhc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gaetdjyh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dmlgkekf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nzaspukv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgccjas.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zfcfodwp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3aldgugeq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3scozjoun.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jvmmpvit.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qsdqsjav.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tnbjyekd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qthsdplo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3yogthbel.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bkncfobu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yipigrmr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3juprohqe.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hhrwnkns.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nqbzbpmp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3thvhcjww.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3uldbhaqf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3gznuteqj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wajqrfrq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mfupbknt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ccfkhyaa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3dhqirbth.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vyvigimv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3iowtokuc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3qajxrksg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cstgkulp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3clzdzcip.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3atdmpwjn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tiplqlig.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3icrxsaft.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zgurdsxi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sevflwdg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvmrruu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3quhfbgza.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jpdgpfhj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkrgcrli.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3bwfakpci.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3uiiuberc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3azjwnmfz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vdcenylz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urjzsyam.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3bznkizyo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3syryntnm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3edqiwqjc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3agqgcjzx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3shnytzcp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aqnqjekc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rhwkhvxa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wqikjjco.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ozdwpzwi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nzoalclu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cjferbrc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yfiekdoa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fgbqhoae.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3patfsecp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lyrtplvz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uwfzzxos.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3hxumqjac.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vblmfxgb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xumcxluq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sbxzsvui.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3axhkawuc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rnnsiiub.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zeootkpf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wumdhamd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fgixyhjk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3omgqepyo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xkvesays.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3pinbmemg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nzyhgyor.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ffojqyqp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3digazdzp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3utnwaasx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3zpbdrdrj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ftqacwqu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3smelrfpv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jhneuioy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ntsovyqt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hlzynovv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czkznpoo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kxptlwto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkejpfnu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jwfnfgux.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rywnfmoo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3apvhqlwn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qpsougqv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nahtfcxp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ouuqhmrt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ygocmody.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dyaedwmm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tzjetnyj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pavvrvgk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ibagbzve.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3olzpzvmu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lzrmpklh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3curqruyc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aaiyimjx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3uvrjphku.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xsvtqnvz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3emkdviui.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xnysbfsb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rowoglof.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hyhiukog.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xjaogxgy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ubmzcijg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3naqlmxuv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zzgzasus.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3smqpthvd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fmbwnjpl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ltwjbxac.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wwasdkot.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nzjipyeg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mowzinmz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohqgchnc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyifekqx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bsnzclzw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jfacband.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwygjxkb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vqdhqdgb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxdnqct.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ittdmbeb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mujvoeoq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3newzsnll.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cgyxqpmh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tqcjrdmf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3syfdhyjy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gquzepaj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ahgabedq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kgkrcgoe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nbcmmbdb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngfyblmd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vonnokmw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbjcozfj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kkrcnaun.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fnswgqpl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3whdbhztl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wnaqziqs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tciwtqku.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3woxejomf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpumeyam.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uticvoit.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fgrnpsqe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nlkoacnq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ejltsdce.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnsxhxnu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hnnoropx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3glnsvzxq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3meuimmyg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fhespuov.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wvigrmic.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gheopmao.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ucviadoh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dkxpwcgr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3retupaeq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ltxemvzt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ckmhjtpl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tqiiwqae.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3riuivljj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzivodyv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3domatdqp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cjzstemv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xnozhfdf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ntmlkkyn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iegpbeck.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ksmntsev.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qcsolhwv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qhpiarqc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ffyecywd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3drqtpzys.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zarszhce.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rfqbgpzp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aglhqjqq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wbjrrcrs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3szpcgvud.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3esxjhmot.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kzzspfmx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vthzpyec.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mjimhuyn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ofsihxpp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dfkamsgg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ltmnrqat.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fsjwevie.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3towzeaqq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ulzpmmli.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jvqyumnw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfkrtdec.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvuaaaxi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmgfirvl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fgrfvsmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bfkinrdr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3udaidrmf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3betkvkdd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dopzsyts.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tgfhuthl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kjftwbgm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wlrdskyu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zsrbzvod.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uwbjrtks.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3smdqhkgh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jsvqzbcc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3knxmrwzj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fbjrpicb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bduldqpw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwznzbln.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlctohjs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3khyhewfj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xnwqaoot.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wgztnvfj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lzvfitix.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ewgfhrgm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lsfmnpyy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nvpwyims.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gzmhhgps.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cpvmoxgx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iklwwhhh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vagjakmf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vlyxijvd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jgdfodnh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yvbtiqqo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zbxjhxad.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bqlxjxuo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zrylblce.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3loyqdaza.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jqbegjes.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3czcqimod.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3augsbhpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3riiuusya.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cfcgqisp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnpsrxoo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uthlrleo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3phvmiftc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwrjcsdz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3idqdnihh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mktkorvk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sbhoxtpx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lmszgwvi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3bdzttzml.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnpwnqes.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yomzpwnf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kxmwylgc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ugafwqfp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lrztplhp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szqbgjtu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ipqmmlnj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fetzbijt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fajtqtqw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zpxivjxp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kchglngn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3oipjffcl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wzfjahjw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3evwpdskd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jewrreru.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkuzwgel.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vgowmwnu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwgshdrj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3eqtaqkvs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bnoxuimp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jczryffi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vejqbaru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szapckhm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ytkaeigw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uenszamx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3auhffojd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhlbdis.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zkwcthso.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gxwvgiin.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3klaaufqx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xdxjoqno.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wpddaatu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3itesaeko.html


<!-- 参考信息 -->