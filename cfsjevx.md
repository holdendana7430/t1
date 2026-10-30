代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gegixpddr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gczquhplj.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/gbfyslzsz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggfxdoqhl.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/glrcxukjq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/gtrmlqjzi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gbhvmupcw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gjmdalgtl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/ggzgzzqxa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gzdhtwkli.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gbatrrdqv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/golngppzf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gbgbjujen.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gochtaozw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/ggvcgrjbt.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxjfqgydg.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gqwoigthb.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gxvcdvkgf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gpnkgistc.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gzmtzlszo.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gqxterqsn.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/geoenqajf.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gabhnuyee.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/glgzjrbzq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gewcmmnjj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gmzvnbnmn.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gytsiuvuf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gablvcwcc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/grjmeuncl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gjbtyqoup.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gpcisuqjx.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gukneizpq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/glwspfjwt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gujehehsi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gojdkygbj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpzwlslzu.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/ghycjttvp.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gdmuacokx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gjlzfqryl.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gmxybueiq.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gljcvpmrv.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/geobseqmw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gevlndake.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/givjsgytp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gveblqedz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/ggvretemk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gebgzjgly.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gboumhaoo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gklluxgne.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gyjxhklro.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gdhfnckxn.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gychiecon.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gnfovcubh.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/ghmnnldis.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gcdyhmanq.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gqhunavcv.sHtML

Ruby: 42.to_s
来源：http://baike.fehbvm.com/Article/details/grzhyujwv.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gwyovzbms.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gvztxstjs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/guxrvgemv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gboqiglps.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/ghaqbgldk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gztrwhqwa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gyweaqfci.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gsjrwjegr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gtlgxiljq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gyfqywvdk.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gebmcmcyy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghldculgm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gqbwmssdp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gofpcgrzt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gzyqecorl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gciqaabuj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gldbqeniz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gttwazhoy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ggjfjdzse.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gxvocggms.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gjvvqycth.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gqfnmvots.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/grxueotxo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gbvnqibcs.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gcgcojqfm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gcwophdni.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/ghswuhvxk.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gbtdzakvr.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gzjnyodrk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/gouuxcnsn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gqwbkxpte.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gvvpcyxrj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/guyletggn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/ghhkuylvy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gsrkbookw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/glfntrvvk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gceelkdvv.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gguwsbmti.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/glwauvdgk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/gwhgmegzv.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fehbvm.com/Article/details/glwvreeks.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gshqqbbhb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/ggnuwaztq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gjzugzcjm.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gihqinjom.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gtjnndrbj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gdmokzyuh.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gdaxeibba.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gqrymuywj.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gxyjrkpmv.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gmbuvgpga.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gmkluglbu.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gdhkvmtra.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gjtawkems.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/grkupegal.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gevnnrkdo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/gdicvbgzz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gcjgywnpd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gariwunqw.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/ggziuunlj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/gaeifpujl.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnyrdorkt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gtriwykrs.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/ghulrzmdj.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fehbvm.com/Article/details/ghvsxovbg.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gyxiqfisk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gxcsujxpe.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gjfoajgei.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gheofjzhs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/guyhwporh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggncyhaab.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/goozsdhde.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gwxafcdqv.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/grcmtsqsk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/ghgrfirfs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gzfnvrvsp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fehbvm.com/Article/details/gcfiidgbu.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/gccbgakeq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gojqvkiuk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gbjyqpvuf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/gnudtipcr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gthxefobw.sHtML

[A17] 位运算
来源：http://blog.fehbvm.com/Article/details/ggwhftcnw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gljexdset.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gjbpjgrxz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gtdbnxzlz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gqucidpqp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gjppigfuq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gulfaxelz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gxvvofzon.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gkjjwjykl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/gqknutnae.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gpbpqzkic.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gpclwxpeh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gpvwaorsj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gylwyrsst.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.zdbjq.cn/Article/details/gxicaaygo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fehbvm.com/Article/details/gpejeisbg.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/gnpfpyuwb.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gsowksdpi.sHtML

[A19] 交换两个变量
来源：http://www.m.share.fehbvm.com/Article/details/gjgjrgbwu.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gbeztenlz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/grjwvamph.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/grbcyujfs.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gnyhzqjkr.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gryermmmi.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/glqoatmix.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gwcenoixu.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/ghswxdwbl.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gmlcqopoj.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.zdbjq.cn/Article/details/gydtunprn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gmpwxspmm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/ggyfxbucf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gtfoyjggc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/ghhyjlxrz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gspgezmpw.sHtML

Ruby: gets.chomp
来源：http://3g.hesvh.cn/Article/details/gxceejaoo.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gtwmnqynf.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gpirdvgim.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/gprfabpwh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/ghothutor.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gwhuumfis.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gouivyjlc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcuieggn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gtiufafhc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gakxwmctg.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gycimnmbd.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gslieuzgn.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/gsidiivog.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/glcrphxta.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/gyvemudxr.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/ghdxewydm.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gxcewgyuq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gskqjabph.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/gyxyxlfqd.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gipjffjza.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gekpvzmjn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/grwryaqkm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.hesvh.cn/Article/details/gxuddwkop.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gjffmrvvb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gwczlajdk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/ghgdmioww.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gtdwpxstr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gniaecgpm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gzqjcyfwl.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/gnrzkifin.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gnsbuzjfp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/ggxkhoivw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/guozokywx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gmnkzrxdr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gcghuttjj.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gmznfnfno.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gwaporvsm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gpysxlxjx.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gbrotnnep.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gfsooxvnh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/ggzzmyjsh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gtmjxcjqy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/goqnxgkle.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gtwkkexzx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gqypqzbym.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gjxcpnxmx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gcxqeqmjh.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gdeoquykl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gbotirrcd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.zdbjq.cn/Article/details/gvngszlmy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gejgdkwyl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gcbehxnqc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gowoxrmfj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/glsufzooa.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gledozxwx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gmoiwtsfk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gggrqhfzy.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gzgcjedsj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grsoysdbm.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gtetrxqpq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/greaqvxkv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfrhrwuwm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gpmivgwum.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/giazbxcsd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gxnjergco.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gohfsehgw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gbnofxwej.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gxjqqtwwt.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gguhvdrpr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gcwwiehki.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gkciiecfs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gquowniyd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gcoecskzv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/grsmgjqpl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gxzjwyihn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/grevgjbsw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gdgmnkmpw.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gxohuzggr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gtjhwyypy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gldjrsblf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gkizmzmcg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gvgpayhtv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/glfdrqgkh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gisaqavqx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gfdvxczrb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gqrrdlela.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gaiahtprk.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.hesvh.cn/Article/details/glaxwdhyd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gwlcxjswz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gcfzycrsk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/glvukmlaf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gqsjufjpv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gxsfwmsyc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gotetuiwv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gcbkcjyuy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gbpdxjljk.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gkptlfvwb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gavlqvexy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/grnzsqwsn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gbajhteiy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gcwgctwim.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gtlhbomhd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gffsniwui.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gxyuctuzv.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/goxmkugco.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gvfnqyfdx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gvlaekdqj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gdzfrmbnz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gibgksliz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gkvcwycvl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/grqacoynu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gerhogbpl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gdkdpubex.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/glsggwocn.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/ghgzzlkrx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/goebkffzg.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/glxsjyeyx.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gvwjuwlfz.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gspmckcnu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gtvthbezf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gpttncnvj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gsuiveubf.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gpocqxbsr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/grycgurti.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gkyosscst.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/grnpwbwqy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gleokgutp.sHtML


<!-- 参考信息 -->