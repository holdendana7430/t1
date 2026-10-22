代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fyszjuey.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ggytjcoy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sehbfdwu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmjbbzyp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2cwakmvln.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tjsuphkz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xfwxgoac.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mtaraxwd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwgspdkj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gestbqmt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fxycfusm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xzfhoukd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ivwhzgge.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2svczumbv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqhvfdzc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oxoujykn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vekwhqbm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kxawnhez.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2akyawewa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tniohcoo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xcdttaka.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2wzilxdqn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ysyxezur.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ghfvtnnu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2irearaam.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2txukhpdz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ijqbemat.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wchnuyof.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2twwbbkbx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tremecjl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dxyzwrwv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2urteddql.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qdrjzygj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2tejfunlp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2twwbwsqj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2hyjiodhx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xgnpbuyq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2etukozbd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wihywvls.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ssvrhbiu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2piaxuqnu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vtjlxqch.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jlhzunlb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jerwezkq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2thngecfj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qytkmrdp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fkqdnwew.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jawvmuyt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fjcsxnad.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qadtjrdp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mznfqckr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ywcjdihu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qeyglrct.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gmdyyabl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pawnzeke.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vrvwumth.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ahijycio.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mfcjsoqd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxbrmrd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qmzecsvo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dmgrxqxe.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vkbuwbfv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cxndaqfy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkasqxsx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hgdxxyjx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fmublrst.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dwxxbtsj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpssxsyp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xbyzbnlz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lvlgoefw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2dchisdsp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bxshurvo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2eehekrpv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tdjycbjk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2waxprcoc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cefdpvex.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2vwuxojkh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ifxzvgqv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2csnigbni.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lklvmfxm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pirontaj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouksgfmn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrphoqyw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kofvtcly.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofluwwqq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2obyhzgmu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ehhgeyvk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2beyxnhfo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fpndbsdd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rgfshnzd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjhnajf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2iqosmbwe.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yvktugqe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bkvmmsrc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2derijdvy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xbwglexq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jqwlnilq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqgxkkde.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fxbkhhms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsbpopqk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ziprvzri.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xpyqpjnl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djghwdlu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jnkzmktk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cgitvssb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nffzovbx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qlbchzoy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vktsqmvo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jpmrvqhe.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ztavcaqw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2aeyrmhqr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cvknduhb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iakhjcng.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aluwakdv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2buzrgoef.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2cnflifub.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lxionklw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2axbyxttj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2cmgyajlb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hzmfzlgy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgjjuisf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prvrbouv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2usaquikq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2frxwzfnq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iiytgdlv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2saooawim.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2geuylfkf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vabjaihl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hppezqrh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2reqtyoqf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jkedwqjo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aezgxsro.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hsrviqrq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ywkqoonw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zxhvmxuq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xdeadyqr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ecxzjpbp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwsruyi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ihhhgqny.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lpzmwfmg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipffownb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fhylkwiv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2sefgqsmh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hugrvfff.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yvcgobgw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2omgaerhd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2toizycwf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2piuguxpl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lyuewkvy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfxmeff.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2levtcylq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jsljmwjv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vvckkmlf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sfdtvpjd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2oudrzvfk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxdqkajl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2unwilezf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wyeplhjs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssoexbgz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vofjgkra.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jxxeivtn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2sqihxfdb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xjvolaqf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dsijdlsg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lkklthdp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bjcflhic.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gzjyrmzw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tppneods.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nkxibsiu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lpkrcpxl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mvcqhkwl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kkfnwlsu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hmzkepyw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2thvcyerv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuftvbwa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mlnmlwzq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvmyrgxr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gixnqzak.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2chjrstql.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xiypahbm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dkfthknl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rcvfvaky.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2txfwhzrv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyulpmht.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nrqgsjhv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2felukyuk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xscxjday.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xasnwpjx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gvsezhaj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2jsmndovl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2gmjsnjlf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dolxbyqx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2eoughyhb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vuuarmyw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2srbyepwf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ewsfciyg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jfpfmcim.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xysxxcsp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bkuvbkpx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2itflksxg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uhgwhgof.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nmhwvgvg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xfkedjdv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxxazas.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xgshqave.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxqhoioi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gnkklebo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ndvhhufp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2typdxnlt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sgqaslhy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rnhpkkcn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xkmazhfx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cskghtlt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tdbnhgwz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nuevamji.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bgrhujru.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2czgpddyg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2psgxrpps.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ufwqqdvb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lwnhfyqv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ihoqasfe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkfkjljb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cjdtdfoo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2eyushhwq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2amvumefm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mrhmqjes.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vumdyzmf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2udddqaid.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2unzwlgbr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xbfmnafz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2thzrlzrx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2idzpzrcs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pmduwdeh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uzsgdcve.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nsnekaiq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2eqsoyesn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jtmbwidq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2kwcszksl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rsvpeyfy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yaquuaty.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iqqtuqow.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2emjbqnni.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2clfvixok.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ozpeycaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvnquebd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cnqiehbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qijzfowa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxkvodrj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lzlvsfxc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugkqemkw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xtqobmhe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmgncxam.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zzovdqsa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2avzljhnn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gcvxpjuq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zrdxmqha.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tticpmtt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2erexantf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2prwkuojg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiktqwjb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2womalnib.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2krtamptx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxuoegcj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2eyhpvydu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rlbocwjv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehtexycw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dhaqoubb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2slulhepj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2eudifooq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yxmobaki.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2chwspijn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pjrtvmpv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uvdiykiz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2uqoscihu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ttuicybh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jriatgef.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qginbifa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oktfumsk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jurorrgu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ahtxrlvh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cprhuqlv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yozzrdss.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2axsyfgus.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zsqdvcjk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ehbabfbh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kiunhlha.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gbrokxth.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2chvdypsk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yihdslkk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mksacxpo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rocxzjry.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bcauhcjh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fksctsju.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pyefjqcf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vjnbofbo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tnxqrcir.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2paovjshy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wpvivgln.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2alwsxcge.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2osuqlrtk.html


<!-- 参考信息 -->