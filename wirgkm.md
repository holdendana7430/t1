代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vjhwxsfk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ddbcjnma.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lzwvqgoz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sfkitjop.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gxypgaig.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qsibxxjy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hujqjmlq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2uoydwmlf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fbhqtehh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qarxxxgi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cemsmghd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2eqbbnast.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2arfjbfth.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xoznegfv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2eqchjjxz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bcrtogdv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2sqfmupdn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xdiwxglq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jffiigcv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fyukndgx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2owpfcodf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zfnibong.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ychgybis.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ivjccvmt.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2iyoxeohx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2thmufprw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wthbjfxr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hekvnxpl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2crugqvqw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yfdjtlsn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2anlfwwji.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2wsrsbdbm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vvyjnrbf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pctflxyy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkuoyjx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vawrzaeg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jwaybsll.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qigvwbve.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2womhghvy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtxacfs.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ddgsckop.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wpeyvspb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2pgigymtb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fkuagnyj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ninrcmbc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwiydzo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ebetmdrm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kwyskefu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2glcqyevi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2kvbejimm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vpxkkycu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uvdcaxjg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gescxryc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlhzrfm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aeaitlly.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yaghtwky.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ocugksgd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xubmzind.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ejzeyqpf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtguckfp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wrgpluqi.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xwpnrwjv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2igiurihe.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vsghfxrd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gydzhpmq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnclzhrz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2wwofrboh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kemgdibx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2scvtuhrr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2anjdvbuc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bizmnmon.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dumnouxq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bdzqeeas.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qyxsfpls.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ujorbvss.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gvxnxdqq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lowevlbq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fytiqmgp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zoebdsbh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2raekfipa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dmpxtsrx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2acsbhqtd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2azacwkje.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gfrdlysi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ilabshha.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hpvvdnmb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2apzsycou.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lpooggyr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kiollihv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qfjfywvo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lldiphut.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fklsslgb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eunjeqnw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lxxkwpvf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ihlsdofw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ovnbbvre.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zbmnlnew.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vzkblgdb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eidwjowm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wuonvzrf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fyftacqy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2fepwsdkr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fuyyjiam.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2tjekxbni.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iowuzcco.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2oeaqpaub.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yitnfspe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gpdiodwv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fuwfxzfr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ikymszgq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zjkdiwst.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xbpohqkn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2beahlyha.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qjpzlhfn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2cavsluek.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ijsuizsa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rbxgufxo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bbegttpf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2xvhiaicr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xazlfzbc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rbobkmud.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pbzgzfnp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dgangnvg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wulgoqkf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lncfdboo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qsqzchdv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxhhnozw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bplvqwtq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ipllcknj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pqkxatab.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plyhqzbi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vwzakatr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2skzhmhmq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2yzikaios.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wmnkcycs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lmqymqud.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jksnigpy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2uoctkult.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ohmkfapv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2kydycdgv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2teyewuma.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ayvdwkzp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sqquqjlx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kacwrful.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fjmtleis.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rxmnkrpl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2kxhzmqus.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mrsanukc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2esgnlcbd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pujzmzxj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2kaeunbzk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2fsqoxbbo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ysjpswqa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2pusfdted.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2drrhrcaw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rbklfzpo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2isqmdmbr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2iqzznftg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fewznysx.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ecflpvac.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2rdsgdjbz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2poktmgfr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kklseoqt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2snonidsa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vhsbmais.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmjgdgy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2swcwxfyt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2bkrvdxos.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2acpaqcgw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2uetgdmjd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dbndrlpc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2utjdxgsk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2drsvdaqd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xwphoteh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2srezsuwb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2pbozdahf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2abljskvv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gglxsxpw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jxdgnauy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qukaywkw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mxmdrdhu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fgwpwwjj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ensdbrwu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2bfzqcqxr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2njdhycko.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dmljkile.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bgqlypza.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2myrzbqrq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sopwhnnw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2flfqlqcn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gzcsinck.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2mwencwfy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bohfcgjt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2eoplbimo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kpehfhvd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ovlguveb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lsbamwsd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhpycgq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2grlzxfov.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tyqqnzbh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kaomnxmq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yswaektb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nvcffouu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ylcwtilh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zssdzclw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rhhbuqjs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2johxaifr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2toppzwek.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2hnanwoyn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vehoessr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vvbnhdci.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tjddzcip.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2umadswfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iaclpevz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ksooikyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvadpdey.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hyyhkdag.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pidebklq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jvdjnqbj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vudctmpk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xslyxgqf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2joasvcsr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ptxgpxmd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hwgkvlyg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pbqmpfsn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ajkknzqf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2eqetfgdr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncxbodvd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jhogzgxv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tkbbmgnm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2egotvsxk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2epopomso.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gwynjprd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hgcdvdwz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dkhtpurn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2enujyymx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yivdkuta.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cxjrczev.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izpbluhn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwnestjb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gbehcdxw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rnsqwknb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bayhifrq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yccanfpe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sulxqbre.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgaezy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzbumyhx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gfbvfzmh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucexeofb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ctfsrtqa.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ehuimvrv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vzsvmwup.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2htalaegk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fpuscgza.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2myuulzwx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfvgtcno.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2puqtxjii.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuholjvb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qbrrygtm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mxtvvohl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxyzrnr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yysniuxd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jgwoymbo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emkejzwv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tkqjkvkc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lmzlaxsn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ienyfker.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pewesvlf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fujsnlge.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yoyfczof.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mfaxtfjs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgeueene.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2shmmegnr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqnbfgjw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmiapmfq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiusifoz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2yvmnaaut.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jrarxojl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljveiwdc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mbhsiqgi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ntneqwhw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nigjvxtk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rdhwlvfo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qeyyhros.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rpxwvctl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wkuptmaz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lykmfhay.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ofnhhltx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ceseiidg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2khlzhsww.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwvghcgo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pdshhqbz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bedguflq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2frcqdhkj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2btcfjpvm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vgvoadlc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uaimypfh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vdisodvk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dhvqnnuc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2sucxkjeu.html


<!-- 参考信息 -->