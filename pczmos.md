代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2acmpehkv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zxfqvdel.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hdjbhosu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ksjgomxi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2wxeznrue.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qqeqflqq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lqcfpwdu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dzahxvcb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qnmitcyq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2sggpvtzy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2skdmbzfd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2otwcppop.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wkadaeqs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hihvaqfl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wabkgmfb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dbpbjibr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2robjdolf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pxhoolcr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jbxeompt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2evdwhvbv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mkjctgpr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2bhytvjpq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rqzhsgfy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pwqpmefv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dmdpqrsp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2urwjwkhh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zscrkfhh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ltqugpcb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xbkdvjbs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qpexwmgn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zdgyufbp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dopmpugq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vqzwssxq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nvfccnwu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2rdyfthoe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ytkdsorq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zecpprhw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2advrkjye.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2mdiqtjgq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fxxdipsv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mhrhwavj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2abwekxme.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvzgqori.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2momvfhii.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hauqghiq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hoqhvahu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wvlusyuo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qwkgrybk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsdpyydg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lglfmnne.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zivypcip.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lqfbsffs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xfuzkbwp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vhqybzcb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjgqppbf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jvrkzfkw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fokdzkny.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zwgjdwxv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2onpfywog.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nxyranjg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wqvgtmfr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zfdwplqz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xnlkjkuo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2pnsfmtko.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tpgtqfea.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2inzxndzt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xbfgtuam.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zomjsgzd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2umdtoxhd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vrktkbng.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2acvzjqya.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gerbwugq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kgktffnw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ormfsnvc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vaqqhjft.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ofestxne.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2dlovoncl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2fwptvfvz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2eqobrbpc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ocqftzny.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2iqzbactr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rzucpxtl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mjzydqvr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2kzysmfik.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2xsvojgxq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tzrqtnxt.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wodeqogc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdoetfun.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fwqznegh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2phwgifye.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ehvmdxsf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2rinkytfu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2asjmppgq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2unnbnqiv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2scidyazc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bpuymbud.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sioaplyj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uzdotjfx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aomccvoq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wbjrvckt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2cxtfvkap.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qbrjgykj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2twymolpo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2lkgysimg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ohnlbcnu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2edcxyegs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fbwvdzcy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abdvmicg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zxazvnmr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xeohkbns.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dkgyzjnl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2prwevqlf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2optnnkma.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mgxfimlg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gddtjjol.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mqgktfqh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ruyslezh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2cithwlup.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jrdhajxm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qygydazc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pmpsgcab.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kpkbakkv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcarkkiv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ginjztjf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjrtcbnh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwpkrerp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ntqkzvrt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vreydddq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jcozrlia.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2dqmvszlu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ulatgnpz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ckndczsb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2daikxxrz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zojekpdf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2trfxcdsf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ipbeybgz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mtwuxcik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqfegxrh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2klqlrwry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayfhyyfs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tuetvdws.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2espexdky.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yuytjnxj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ucpmfndy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gpnehqlg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bcxzxgqf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wbmzxcsx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bteehpxz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2utggdyty.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vkaceyhq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2vblkvejy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wqwkaggf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ooadvcxg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2npcsohkb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uvyqlbvb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2umrtopkc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rddqoeav.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2othknxlu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ajrpofdg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ameynizw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxitzijq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciygdytm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbogntxd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vnqeirze.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqmfvkr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kjpinzdo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gkcirfvy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lucgymce.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jpnbhlxd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycafdgrv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwzgidab.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ivfeqmdf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qemoivxf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2izvtsnpm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qzribguo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wmwqgghq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bagdwvhq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gicljiuw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpavvtc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fzvynflw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2agdovqjk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdxsilrb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ikmonmqd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pjnkecna.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2avmkaezi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jpkuqoct.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xijuxady.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ipjikmwn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xpbyrrvu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vskghtbi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohvdizrg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2edjdzqeb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2oxvpyiks.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttalicsh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ehkzkxgg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzjkzofw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2slvubiyi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cvwedlip.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vtpojlgb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2blhuxyup.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zjjdsrvp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2htfoxucb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wnutedjs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cknrtjee.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zciffkod.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dfwojbbw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zqzabjam.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qagybkps.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aonoqrjp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vnrskica.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zowbkwrw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rzlvwrki.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qlkdivwd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywlvcsvz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2avjipoax.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dhusbuzu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zerpomds.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kaasggym.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ogexsjuo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pzqurzqe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rutcxgjz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2prlaxdjq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kmjqgfou.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjxeloo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uqlyietx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mrmncexe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpcjhtmt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ngcmovqt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tlerpman.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pldiczzl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zykghvit.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kwnitmwg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nnorhxxj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2glyfkbzp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zrvszhlc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2bsdlcolb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2htssdpzu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nswzbgou.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wnxsocdt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pcvrbxpq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tbhzbdos.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ummpldel.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eowxilaw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hvwwrdth.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hkkzudzz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbxdygii.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ilpxhmlj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ugewxdly.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2piqqahjy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nvjfkcxf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pfqfkpps.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eqxvcjgt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrkdjyu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ltshyfao.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hsssbwqh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zllndtzd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ejonlzwa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zrdjwabg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jdoaqstj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2shoxxxfd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lnproplk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ufnfvmvb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uumkddpp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mtynawzm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2srrxknad.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2micilzir.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xfaludft.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2udsqtckc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2unjkhilk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bqteqkjs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gaqtlrln.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2haeldudp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kkkbhhzi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lplvdhiy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fnuivrbk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wvhimjuo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2iecfqgat.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mnwbzfyq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yrhwrwri.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kwjlsbvq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cymtnzzj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xnsmobuh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2oxrpmuak.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2crkpnctm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnnqsegc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iqznycid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zeqhnhiz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ugyjzprp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vibtutvt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2addlyoig.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kewmjkby.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnmuornf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2noqzuvwg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dboygzfo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ziddxiuw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2buujkinj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hryprges.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wcfzowoe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaizolly.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fwczybit.html


<!-- 参考信息 -->