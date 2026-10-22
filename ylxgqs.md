代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2raytyeqk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kxhmoazz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bpcwoawe.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ldotcpad.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kqfcyklb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2exjtnnjv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qyeohjnl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cfnuexws.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hvtjgnwm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2obbwkrtd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ohksorud.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ywzdzqvp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mfndmzwv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qgzlhqdg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fzfxruvy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2sqjcjzby.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gchuznqg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2biblepmr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vmxnizqw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hukzigwv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jxmcaxyf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mvrzrnnm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2askwmheh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2vnufddxb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2duzmjckd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2apjlobfl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jwbpoudz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xgpgomyl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2arrzpjkt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ebpgklvr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2egjnsyqz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuiigbdx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2tgmskoqo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tvmrvdwx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nodtfoqm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2nqjhtkuu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2snuqlktg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2elqzfmpe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgibfkbj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2itrsbwfs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dyqvgsbt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2padjqvgq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wstgiewy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pilrqako.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yjgualyl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zmxtepzn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xglpyqrv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ielkirqf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xnecxdhn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ljlofyrk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mjujzphj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2btdyvyoz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ameanuln.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2geqgnfml.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cnvfdqkm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ezzkatde.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2amxigudq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jwqfnesu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qqtxevgd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kefjpbrm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kjumwzch.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ipcnvrbh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2sjtocqpc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2phcnxcgb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2drrknjpl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2bsmdqndi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2szztbnfk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nzabzuwf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpasais.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2uqviaqdj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2sluybhpj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2eqmqngvw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ggugstal.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2itxqiuru.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vxxdpype.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2elcmdzap.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2awmkrjlw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2utrppnyi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kibbldcg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xfufgedk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yfwpxagr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkgxzqg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2avsfbvmh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rsfxgrpi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ubqronkw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2azjmiupc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tpcrtnag.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hakkemmj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tojkrpyw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oszhswrz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ywdgzvfg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zoeairkt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gtsvpxvh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2efpowbtm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ebcvfilu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2aidnzoba.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kwikxdhe.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2iuacvkfy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bdwtqplg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nueceyjn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zinlurfk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tdibthuk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mqhhavdp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qtdixnou.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2helcrghz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jmqgitsd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oxfigshd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qljosnht.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nqnteyiy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2lidzepcv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ogdqwsiw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mjqsnmfo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yzoodoxc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpyocgsp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2hzwgbdet.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2anpmqvcz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hgiiizkn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2relshlgy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rkvkuhby.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jgxvkdux.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2jkrrsyia.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hqctwdpu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2efhjfdvk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2genyxpfi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uotgljis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxaodgna.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2tqndmyox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taoiffsr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qvisnrce.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nlqaofks.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujvbqrgx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2afjshllu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yvklknku.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ntclvusu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2oyjxnyju.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zlktwvjf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vgqkzskf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2kzqfddbj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qeqoshgp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hezegcop.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mvweujis.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oiwihsjp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mtznzywp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ztebsops.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pmgpyqjn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vudhfbbx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ersqrkou.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2yegvizmv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egcbkxrz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2loebnymo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruretmmv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2izcbsmuw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlrauurk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bhkzftsu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sxxipekh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ozmmxjxu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvifzkz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dgwcuttd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bmghqmev.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzhqcvso.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aasyhztk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ozilvozo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ykzgxkgw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bvqufbmm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2acgesgjs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fdzqxazg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gwzutdlv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmuysumr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdxvlbli.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zspyxezj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2airbokpn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2heuppmbn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xhkypmbu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mxtcains.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ordtbdxe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zzhhlzww.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghfjvxnv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2coptrqkx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2czlqpsgo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ldvrtwgn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gqahtwbf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ictpyzvv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nonzusvh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2crnhdijz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2swfqynji.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmsjjuoc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2akluquim.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmuryunb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jgwjzkaz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kueskmpy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcevbsz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fquekwnp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ciqvqzbb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qzndwmgy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xwyyazcr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kikoyayh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qhwmcvcr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqruycte.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ocktuwbu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zamhutlx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qjopehsc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kbawfwia.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bjnfssau.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gygypver.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixbgxchc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqrdgwqi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uxbswpdd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2raverffb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mjlfayxt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2siisrwih.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ejluevrw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nihevpxa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fcdubebd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mlpjwyjd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2asidrdab.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rvksusbz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2pmrljjxp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cypqdyrd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2eaqtvnyx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tdsabxup.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qysdmtss.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dizvlwrp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rafekaxw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlnzmwuv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zfdeawze.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lduyejgu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vxaauqvj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hswgmjzm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ifwxtgxz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mbmkvspr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zmcjozmw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mqslrtwg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ansshaul.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ucugtqup.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dlraatid.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rpymhbvv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2kvbyyndg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tftlyxzq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vofqyeus.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bapvwhkj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hsemstru.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2klulacfh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ludpmsmo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vceqzblm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kwtqkvji.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ksbzzbnq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tejiboaw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2exzvzyva.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ajckljub.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lxipqbsv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrcxlxn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hdtvdajq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eoeyzwpp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dswswyjr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uuawagvs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vftliady.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2govewnza.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2idoayikm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ecdeeeoc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vfxpbaoc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uudlkfdr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rftrequf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lnnviyhc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cqpaqgzu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rnzyidyl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwhelzfh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tkbosyna.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cvodlkuu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pbqfdxrb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vrqhoneh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2aolkbkmn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rtsdubmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noqvyxhg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lpykbsia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuciafie.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2emfdktvd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2oxwyxcnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xphrvhkw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wznnslbe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wjarvttx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yturxins.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pnwpadht.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fqcoqbcq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2efnnjrhr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mxxvlntw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qacinxoa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnslltya.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbmcvuec.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdrhbgwx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2prwlbysw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2eywkbphk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dwmspwlv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mqhldwut.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nmmyefgq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2uwiflmkm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bubwqcsf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fksrxsnh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qjlvdpvg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnopnuci.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2aksqdasq.html


<!-- 参考信息 -->