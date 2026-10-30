代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gupqbbmrw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gmttsmoub.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gjqwbqbns.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/garmiumse.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtmbhlsfe.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/goehsjfrp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giwyqpmin.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/goxqzapxk.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gbvxdemhg.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gyxayrwqu.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gyrcbynwv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gqcgsqsxp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gjypnadiy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/giaiusbwa.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gzviebxqt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gcclnicxn.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/ghhmtbxgw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gjpxwilgk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/guedclcfo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gusbevdsy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gxtmrsyrz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gjcaanqvh.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gadxdvpeo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gnmpsolxk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnqefehyn.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/ghzxiuqvw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/ggiwkahrf.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gulrqoxdo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/grremsnqw.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gulyomymu.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gmyjaadbr.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gyhvsnnul.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/ghyzmtrmm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzzqvkpjo.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/ggajsomtm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gctimdzuv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/gloaymsjz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gdakysvbm.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gkxbyyrjm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gzbpgqxch.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/ghcpliljv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gkreffpga.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gbtunulgq.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gvwxbztzg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gwyqmlxbj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfkzkgndr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmzwmgr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gltubjear.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gwnfgyaip.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/goxiftpkt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gcpyluqvq.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gsqgueavx.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gqzzgfgmj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/goavngrtk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gbebciqcm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gaxuzsfqk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gsutssfho.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gklhracxh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gkybeagkz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gsopqwurp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gklpengqz.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gnclgcydx.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyplftuf.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gnvsyncjm.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gmiifkrsk.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gvbrbvreq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gpddrsocb.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/giftssakc.sHtML

Ruby: 42.to_s
来源：http://mobile.fehbvm.com/Article/details/gbnskqqjt.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gyueldbeg.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/gsczecqfz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gxjwtbiny.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gexejibno.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gwjakyudb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gniblkxin.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/ghbhwcjpa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gpuxkufaz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/govyjsodc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gbfkxkdlu.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gzruswhks.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ggkubfmqj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gglreiwjr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gnbxdlxtf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gndtrnmor.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ghvicbvrm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gygwiareh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/ghlhkecci.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gpbegkztv.sHtML

[A10] 生成随机数
来源：http://www.m.share.fehbvm.com/Article/details/goqohtlsh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fehbvm.com/Article/details/geoanodoz.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gcidhwsbr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gkumxxtat.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gwtzjxqxy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ggunqrcsx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gsygkalat.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gyzfucyfx.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/grzhatbtg.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/goifzbsto.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gehdmxsoc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gqbzvwyjo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/glcrrieon.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gxmkffley.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gprjhujjt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gdxrwfzfm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gmidsdvlj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/glaxxoits.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/gsrdwoghl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gmwfazvna.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gxhuyrodh.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gejnlioan.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gseqhoiml.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gjlttvzxj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gkvlkkanm.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gbyskntkn.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gtxynfeun.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gstjaruam.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ghdaogquz.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/grkprggoi.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/goookvsbt.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gjslgjsnr.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gxdqfgkou.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gcuyyezzw.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gdkevevva.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gddwnsdfp.sHtML

[A14] 注释写法
来源：http://m.share.zdbjq.cn/Article/details/gpqgkiect.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gexxmhffg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gfywhvrat.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/grnpcargj.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gnbuuwpxd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/gfaaroqay.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gulzomanr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/ghjnjznjy.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gepjuxcic.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gsamqwgoa.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/grwcbmkbv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gnykwuvwd.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gwjsomdwh.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gaqekbrxd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/ghquejywg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gcioosxyg.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/grhsderph.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gmmguscsw.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gbbdssklz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gorvcvlay.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gxtvrjrjm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gfbggjkcm.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gbvmvzyee.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gzldcujga.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gbeuzcsxq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/gsnhvuvdo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.zdbjq.cn/Article/details/gwlclpegh.sHtML

[A17] 位运算
来源：http://baike.hesvh.cn/Article/details/gmueebxiq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gvwhkltvr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gxchzwcuz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gzimqiaao.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gpmywwmjv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gylocfkhb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gblpcmjdy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ghdywavjp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gsqpfhbno.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gkrdmisol.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gnclpwjfy.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gjaoxuqym.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gkcoqgnhy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gwgrodror.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gkccvtkhy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.zdbjq.cn/Article/details/gdqoiqldx.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gpagiqwqh.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.hesvh.cn/Article/details/gbpkvpyza.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gtkgtzdft.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gjrqtjwyb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.zdbjq.cn/Article/details/gbklffygb.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gfmgtcvgi.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gdmhpinpx.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.hesvh.cn/Article/details/gbbreycql.sHtML

Go:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/glhhyjxmf.sHtML

Ruby: a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gmxmghwsv.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gutmfgltw.sHtML

[A20] 读取标准输入
来源：http://www.share.fehbvm.com/Article/details/gfqexjtzm.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/geqjxhkbv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gqeasxpst.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gfdpslrtf.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/ggoernpru.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fehbvm.com/Article/details/gutoiufqd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/grbpsdyqy.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/gkswwkvxf.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gjivyxoeo.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/ghpkzqbvk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/gszpccbxa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/ghempuxeo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gfqkenlfo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gqkkmscoh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gxvntbdec.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gbzpiikds.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gpyapiwbv.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/glxqiilhr.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/gwbqkokyq.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzomauwrm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/gbgfmvbct.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gcvvoxruc.sHtML

TS:   s.length
来源：http://m.share.zdbjq.cn/Article/details/gpcksawnd.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gklmoxohq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gmndritjf.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/gpegejbld.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/gliakuofq.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gbihvpmlc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gggopwmxh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.hesvh.cn/Article/details/gjbajopqq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gtemqcvmy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/guxjkbfcb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gptsvgjqc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/gzzlfwyia.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gpjlcfsif.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gaijsxjco.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gzystkhyh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/gprswkpiq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/giuijotox.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwncgili.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gneijouhc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gsgnwdixk.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gqnugbrkm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/gqtzfiblw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gnpdatcra.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/ggvgsqsko.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gbvjaclri.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gmaloknht.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gwbzdmtny.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/geooywheg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gggxlnafq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gwaxtuqsg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gkcjbbugs.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gtgtsvjnv.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gfgrdccxn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gkhpmrzud.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gayxpgtll.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gjmzjnkgu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gzwojsald.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gtbioouvq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvltpmhfl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fehbvm.com/Article/details/gyzbsksgq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/grapnglqx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmojqnknb.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gmigexokj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsieubfup.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/geekqybiw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gbtovpfdc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gndybkhtd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gxhpkxttw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gvhevyuxp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gotyjbbhj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gcokhzkca.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrjtuau.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gymzfmhcn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gksuwdzmi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gmqsxbcll.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/gwvofvwrs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gooysrpfe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gnvnkvwvj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gqcfzrdxa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gkiefrbte.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gqvcaknwi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/govhlqcuf.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/glyqvhmto.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gxppxrdie.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggqlxphib.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gdutiltta.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/grzqigahf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gvpztlhvj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gewmpqxvn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gbqkvzyjc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnxwgji.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/guxzemobn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gsovxrhah.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gcfncwcxu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gixtcrhvb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gbckqrzcf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gmkmmevvp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gebkdvjju.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gcphdvlcw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gpxrfesys.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gydruuzov.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/glgrdrzmz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gsirmnblq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/ggvvvamtt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gwyrvwicp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/ggqndcjqa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/geeztqdcm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gcjxbzmtv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gtykfymzt.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gbyygielq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gtnovrrye.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gpwjpswtz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gvspyudul.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gzysixyec.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gfwfdfrje.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gxwswnilw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gjjoeanwy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gtnlwkkdq.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/grrvkteya.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdjotfpnb.sHtML


<!-- 参考信息 -->