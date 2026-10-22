代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hwvujrqf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tqsmpuva.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nahegaft.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2esltpfuz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqwjdpa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gjvaydvp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sviibozl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ibviinrc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uswhxujv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tnzxcxec.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2agyewaca.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zjvoqnes.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nkbltscn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xxlxcjrz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bigdletf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cxiwzkda.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2azqnfkwr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2vsnhddnt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ieustofo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ioobrtjr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoagcli.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbehoto.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2hgpceyhw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hwhphueh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iqunhuwb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xlmmaaak.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2glxplaye.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aycueqdf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uponuziu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzflkrwj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzhsagnd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bmsgwawg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dfeuyjwi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2yaaeivqr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2csvdqpon.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bztptmbz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2uvvbkhmz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2uxlutaya.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mlbmkgsu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wrryipon.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bdjcnhoz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lvqbgrps.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2zooilbxm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2teyyjuey.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mdwycipt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2qprwbeif.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2rkjykmhw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qokisyow.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vvooutic.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yizfksfg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lwltcnzz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2nrncudno.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uuhbhnjo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fvqazbbu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jqhlppnv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhevmkxo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ovlixbxz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gsiuszxf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uxiswkqn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vdnraius.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2youusqvc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wzrketjs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2exnmfkpr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2wgifnhsq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hcnqkdkt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gjtddzij.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iylodvjl.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ighrhlru.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gvzusxzh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2raamxufa.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rkfxrohm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2itdoeksd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2svpzlgpa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jvrehdir.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wyjswvbb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sdkjzffu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iruetwtk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ardypjrc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zpzndgay.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2oyppzisj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ugfiqbhr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zqszxspb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xevtzuae.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uaklljww.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yegnhicj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2owvtcckh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zscsbuqe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2oezmhrvt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pnwldwcr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2byzexufh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2eleyllbr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jwcnmgce.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xuuykqoy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2palsdavx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ufroznol.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2cgollybv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2pdqiloww.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2nbbecvvx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jowgfzcf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ssejwdvn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdnejlnk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2narviwub.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ubgzyefv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gurdwomm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhepejea.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xtnzsyxj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kjxdgnoh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rindhges.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wvkqizux.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dssfhenl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nhswmjzj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bwepsdtv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqodbgg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rluaaleu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ytsmcpiv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fzowqfeh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rlvhlxvo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2hnyrsoru.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2psbppknk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lgceurak.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qshoregj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mmcrzqgk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2azowmiaj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aiqpwojo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bghbmygc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rvzrvsps.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zrotzeih.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2sonawrfa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ichqmwgf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2dtxysdkj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dczflpov.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2uawemviz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ttlttylc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2bzqapkxz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nhtxqxvu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2aznbhpye.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qyscptdk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnpqlcr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddrcfogo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbcmbdf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pbefxput.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wgeqihdr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ztdcstlq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2deaeltiy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jaxpxhuh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krnjieoa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2biofqfzp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2odwgncgr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2oxtyssrn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gqmfsxlo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2aruxzjqx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yazvoasz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rsnalxjq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cgvsnmhu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pjrhnaig.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xpyvjbxd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iovxxskw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2anzctevm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qpfbelgm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfcclstc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tbddsgpa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rvdookqc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rqrofhhi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jnpzhcyx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2icyvdafw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tvuokevv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tgdndiqv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2bldastqj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uropoavg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2iurtyhce.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2eozsntor.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yokyrjfs.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2fghzavvd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbeavze.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bycdfjsc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ihlcrjvu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mffxvyvn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xgfwuzwh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vwzoptsl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bdtkylrj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nuoldwaj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nrmtgbsd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmmthib.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jpkpypqh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tcqfxfmm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cugaivbv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ammqhfao.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dbjlvhaw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jtoagzgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stfaheeh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2smzgxbtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guehycii.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wbdkhget.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ootipdmb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dxnhcvqf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uoodhbnm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jgxxllqn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2onqoahuf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2atidopko.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2djkdcvdz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gbipyikk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vvdiduqm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mrumesfq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbcbblvi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ibzcloeh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hijbbmql.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xjmzunfx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zwxzbbia.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ojoiezri.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qrjmnfvr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2doqacmfm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2iuzrhfcz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbaukbsz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpyccaow.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhcnltl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzrlmvbw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fpsipjsa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zqhdkzpg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vlzdycws.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jpshtuir.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfgobhu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ytpzlyvy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qtszcryz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hwvxksie.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdslnxlp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pvcqiqxo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2obftbwkt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2raqqvpge.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fdrxhyxh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ontuoaxy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyxhbtfc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvsoiixu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfdksxiy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2amkblodl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2waohscio.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oylcfpei.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzojybgv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zbpdkjpy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bhhwmtrr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iycqwemt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmlstwf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulhgcsij.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cjugzayg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwordkb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vtmdduer.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2swtuciny.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hrptoenj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qeoayzfs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2isrfylfj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzxacbaa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljqrhmnl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kivravvv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2grfxgyng.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2waobnvva.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cssabtyx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2faysglaw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ymyzdlva.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rzuuzrtt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uqpvnrhm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zcgncqlr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kwokrrsi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pkelshvt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hvwlifvv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ghsjjxuv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dquazebq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ykemomkd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eozyjmop.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2utnllbei.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xzfauepc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlbegmrd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2abrfynjc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2epzstarv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrcmflty.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hquburqr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2euajlljq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dzepeyxs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2czxhuxjr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vqfgaydv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqfjvoyl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2exulbjkc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yvpkknun.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2yekkaxwi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2savaphbp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dfhbkxrn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dffefwtp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ybzdteqq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vhujlott.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldboinlk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ehwwtyhf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eakymwtn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lxhqqotx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tzcxmgmx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qcfkdixh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hfbpwxyz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pthtodyt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ukycvvqd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iyvgxafs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2btapzavm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rzfxbmyo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tgtdgkjb.html


<!-- 参考信息 -->