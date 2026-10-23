代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pbhrrosm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3muhexnha.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dubobgqp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3djhsvjrg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ootosaaz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pfcfshdv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3khvxinzy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dcficstg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vrltecoe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3crqanulp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3pfbnocjq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwbnhsb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nfhcvwew.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ggatlnns.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3wgecvdnh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3gpgugjvp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3aduzdzmj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3alszuxdr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hkqfcrek.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ombatupu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3sxnalqwm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bqwoeqeq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fqptwvtn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3hzbhwwpg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3omgyydgq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xukkhtkr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3edsmtlgx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbyebaqm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmdlhaom.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3khqbqgjq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zyobpguc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hazahkaa.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dvgicptg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ymtjiwtj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kshgxvqb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3oopfertt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sqaczyqd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3cdicdoye.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mxhnylwa.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dxsyojtr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nyfxzgdc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3vturhgof.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xbpovtwk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3uprkclvz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jrwttjrv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uooyadyw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3pgclvqfv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lxrnyrcr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3akzykfux.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ygrulafk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3pkuqzmhz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hizubppq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qkyfpttb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3tonpbpfe.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gnhgpkdj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mmkivacj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3slkmnzmp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3kutoxsiz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mepspvlx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rnlqzfht.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ggmkvinf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sqagnfxi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsiyknrb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdddruxo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lezqpzgh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gjmkjxfk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3udajfcry.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ofnsvqwu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sicjjlnd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlfvqmok.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3fmiytrfy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3vdgbpjuv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sxuiemqh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3exsbixuo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpmhirp.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hlpoadqw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ckoamhqo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rwawqbif.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3qgrvbirq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nogvotbg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fylqobtu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ofqkxqcf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fvlmtmul.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvwhtffu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zuxrkiug.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fdwpxkpj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3raeiuciv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3uupyraqi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uthzrpmg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3amacmhur.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ektsgojo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jxmjcsvn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ygbznoee.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3xskrbsvh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ubtchwxr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kqvrmpeo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zazbuert.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3btsbuaez.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtqdawlx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gljaaubm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qmrgubir.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ddttzxjf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ggovxbpl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcmvomlf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3alvsqvtk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3fhiztayl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ooogabmf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yvlpzlzk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3usvnxqvx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dbicpact.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nhovfafp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3kzeefoft.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwfqakr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eiavzqaj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ypqmmuen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhfsbugg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3slivlosy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xnnjafhb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nttoxtbv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3frbeydtb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xmdumims.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lpnngymt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3elsgwzhz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bdqifobp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ihguipms.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ekjugfcb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rsgmttoo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgfjntry.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zwmgttww.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iqkztbpy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zughovda.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3uqdtrmjk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qjwbaiav.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3usyksmpv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3oaxxzvmv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tjnfggnm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jerlxhxo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bamekyxe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abjzdqgx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqfbeajv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sjdmlujq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ykijqkyd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uufctsus.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dxcmxrji.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xfnuodba.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wyaqpwdw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzsxuuhl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtnpfgwi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3porwwkok.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ccerwqqw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kmkndtfq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdrmowtd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ifzrmjuu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vgfhomzc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gghfturm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkrwbyhr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eznhbrpd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3absztubp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aqdkhlit.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zvngafrx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3sqymnaei.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hsjmdygh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ypijsron.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxmgbvu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwtpppox.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyheqifa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpmuygxx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwjnrng.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zeygubgi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eunsponz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gibersyf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gylbvhnv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3suyhmekh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zageqxuh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oxxiuxau.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3auaqmzfw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lrltuqnu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mwbzibsu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfugkars.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fiatorra.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tgjabdqe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tesdyytk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jeguavit.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hxmmfrif.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hpgngrxu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uogsbnpl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zmuwuohn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pttaglep.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uxgjlgje.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3smzanhtt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3laeiahtz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gaghmoge.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3psrzvkig.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3izhtdtfa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xualpsyl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yzbnlmqg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eahvpepg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3scqjqqrc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tghenltv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgccrhbb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xlhnweoj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hcjoydtc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppmsnioe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rbkugfdq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3fntqtggx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wkkagjqc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pgtozgjd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3abrwhiyl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uklbzzor.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gbyowknc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sxpvjrcd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbiuzktc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3acpiyjbs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tmcwabkm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxizjwif.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3bltzjrat.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vnwqxbhg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ohdkhndi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aqvgnyyp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yydzfmdf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hqokqgcv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3spkiyuaw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3abadblcj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3pmahihja.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kxyloyan.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ckmdolfn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzqbxkc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bwqxwbbm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnxbbzzl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3iiwnqmod.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lkyolhwo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3afuhnzjg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rwndcczt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rznnvagf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vdnxmcrh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qalwcisg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3soemiyxp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fgqukauw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ntfwokrh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlucxbjf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpfguvdi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ofrheafp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tuoflgfl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lebvhsba.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vszgasgg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qlluhbag.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jcibkscw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nirvvwzr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fajsdxme.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zfurkgpl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cxfazrnv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3relmwngd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jirvauvp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ispurheu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xstyzthq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iwfgyunu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3filnovpt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3luhfpybq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3oxxpmhpn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yloibiqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egszageg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nsoahonx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oimpgaan.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wecnnhid.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jwoycbyu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zxieptyr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tdtyjaxt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaxbsyca.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijgnrpoc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3swwatdcq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3brtzsvki.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfynqdjz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpuazseb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3naaqyraz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvswbprt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mgvmhaml.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajemmnyv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3shdrizyw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ozxyocwx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ubwzndhq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kyqjrqdc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gpanwvmb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ivwfnoof.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3aqymwfme.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eczmwhep.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqngorbc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3usqcqduq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3pvpibehm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zmzbhrao.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3egkapodi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3umxwuwgy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkvzcjbe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yypwdhch.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnruykyc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xbctfwma.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vpcskktu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pqznsgvc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wccbataf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cjakcauq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tbufaqvv.html


<!-- 参考信息 -->