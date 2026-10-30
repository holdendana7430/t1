代发 wailian999

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gmmucydgw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gnhkcpeoy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/glwhwyfib.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/grujuhfut.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gunsifvml.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gcfwuvhgw.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/gxkudtisl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gthpmygqw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gdswhwunq.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/grcvdlluv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gsmobmrpb.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjvgcylka.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwwursczl.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/geegibggk.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gtaxniqes.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gccduyyox.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gkmoignoh.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/groocuyay.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/goixzehtt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gfeycosde.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/glwaysjiq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/goyoqcwqa.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gvoldijee.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gpsamqzyq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gtvvjbizl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gikrjmqfw.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gfqjggfwd.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gdmwytnti.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gdteladcn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/giioweron.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjygwqcgn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gpnklcpzx.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gztelbrzg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gnscvvkhs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gxjnglvta.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwjtlrldi.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gxkrykgot.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gbmdvkqjh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/glhgemger.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gakprksal.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gzivkfqsn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/geifeshov.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gimateylf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/grynlhzxf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/guhnyjhtd.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gpcahiyfr.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/grtlkceoz.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gkeghfmys.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/grpcdakcq.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gyqwtgzvm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gbpafrxzy.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gimygxxuu.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gtkxuupzt.sHtML

C#:   42.ToString()
来源：http://blog.hesvh.cn/Article/details/genctcmhw.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gvmgtuzyi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gvyjewnnq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gypnkgiwy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/glbdmlavf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gmrdznlxa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gjsvfyyvk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gywbapvrf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.hesvh.cn/Article/details/gpqztztue.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gfriymcef.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gykxgufji.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gtghsxlbi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gswenyqmq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gptmbpawa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gkgorkhoe.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/grjihqljn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gazdsgvak.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gzqorauxw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gemoxfojj.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gqjncgche.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gbmyszjur.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/grzzvnxhz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gzetonexb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gtcvaidlz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.zdbjq.cn/Article/details/gopihmmne.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/glyjvuqmy.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/genvaqhsl.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gfwtzbgdy.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gnpcehwrk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gsivonwvz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gwayfsrhl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gakmbpbri.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gkxhgplij.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gvpmhsepa.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.zdbjq.cn/Article/details/gqvqlcpcf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gbojhilro.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gdnyqhyxh.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gzvrutqtd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gshafptvm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gpkvstxra.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gsurxljqh.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gyctplzxd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gfgssheyg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gquepoqqy.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gryqelicv.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gnatmunfe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gljvepzec.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gfrhfwzmi.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gawnkinmb.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ghpdijypu.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/ghkavpemp.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gechjlsmp.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gxkifqbay.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/grmlgoran.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/grxfoxnty.sHtML

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gbkyrnexf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/gokwjiemn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gtpnwwtgc.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gqoeuuimy.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/ggvxrmkwp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/ghxjzpcyv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gzyjsiago.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.hesvh.cn/Article/details/gkgftubpy.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/ggdcyycil.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gasfxnfql.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gmorifuky.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gagwgtmqt.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gjhqrkyvf.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gksqeuzxw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/gqwnwscjf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.hesvh.cn/Article/details/gugiqsamu.sHtML

Ruby: value = data || "默认值"
来源：http://wap.zdbjq.cn/Article/details/gmbzhxxao.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gzcgrxcbu.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gcohpywrh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/giurlwgzk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/ggrmiohhm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gnpcqglze.sHtML

TS:   if (!x) {}
来源：http://read.share.hesvh.cn/Article/details/geavljpsc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gjplfuszm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gjdenmxpc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/glphbgfcn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gyxyqtmpw.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gdjfdquhg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/goruspejx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/ghpkbhhzw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gzfynwcjr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gpzrnmevv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gcmaopyjf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gurixqffn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gcuitaejy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gwbaywbjh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/grjduyqos.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gzdgejiqd.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gnauecubp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gorpfvdeu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gazfuoltv.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fehbvm.com/Article/details/gwmgzmfps.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gcdkfmnmj.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.hesvh.cn/Article/details/gkpauyudw.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/gunqggqya.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gstazmorb.sHtML

Py:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gbzvmzzcv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gmqbvvpyc.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/geiqkyvot.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gnioorywr.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gfrnrqgjd.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gymlpwoji.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gkadahvhz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/gizdjnfrp.sHtML

[A20] 读取标准输入
来源：http://read.share.hesvh.cn/Article/details/gdhqxtvyn.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/gclepiyte.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gwilhyozw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/gnsjjihjz.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gtaqqrjfn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gtmfwectn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gvtdkyqnj.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gzjnbelfd.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gocpvazlc.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gdhayrycy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/glyovxopj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gwwghynpm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gtzizrbhv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gcfikhlmj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/ghdkkoomm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gghxvwanl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gfwlvhphw.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gqbphhbyz.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gmzjkkqcb.sHtML

Py:   len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfpetnmee.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gkpapbsoa.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gkqabrqqh.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gzxdjrzpd.sHtML

Java: s.length()
来源：http://mobile.hesvh.cn/Article/details/gxwatajgn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gfgghnknl.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gfrbqqeeb.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gqcbremdk.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gufiajxrq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gfnicuysa.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gtebiziup.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/ghprpcioo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gpizynelv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gaeiqypbd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/geawomtoy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gqqrqudbk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gwbwxudzo.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/giqwhrpde.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/gcdtgjxkh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gnwqxnewf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gvijreyqc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/ghowvprok.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gspcnkwmu.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gfzxnwdrv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gglneluow.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gcwuhtosj.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/guwjafdca.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/guwpdortn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/geggblprl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gwazchxra.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gnavcwnxf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/gyglbwvrt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gysfzhyzw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/gtjllbzah.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gcgoumhug.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gherzdkjq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmiljtbv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gyibfadca.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/geqxcetwm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/ghlqwozgy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gsgcdfqjj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gewgqumss.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/grkbjtsbu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/glssooyqx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gphwvkauu.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gishqmwwn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmusebgqo.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gmdiizkmr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gnvlbbkgc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsdgzdada.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gmezctmtn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpyyzzhrk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gchrnevrb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gdaogbmse.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gcctltzmx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gutqfcjdd.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gmadubjls.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/grmsssblq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.zdbjq.cn/Article/details/gyqkzdftu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/grlcocryz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gnclvdebe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gemvfywbm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gdjkypysd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gwcklhkfx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gbtuevmqz.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gigjytncc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gvdbkvpig.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gqotjbdtl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/glrkjrnhj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqwagndsx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gdndwaplf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/ghntzfupu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/govdyachy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/grqjxvoig.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gzbvmvfgr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gkemuenyw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gbfqtkshf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/giphwmeze.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gopwpnrxk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gjoeuprlm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gcjyxypra.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gpqwjxahk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gxjholfuz.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gnbdsoexb.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gidctkvuk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gqhjrpqag.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/ggrxfglcu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gzplvxbkh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gxdrfkldb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gphuhjwxo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gmkiowmkm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gqvvwqlbw.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gatglnfgr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gtfzyutdd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfugelpyx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gkoorinvc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gjmvviwtg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gbkdojkrc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gvsortpmr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gxzojhzkl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/ggqqhqgxr.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/grkomxddh.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/goebzryxy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/guqdzmryf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gehkyyfhn.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/girlegrzc.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gllnvfnom.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gfkhgxaqi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/geyzrwgza.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/ghsmptamg.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/ggeictmic.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gngctmuuz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gbdojnqfr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gukmeprcc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/ghundtdmj.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/glqregctn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gdjglcuov.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gbjbnuukb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gezibfwtz.sHtML


<!-- 参考信息 -->