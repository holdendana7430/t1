代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nrwubxaw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2trnwfdln.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gwykjpej.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xavksatq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2idgsnahs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xlawcofr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jiflykyi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2zairfzho.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aamryszt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2yfwfdndo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2knjvthep.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ftzglurh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zikxgtqt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tfmnieia.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2dajutgxo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecfpwrqq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ycvwfdwq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tbsnpqqj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hailxrgb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wfotblaw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2rfawgmxb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2avzqtrza.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2itugdskq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkscjevc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xiavkrzq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vuwawryb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rmhybqgq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yzqtmelz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lxqoubba.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxicjhqw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vazfqtiy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dztsnnzt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2czxohywp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aacridum.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tydfbrup.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dhdnkgzi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2akkpdtrp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eszceuvj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lfzlgpfe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hscqtcfn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ltktlkvq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2njsaylnq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ankdvjyt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qxmtztfj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zgnbgukz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2tqgfasia.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wzoxjffg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2hgnmzmbj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uvwxcvsh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2novhnngc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hsxdptcf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kafbsnxk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ihmstovb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ngramtst.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qkymmlfp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gzkqguqp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ujktjiwt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uothowqx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jkrgjzbn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2kgofauhn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xgccqfjj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zkxvlumm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zngkknub.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2blxftlmi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fneeplgo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yezcwcnj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ugjbwhdy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pwtzznpk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ernaejbx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kpvaaram.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mdukzlbf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2fvviljio.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2muaptvwq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klnqmjid.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2sehxudmc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2loryzscz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xcozfyym.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lqviptzr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hlokmyin.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2xdzpseam.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2npgdzxuo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gfgtwcxy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xvalykyf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wtcekwxn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ndoxurwv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kzlwbfei.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2htmtfvzp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjbulpv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mwmqldce.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xrzpenxh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2dpziqiwi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nzuuebiq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjdaxpum.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ggsgxqvc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ifkgtbbh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2uqbrlfum.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jvsoejxz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hysxaefw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2eavpfnxf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nufjtsub.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hqeimvfm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbnyjbzp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2smngmxjs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sejjsxuf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqvdhqq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjrvwzm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jkwyapib.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kngecvze.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2akuhvqid.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cikfdwjk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2rkixuoka.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ggmjdxis.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gzcxbcmf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ltaknluf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jzmudbfb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2blcozsoc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dwvhduvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upautclz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xignejgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzkgriwh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2cmjsmmpm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kehsiwfg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hxuabngo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bhzldwlq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hmvxthnc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nsopdkhs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2nfbnhmaf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uzaohkmq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zphchxwl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ighsiqzo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oipfidyi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jofwqrjt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mubhwzep.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2udkxkcec.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rnoplsdz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jerrumgq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2zbwekavi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2onkxbjpv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2seubhdoj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2beddeppi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmilapv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ydsxmufk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sshhxcpg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xudscery.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ufnnoknd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sgjnrvsi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jqnojeim.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdxwzvou.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zoqyozmj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2iopuydym.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2znhtrvyu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oricodaf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jijpprxd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2eprhnoev.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2twhwaeeg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuewtbpf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2crxbeeyt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ymlqyycn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dwgxuarb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2knezxhzi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cjbrhkjx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxypujpw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zvbvtkwl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jbksebtu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfedjjud.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xpxtrsht.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qumwdyib.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xxsteloy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bygcdper.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2egrvahbo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxjsvoiy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uaybgefe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wviyycko.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vmlhsydu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2kmibubxf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2njlpojsf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lavamugu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uvyrfiqe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tplbirdd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2klkdezsu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fhaxrmlb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nyygjycx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2scslhvuv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zgorisbc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2crfppbia.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2srogejdz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2whuemfbj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kqijsbhb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tjxqofdk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sypcsbfv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2oonrrozy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nigbgcvc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zrognphq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zxyrvjrd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wsqqfkwc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qcabyggl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ymntrgat.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uixaadxs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zfklvxip.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xdljpwdu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdjfepw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cgsfoytv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hsibsgmt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jwihwqbk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vvomocmh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2aojcidjn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktrledbe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pwkmilut.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wyiwxgpd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzlguula.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2guadlalf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2efsraoew.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ffzcnwjp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mpmarclt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2citgwoit.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2baubgiec.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2veqzmump.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2excykhbt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2axdmkwco.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2kxkrqvjx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ndxzgacc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2enpyphzd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mbjvdkls.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zmglsawp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2trmswovi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2llejhljc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cfaymazc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fzipkdjp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rhdqwprz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rwbpukax.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnulyuvj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lwdmybwp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vddydvfj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cauhdqcq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vszuljpj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbgkhud.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vyzkisww.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dgxmokxc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dsmjltnp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gojephwc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2neulinbx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2icqebidf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nyaorvbj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2baqvhiod.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aleysntv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjehmaxl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2svqocwnw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xztntano.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rkjozufu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kjdcoggf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jwvotprp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ivqcelfm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yqgzybiv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dsfkwevc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jmeljzug.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2awnvdgna.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mpmlkdcg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2uqeobxuw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ghmxyalq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hjvknuxj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hmxvfhvh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kasiecsl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wobjdqis.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jdqqkayl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnfurkfu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mzyegnxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bypjokfr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbnxdcvb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2demnzhdh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pgzxhfvy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2otaqmyng.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiehsiot.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssfeawqx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mrxdamts.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fzygzvun.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zpyiiaih.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vkddepyk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2njosoppd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztliwmkv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2poszmytz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oqvellzz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hbapswri.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qmbpiywb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ksttjgnf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dlwtmejx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bfepsxiz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2brnohlex.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wglprpmz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2utoxhwre.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rwuziikb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kstpxzkq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rngboztw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wynsiftl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pawpkzgs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hyhoftrb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2veamyogg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ijgjxnlh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nsvftpfy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qwbssync.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mpgebzjr.html


<!-- 参考信息 -->