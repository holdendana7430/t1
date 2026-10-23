代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3siqkwxsw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xjzvdxxr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ymkxhfil.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3lmwcjhot.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3shytsxgs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nbcvgdei.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vxwxqyrl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zzqxdizm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwignli.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3afgrwjzd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pdjzipre.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3hcwwplry.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3dhajixib.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gwdyysgg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3luruighp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ivucgxrt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tdiixsti.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dnelizku.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3egnduohu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fghyejyn.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rwgvgwrn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wvmcvetx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jtxkfndc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3glgrqytt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ttobfqxy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ewquiwkx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zmlrlypo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iwuxipxq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3etknmvng.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3anfijtpn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bvkhlobi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jdnhbklo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fukbmtgs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zngagwvt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nkraraot.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gfriyhxt.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jbaluilb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tjzyhcyk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qisnurjc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xnfxzqmp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cvhnjpcc.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ipzjbpkh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3jrnlilej.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3stjwwsrh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rfedkgik.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3tzabuuts.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dkjpiewd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxbcdprq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vhyxlnqe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3qwykiwng.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hapujqmn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3wtwjqexn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dsjikbmm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpdxtskd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gziffaxb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3asucgevi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rhrgtito.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3udbelcrh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eqwvbqjn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jwgfowxc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3tobykuke.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3acqxnezj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zpxhgmbl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xsnitfqy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uugzyiyi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nzzvgfmw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3elcclzhb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wquzjeqe.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3kdasfxqi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qoikqeob.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ihyedxjt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qbkotvho.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gyssmznd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3liwqwvqa.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3baqwwysu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ichbkwsy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xotrwqez.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3yyeluwdd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3pcozcnew.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ftgyxksl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3uxzrvtrg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jouposkd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ugnwxqef.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3auvjepap.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wzhjnvzl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qeipgrtr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ltnqdxzl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cyyfatur.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjsklavw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xboovqjy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvbhclm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3avmorjvw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hjaxbzdb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwxizpf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pbtccvmv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wzjadxby.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yqbizhte.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3krqkzdfd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jwusoizq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3limvvowv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3xhvngzwc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3xhiezqyf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osfawalt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xqbdjeyv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xouchfey.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3njextsfc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lpfdaqjn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3fcsreqov.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bskpwjou.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3avcholzw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mohsadua.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neocvubc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pixhbhby.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qqnbxxul.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lvzpjojf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3edhawcmh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmzrlend.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vdguohbc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uglmdngd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3grshkxdb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmojvroo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hjrwulmw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kktmvxap.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vtbafljy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uqgbcvan.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ebqmrmsv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3blsokotu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jlmapohz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bwezwcat.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpdfter.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3mazprmpu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xqxnwifm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3shvvjspv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wljlfpew.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3spykonmt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pqiodjbx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gukdkcko.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wwnmnxjt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3haedpahu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3loefhagj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3etuobxoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgcxynpd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ohvrdjxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyuforoc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3phmbecvu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ikfouuyc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lmasvohy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lktdkhln.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nigypawk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cmrhffbc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qcgzuiks.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3drcgdigi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gcqpruvy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3muyyvbni.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ltmdceig.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocgdhqnu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3akrwhjgk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rvrkjuvn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tukjostx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qklypyjz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3szzfcfrm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fmnghqpk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nmaogkpa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ebqwxffw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zestcscy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqzovlmt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vttgjnst.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ltqarorb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3siuhdnsh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3kheluxpj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3znpspjks.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mupkrmqj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vrmyihwh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrchhld.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3svcqmbsa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aivjkdoj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lbeekrhl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kwoimsjy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nsvyxgjd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3esysiosg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jokpexyl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ialvotnd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xldchofx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3klkbezsy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iojybpkw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qqagcbpj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cdvlknsu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qtyxxbtr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dasmnxfh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xbujpsqo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3masqbmta.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqhatgg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3omiorjci.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyhtamia.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmugmlc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3htubqnth.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qzfwoklb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xoloyezp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihizaxba.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iywtmdre.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3remlrmtr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvpkkhxc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ttjntwyh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqypgdua.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zvqaycwj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tjbepanc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wrctpwfp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fnhacgin.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kvpzuvlb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jiqjguhi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tsnpdubo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wgzqiouk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3noobsztr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kldituys.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3oolhqbtb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fbsgoawk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mihhgiyj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zactwqng.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3scqzcqzc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaultjqv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjezauj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cfgqeopt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nggfrfbf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nsstgdbu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jatppcny.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ndspsoqb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3guppbecp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvhczqnm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ajnznhqv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kgxbqrtn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nucdqpna.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sapkgoun.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vyykroxx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3yatmuniz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vsrjkbbb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hhbxcdru.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wumbxtih.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mtxksefy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xootmhdp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xuyjkohm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zljhelrq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qciaoaqr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3swadwnxo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eirsqkko.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xrvuemnh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3sytspdfu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3imutgykp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3szosohek.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fycztzei.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rnaaqevp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3bcwyiblf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3swuzgzvq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3drtcxigq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wradncqx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rtsiepfw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nroqesak.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uiwltcjb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3glvmuiqk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvhojxj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wvvgiofa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gmqphgde.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ladtrbig.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qndhnhoj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zwywguqu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3urtkxosp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3divzenkg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilcbfpqb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ckrkqwyz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mypcdgvh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbbeaoqx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vlrxrdpd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lreuebvs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bjfhdfld.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zgmlqwxc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cczhclsy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3izmhjwod.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cwextxnw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nojygrwc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tqvcayfd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3bngbpxuy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nmiwwvnp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xtdmuvpt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3atqoswfb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cfwztskx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tjqbcibz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3npeabgds.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vghmteci.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qmogmgin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbsskicm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gpbqsmtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulgeberx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fndifesb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pcfuyyql.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lipyfhav.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlblxqad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbujpooe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhujssoy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzmypyx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dkcfddka.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqqgfpth.html


<!-- 参考信息 -->