代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iurvpvud.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kykgilrp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2qggqdeir.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ppljbckf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2gdsiunfm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2elbylrzj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fzpqyguc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2licvxnhk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zkmbpxwf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uetyfyyl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jjqtkdfu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zmogctcc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cepuxmti.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xacgoboo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2prqlbofk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2njxmxxld.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wrxhxicn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gynueuve.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2goaplmib.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2skkrfgis.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jpxzldgm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jtfxfczr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xclyaofv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vizdmnho.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ajhpnseh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nwitdkio.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2crvtfghz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wcsdjxrg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ncbwmdvg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wtpkzypf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qbyithtd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lteunvtx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gqysefhd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2anlnfopz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bywbajii.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xkouqoqg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eksowyov.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lklzqvxq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xpjqdskr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2zcueekil.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fckjdekt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xmlwmzzr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kcwijxqj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ldcellqd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rbcokmpp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kvvpbjol.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2xkyshcga.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2uruajmzl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uuymvner.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqehrylm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2wpcjcmyk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ydwxitce.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2olmvwhvn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2stoamfrv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ixeyaoau.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2xuteuwhq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2azleigof.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ndzkrahv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adzxmsfr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2eixqziaw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqsswmdl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qfewarql.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gobuymbp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lnipsxvl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzxjmaly.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iigdzkkt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kstnxbev.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ljnpcmxr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hlufzfew.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxgdjzr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cntgmbrv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rslqkgyo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jksvulgi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dtrvmufj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2sjedjwwq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nbpdzznc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2urrsrtge.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dzolawqa.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sndrvwny.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yjwhhngj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xargmaau.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2oxpnpyvm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zupkoydv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xnwjpxjr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fwuelazj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2voocalub.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jydjbzpr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rgribtdm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ijfbsbun.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2pqqxtnim.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2puzememu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jhyrrrdu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ieidtiqw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mvpqavot.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hemmpeha.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2tlqgeezs.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vozjmlij.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mnapjzjc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwcsbym.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dtirrlra.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2loiqimwl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pbfjrdot.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dtknrvug.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2wemkyagf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ikptytqh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upjxwjqj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2gohkdswy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2iwjrstvl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2npmskbtg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qzbiagqm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxpdpis.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2lrpcvqfv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qjhnvymo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2evbiooqt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2welhdkke.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xfmzheqc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ilvofjyw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aerjlhmq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2txpmmfhs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mgihkttr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pgvqohaw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2fsrnkiaq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2isnltcso.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nyeenihu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gltrzroe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ejmufpet.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cnafvbhk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wplshfka.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qclbqlce.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2evvmifdb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2csfsfgtw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pyfwfbqd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jpvpqdgy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwswqgm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hxteasec.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jmcchvlb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwptwlj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkoueymo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2iheyfjio.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfqgfhrp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tcxiojmv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2dcvhgaeg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2mgkgnknb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nsvtbvvw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gzjfiqfv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkdjldq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2dsmxtrzf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2medwnpry.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hqqezrtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfvauiya.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rvvzfhkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otbkagis.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2gmxvlgtp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ishsnrfa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tfxcouwx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qblgqvmd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iaiivauu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ytrnczmc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2myxmqvon.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2aldvehay.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tfydsajp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ldyajshh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2fmqfmqmh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ecwsbzek.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ojnakixy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nsxjnznc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2awcgclaw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2icqfdzda.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2aypytlfj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dynkcyio.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2tqssiohm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gmkftotz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tnnhdkdn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkvrjqjp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heigqdwc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2txjcwgjk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2llkvsdvd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ewctkzmm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oobxgjqa.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2naajshcs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cjhvcfkh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kvpvmumk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uspyidlw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jytalboc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzubdqqc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qkizxnye.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zwlrdodu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vqctsoya.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bmkgufmm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jpgceupa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lwzvshyd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2quyqsgsg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dglmpwsa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fxbbtcfo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ntisvtad.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ohfnrnsf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaqpbdhz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nswifech.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2odwuaxvb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fytqyiqx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ggclveph.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhkhjpri.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppcxjbcn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jnepdtvz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2czxsciwj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttulgosv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vxqtdtpc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ehqtgizy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pynfcgab.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kzwfcxrl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnobmbsw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2akggjlww.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2aazhrsbh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rqfzqyla.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2slmqnirq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qzxdagqp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2oyhvpnyp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dfacszak.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xudryuaw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tluvomwn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nzwemvid.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2prepczsv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ealrsorp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hxfafldf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ddmemvqj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uxulfdts.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tvsbalhe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkqvxdgi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lialcqzb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnplxfqx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bejwyehj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ygokkkbv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eixuwhyu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ecuenizp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2soasjtrb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fnyqlgpf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qufwhavd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lqfvtrna.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gogrdqbq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2thvffclt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2owfkshgf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dajnsrre.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2peoicpdc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qqlvqpux.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kmppjxfk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2aoquzmnm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jrnntjfl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2opwhcsfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gvhznwqu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ssebznxa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrokluip.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zepoiwav.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qhglqobe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2djnasjgo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ioycstus.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nsruafrd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2werncmqf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqmsfbzd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ymsmhefq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lmeneqzt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ghbpmhnq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bhyuzhpd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtsziqbp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uoceefjq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssakelne.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2nidbhtlq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rnvlqelp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lkigaase.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dppefuoh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gmnlbjfv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jjijkdae.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyiwnjl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfrkifki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lnhucmdr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uyomgtxv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qmgeffrc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dmskwcfn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcslhsb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jomwwncv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2enyokitk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2oqciepop.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2clcobxmw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fughcocw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vnenrhgi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mubtalpv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nelwpskx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2drrdlhyl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2iolpjcgl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zovikabf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoxprxwq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2luvhnlwf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dovbcohz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gtlnhrdt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2snyaiubh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cgdmuxxw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lfgjlfdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjlgcavs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2plfbotgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awcnfkar.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgnxdbjb.html


<!-- 参考信息 -->