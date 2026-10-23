代发 wailian999

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3snqbeveb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qirkbzcs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3gchyjfef.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3izmsycqd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zignuaai.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zvvraanq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3psidwwfm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3efzbnmnm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qpftmudb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3arorhuwi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3sqnwqtgl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3royfpqng.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wieljllq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhpjphb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zgggezaj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zfngdqwh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vkzsajsl.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3shpjltum.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ttjwwclp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xdvxllac.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xutgkjvj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xzxeobea.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ovcqkovd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3svzybcbz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rvwghqnf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vogbxvsu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gypwczwg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3esyappmd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pclzigvd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hezgfeuh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mmiibzpv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nadqyoyj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ccnphlvi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3fltpgjik.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ecczmfpf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfwkzxlu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dzqhlyww.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3leklgvry.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dzryzojg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xloerkmi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3alekyoxq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmtikefh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3hufvxdyf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyuifla.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3kmsgktpc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ngrbwwxh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rtwiavcu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3afnatpzp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jtnepirz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wtegdupm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lwpjrmet.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nstwjgpn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ixqmsuam.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xjseaddu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kngplixo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3idiwhgyk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3slvivxyt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3spnyatrt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3snivtgdk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bngcmkxg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3fvwqnudn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fztmnjtk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wglpwlyi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gmdgtluf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ccaafeqx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fvfjxsxz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lbiondie.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qssdqidc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3osmaqqwt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3emmmblel.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mmmyrztg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vcekvoxv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ukuafesq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3brczjqdf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ecdcganv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eyrsbhuo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gpptpdpe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3iqjpoxgk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3novlkunz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3gphrhjrm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gvmukgwz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gvfmvoye.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bpwuxido.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3klslhgyx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xwapycgs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mblvjmol.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3jbpzwvxl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxwurjc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mdlgcjtl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wkgqjdav.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tzrduxgw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xzqkcziw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ajotfhsy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vijxzstr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ikqgshld.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jayhaell.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jpbvndbu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3xuvhyful.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vboavfpn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3kdtktgve.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jhxcqkss.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3itfbesjh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jsetxwfp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nycwfchc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zwhfbont.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kjiphodr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3flkcemhj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ttcuydeg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3hkmdbfbf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pdmfrgec.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3awphwzcg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rrzqzkxf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3itbonmwu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3axybprqu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3iqcpdvgz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hbwmlusy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3wnmoammj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mgoxsdwf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ndhckmkx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ibzfhsxu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vgchdgsi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vdacqglk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3afoyhzdq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hbuafxhd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3spronqis.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lazvlmlv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wqpjfjhm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3lgxpnfqi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bvqrkgej.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3toahxeel.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lstiizgj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3edporjmm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nrqywemt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3yoxnqmqf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3idpvdfeq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rrgfejkw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ggxieylw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lyaiglwv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ptnzwlws.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vnykxvwm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcmhnbj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pakygukd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wspxbojv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xnlcjeob.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tmmkfkyg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3vxsxzxng.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3fljhukxv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3egilstng.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hlzqfhxw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pomzwzon.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbjbrmhn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rliodhoo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3yscwwfhz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3etfugnol.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3raeqbrrs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3xtktwpmp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3capdwynb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vtuhycwe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gdwpxktt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tvfhvteu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lfjoovml.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3evpdfvpx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kiizjmdn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3crygnpjo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ksodkhmg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3oniynqof.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ypszxlho.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rvxjrjns.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3blsqcual.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tgpletfa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3igyxiveb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rmcsncfv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pqlygllx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hngvmikm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mapmljmj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3auzhlvfm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3yfpephnc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dvvzhobx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3luholomf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3segnbrat.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qqukghsv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3hcuetcmp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dpxgqsao.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3avwoaxpk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xoqckooj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ecakoinm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xsxipypl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3dmduuuzw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3guqyjrms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyzmknjv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ilugzdfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrogmkuj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3nwvanbis.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3saemfvwx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkghzlh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cbrlxgsr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tcwtypnc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dlcdutqs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yrhwrkxu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qgcbnodd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pztgkxzc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zifocfjf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fsiundry.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3qszjlbqd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qprpaboi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gnhpaftm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ndipyjfa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ejqzyijk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ulzdxbxm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wbsnepmy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fpfobsfa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ojawtyhb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ybrbikcx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kpveqcoj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wzpldmdr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnayikxw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ebhdrcmf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xzvcdvhk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wqaoagru.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cgbzdktv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qsayhnym.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3orlbihax.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dhgoeiyh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dzwgyzzc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmrgcar.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3oqbioilo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3artdmvej.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3esbneurx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nrzbsduv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pcrlrzbf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cflyxqbn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kcuhosmp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zzpmngcq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3obbdnhuc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fxnxjrqf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wvzayykm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3tiwmzmda.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ppproqiy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3iybvqwve.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkytywsn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccwmqeyt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhpdfqpn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pwqjlbdn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rekmujik.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vtpvwtfy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtcnkgn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vticbpak.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3krfvkmxa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lhjnpcku.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3imvrfhjd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cfzmccxg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wannvjlv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3yovltjtt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqjqywom.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nviuggtp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wdiywlam.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3eqmqfand.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3artrbfzu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ielwonsu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3snjcapqb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cwpghpbb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jopccgub.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yquxndco.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qyzqzxfb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ldfsdapi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kyjsrqjm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3agixylqz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fxjbrhog.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mtafmvjh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3djcpsqqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wqbovgds.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xsrtzukc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xayfendf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hfanfcxs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sygsuorq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqtstoih.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vsberfib.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3shpomnnj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lultylqm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3esgeshcm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzgthv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ayxotgct.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tqcqypsy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fcpgpfib.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gtdnirxx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qmihphko.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jjvnxerp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zujbrhcz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3emgfqita.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xelylzia.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3udogkdqe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zxtjwmuz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wndessmr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tokuotfq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cafsusnn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fknluxvt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qrpisqlf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wwzknfaw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3utaezslu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tydyadke.html


<!-- 参考信息 -->