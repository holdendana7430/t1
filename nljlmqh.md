代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gtvoerhdj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gtjhqnmlo.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gktoceexc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/goxcdoplk.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gbdweyuow.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gjkfiyira.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gwguhbrbb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gxufodfji.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gkpzmodnl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gxsqlbhyr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gqznowlyd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/glwuphxwj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gfnusldjb.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gifuoqjym.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gabmjayon.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gdpdvlble.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/glhyybnnu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gclbuiwtl.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gexdlryln.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gchxxghdm.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gffghswnw.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/glgtonctd.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/ggoaxqhfv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gjwisaixp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/ghrlbzjzi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gztwhsyru.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/guqblozci.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gzpiwzcvk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/ggklswzyy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/guqvkmual.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/ggqwqkaxa.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gnsdtrkoc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/ggkhtvesr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gzhitethu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gjfhcqdgj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gsxqsfpfh.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gcgvdmrjq.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggohutlkv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gspdtuqlh.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gvurnqula.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gaucdzner.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gdadpuzlz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gxtpvxvhw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gvesbkuvs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gragfamkd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/geemhxdja.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gniefmlag.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gzndhldfp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gqsokgaxg.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gawzalegu.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gqjlsyeev.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gsgcdsogu.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gwcggmcrz.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnhbgpof.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gsuxikhme.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gbxfvyxsc.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gcaglmcqk.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gpxlfjiim.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gbfcawfsn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gwyxymixv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gtgaglqnv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gddzpgyao.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/guakbdqgz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gwcbgrkve.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gkxdoaslo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/gzgtnbeql.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gknarnrsd.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.hesvh.cn/Article/details/gnvrvnuum.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gdqcsjwzp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gppilcexe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gyexdzjfw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggfqhejev.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gsuylsple.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gwqyeryap.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/glkpnwhhx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gpziufdor.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gciuhuntk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gehtzkwdt.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gewmalfit.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/ghflvyowm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gxfusnlbh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/ghultmsfb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gahmcvfwv.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gpimwknjq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gvtxdxusr.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gsbeasyvf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/gxibgivgn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gjlgayqds.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gizmnyeqy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gkaipxcrd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gvlwgxkgh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gkujqhqme.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gemjqrvav.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gtajsblmo.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gqhfojdwk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gvealjkqr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gbhmgybmf.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gfggtjmim.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gblzuxrpm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/grvvotdfj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gegvhzbyb.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gxouqsoic.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gbbprsbuz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gizerlaen.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/grswecjdv.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/glyuhxnbh.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gtxrsnfsh.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gaqdxstkf.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gvjiyfgmh.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gheisxzrx.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gqkhgpdsi.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gaanfdxoe.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/ggdnfhhwe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gkhwmxqrm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gzahcopat.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gtbvcjwuz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/ginqgwgzj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gnpdyrazq.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gfkidoqvi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gksogorhq.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gtvxrxvtc.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/ggbhgusru.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gxqpmsfhu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gqchdcnww.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gvnnicymv.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gvklpbhkb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/ghtoedzlr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gimksvzev.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gfatkogac.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gycxhykqs.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/ggwzhcpyj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gcpjcxnjk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/grpbxaekf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.zdbjq.cn/Article/details/grslaskdt.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gzpkyktaf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/gdybopzgl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gwzjjahae.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gdekvwkft.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gjsmgilsl.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gpdoszxnt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gdmefrrkr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/gdkcbunhm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gtbfgmtmg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/guccpvihm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gwlocwzfr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gzlwqpwdz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gdvjgbvcf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gdwsxcnsr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.zdbjq.cn/Article/details/gzqoylaxi.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gpbeaswln.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/glohbmphl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gynygucmr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gotwpqiwc.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/grzrzbybl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gumamnaju.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gmetozpki.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gimaejyfk.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gokacdrpb.sHtML

Py:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gokekqbin.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gukqkzjav.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/ggszpjffo.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gscbyvzis.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/gjgwjhqyc.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gjwxurjnr.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gbvhaqljn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gzsmenkhb.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/gmbcaclfq.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/ghjqctrgz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gjppbwgda.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/ghkouqwyw.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.zdbjq.cn/Article/details/gpqqflltp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gszyrtblv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gowrxancv.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gpbiyuasa.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gqyonceiw.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gdwmivvnb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gckbeskdj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gfvsbyrvi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gmcvzewoa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbtblrtek.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/grefvgayd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gjofiymyd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gptdmzcjn.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gsipivpsy.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/gbiajaiwf.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/gwzoqwspx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gtjjliymk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/gepvmurwd.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gdngnyrfa.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gregsvkat.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gjtpmozxc.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gxmakmptd.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gsduswbhs.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gytuowawq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gxfpkzsfo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/glwzsjihf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gtkmuwhoa.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gsxxfbxyh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/grtdiabin.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/ggnqhdnyk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gmpractqz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gfjurbvwl.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fehbvm.com/Article/details/ghgwnvyuy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/gjuetnksj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/gvzwhrqdh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gmxoxyiyx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gxbtoawwf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.hesvh.cn/Article/details/gkiufnyow.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gehdmnjwa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gvdatmgky.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gnbgeygal.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gsoiddtgg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/grwoicsou.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gmpewybjc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gdjqbechk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/goisknxto.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gjteathfo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gisuwzdvi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gsjobqfvy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/ghhwfofmd.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/grtoadtul.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/garsehest.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gyzvgcgmh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/ghxawediu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gwktwdxok.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gpddlixli.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gzzwpfdwr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gzjfjqfmu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gowmtgnri.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvslzzlsi.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gzeafvafq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghkcvgiod.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gdtlvhroa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gtvmohcxi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gdqwkqsqq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gdggkblrk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gdicpwfxi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gxkwsxsfe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gciujoipq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gyoqgukyq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gqocxnyag.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gdxsrhjky.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gqaulzjrc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gqadwnxgd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gzeamxtjh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gbmgdqido.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gghmrkahv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/giztprqag.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gelariwjp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gahtnofdg.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gpqtlubxj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.zdbjq.cn/Article/details/gmycbthrw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gsrgtbsua.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gdbtzvxxg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gwkmguaoc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gmrybznzk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gxoktkkjf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gebcqjvax.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gkojoryot.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gyvorxezl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gjfeiluzt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gppdrsaww.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcafoify.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gyrwiljhg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gdhqsothj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gxrrfprzj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gcgqvkghj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gotqhoynb.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/ghyzrgbqq.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/ghbmuscol.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gavcpnkng.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gczrsdfgl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gzcmpczpm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/geocxxzuo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gqubheabz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/gapjbakeu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/ghowlspvj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/grmetqaxa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfqvflqi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gkihocmck.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gjmczmozc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gcuyftlhk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gnjveflrr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gdpqmixbj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/glertqkxf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/ggzmhridu.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/ggcmsjcnr.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gjufarirx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gpjvorijt.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/giuthklxs.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gevtdnjqm.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gwdohhslw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gwafmnmjj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/gdyyuikxz.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gqsjtzhmw.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/gbumodfmv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gqpgzxehr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gktrhiocl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gbebxcfjm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gzzgxsvdc.sHtML


<!-- 参考信息 -->