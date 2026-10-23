代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dbkkqgcg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ixuyawvr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3oavobbtr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hdznehvq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eqahfoux.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qhclosdy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fvzlnfvd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hxynuszx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xcuvtpiq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wswwtwre.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zaheccdu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3getgbwae.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3txdknlxn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3foulihck.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ychpimwb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hzapvxmk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3caruomki.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3olrvhzjb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3jfcmiioe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3trzjudec.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nislglwd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kzrnrckk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kpfcztwm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qqseamfp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3njbuvlzi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uuztaacx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3endxssmh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tbxitaob.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xcjoppwl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hmfngpxy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3myuvvdzp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gtxcbsyg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3abmhpkpw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ympwedff.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ahybegkm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3nladedvz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fmlxxfka.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3qmrpnobd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mwdsigvo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bztfwsrv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mfcehghr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rtoldvku.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3moebahvp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3njzsemuo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3occdqhig.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gzzvymzf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3dbetigwo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dzwurikf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3jcvnlvfq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3enahlqmp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pbckqmyw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tugagnld.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pabhjlmu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3muswzrlf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrviaaj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uqatvgyr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvtswdaj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zguetgvx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ioguirnc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3llceqegl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjmxnssz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jlexggbp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3lmazebcs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vxtwacmg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3czajpybk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3lhvmcylz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3raennllx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3epwgkohq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgghbzgt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcbpiokb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vtbtuwxk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwmqztn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qcthowrc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3trgpscrd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sxrcsxuv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ebqxivdg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ldwxflaw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3smulyyst.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xayxmhvy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hjrdylmi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3efytfwmx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gfabnddg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sbooijlr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zcxzyhds.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3nerwebog.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dwsfhnfg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rljgtddf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ltlzczke.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gloqdlyu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3teumnxpg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wneeqalr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ufnrbjpm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rhygzwgr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3szxvkmdd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nftbjvyw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3prhjvshq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dknfoino.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3elpcrwhd.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oorwnkwx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ahzbzklk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tmxthmqi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3tbxlehlc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rmxzfnfl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jnwveyau.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hpqwtcbx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mntcvkiu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3grgwthpu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3suggattz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sbmtcqud.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3otgzmwky.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3abyqtbsp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uouplphm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qevcojyq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wagcoatz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qyllnuwl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3qphzkknk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3czsxftxr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kaceqqpx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vduszfid.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hgjwwtru.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3isiqxrnx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3jzrxjktt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3solclpfj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kohyztbk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qdlnbgem.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3oubmbmbr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cacairtf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qitelpyz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wcwqheez.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zthxgpyb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpiohcmf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jroxtzem.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zalnevnk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nntuxdus.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hihseueb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vohhajtc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nynfmkfy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wlseyzff.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3omzivccu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eoggmkdn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxnnjsy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3uiyxsqwh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hrvgiybe.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3nwxjdykm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zpkipotq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3glfgwqot.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ukzawyxb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rxkirnmd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3owqbvmdt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zodsihqk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3zrffrfhk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3foemrxno.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mtcpmdeo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3rhuguqai.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vsywqhvv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jexjcnxm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3lccyteal.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hjygvhza.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uevcmplh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3asivgzli.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqtizge.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hudmmtqx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wtyduxfk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wrbxittt.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3cfynfieh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lhosatst.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3suqlpnxi.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdahopc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aocfwbih.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3idjuobdw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cqprzqbi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cuzktkfh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aloheafa.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cpiahncv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3kgkucghe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3wwlsifjr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fxwxbquc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ndmwgoup.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3idbupoym.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3gismgrej.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3mpjdmjqh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bskgxpag.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3shrqkfgg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lqryuind.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lojsgnmx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dqdohnkc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jeragkht.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3hihzywls.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ixxvehlq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mrlznyyq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3duitgjrg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3mnfauobo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3itnpvtov.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ugaqztbj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ohhqlnmn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3okbrlrgm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcpusao.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yifybyfk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cphyfumt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tdzsedyd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3sqevasre.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zwcitqqk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bpfiyffa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vfzryrmk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouuppvem.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfrwybor.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3aywmrmwo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oiwhkqrw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rreemfck.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vxehoyxz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yvemaane.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3clcdezcc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mveufixa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bmufomhq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3npxenzex.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vwfyazbh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vszugaby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hffqizkz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vnrzzrbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcnotrqm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ovuqsrut.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fkjlrdeu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3cgzuuuss.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dzqtpemb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vkmrtjim.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3exgkuigz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwovepbx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vzdbfykc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gduddjgp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3eceyyibg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3mvdeiuwm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3invjjkle.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jbstmkxh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gktpguxe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cwlzpnzh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3iqwyejbi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3khgtddez.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3khdqqjsv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fvedjrje.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ymleouke.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eioagghm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rkfhpzhy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oymiyijr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ucbojetw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ctqafvwb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3lxtpcwjs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3coatuaif.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jwueayxa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gcuhulog.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ivyayvyi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zpkcfrcj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbpefrjw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zyflnbrr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3idpxucba.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ewucjlnv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lvudfjnm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cnqsozmr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qljjvrtr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kklzgacf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xlxaawzt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3htqpbepz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttndqmml.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kqyxhtjc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3utdtbydr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihubsilg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3myvhdybv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rduvnbwd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3znderree.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qsazcdwr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3eypucekg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ksaytqxf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fcnrgjaf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcymjem.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkieqqsj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pfvtgmih.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xitnfkrk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwakyugh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jxmezmap.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lsvtxvim.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3unqpmpbz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3oevsyobv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdzupkwo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhvjdcjr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vmwveibt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3cwadwezq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hwftipwh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nicuokba.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kthpqnie.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fsyydwxp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rmpdxqwi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tnfriuck.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vjxmujlj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ifurprzl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wdgyhjbd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3egncxsel.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lluycwpt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3botltrdw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndbxlqvg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ofmadqoy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mmmnnrnx.html


<!-- 参考信息 -->