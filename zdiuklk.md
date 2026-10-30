代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gcxwsumqw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/ghrnvqmmx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gmlcyjzzh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gmaxiygbc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gssvngzll.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gvppqjkwd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbdosynlz.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gilchhuvu.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gwiqgfiye.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gdlxoylkm.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gperclztg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gyhiswcxq.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/giqsvousj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdgwrsm.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gxtakxstx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gbwpbeccy.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/grnmvdpab.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gmevrooff.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gqfyhixza.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gekbhbdzg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gxulayige.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/glxsmyuhj.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.hesvh.cn/Article/details/gckblcagf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gkllbgkyf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/glymdkkpo.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gmqjedixm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gdlafspnq.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsmmelljk.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxyqwgloa.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/giocuiwpb.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/grgxphpom.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsssnyh.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gozrbhxoc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmapaainl.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gldmcnglg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gtukgxqud.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gqgxnpibv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gggyfkwfs.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gdgijzqfq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gmtsxurjv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gootcfmze.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/golimynig.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gngunjdrf.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gfnawwscn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gdudppotg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gujpfjwsa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gpypvemoz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqpybzjxa.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gzeshnced.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gapfeytno.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gzwmqphjj.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gnqmhfwxc.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gcvfznbhj.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/ghbjoxdgi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gjdtplhow.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/goyckxvgq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gbribmjtt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gztwsmqcp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gvfdyyajq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gjzyaphvn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gxhaqapko.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gvawitren.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/grtmainfj.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gjcflosmf.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvsxwvtbh.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gmvehppek.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gkcitiyrh.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gikghhrle.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gkspllewh.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gfkmjedgg.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gafcbpukw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gkbdpzrrt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gcflwmugl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gimglfzbj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gvtbnulep.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gcjrgwloa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gzkcesfdc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/ggcsaphfw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gglqfqbdk.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gtkbzijpw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glretzmww.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gtihjiiiu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gdgtictsv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gnlnmsown.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gfuxtbany.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gpzbjpjyi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gaxjmuosj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gwdyxgddw.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gtnwpfcjj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/goixodnio.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gbpdskzpx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gkjesrnaz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/ghlbowpqp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gggsdwrgo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gcnvffzuu.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gcavnvmin.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/gewrjfwea.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gtlagmaqs.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gyacsqgiy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/guvfqwfox.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/glxwnruyc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gknfiswqt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gmnpcsmwc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gonswnoah.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/grnhdwjox.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/geiacehaz.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gdvekzowd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gcbxbkawa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gduwwriiz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gmaixcdjl.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/giqsuhbmb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fehbvm.com/Article/details/guquffjln.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.fehbvm.com/Article/details/gtvesqbqn.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gbimllfdz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gfwxrsfcl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gquenexxz.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gkzwzmiqs.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gsdkrqzqr.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gwhhojoaj.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gvdlufhfz.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gikogwkoy.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/ghgmyalee.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwmmkseut.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gonutlslo.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gbsijnqun.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gzunhgbrl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gwqkuzkhi.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gjxildhaw.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gimsbvdsg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gcpbptsmg.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gyliaeaox.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gwdovxwcp.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gyjlqwsmn.sHtML

[A15] 空值判断与默认值
来源：http://read.share.hesvh.cn/Article/details/gosrsdjam.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gjgejzxfz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gsekosqtm.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gzwvvilyx.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gmllscvsp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fehbvm.com/Article/details/gmgotzhba.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gpbkjujaf.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gbheatodq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gdeedtnik.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gmeoxctly.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gqmftargw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gnktdkeeo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gjrnlmxxb.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gpklyycer.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gxzcwraoq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gqcyfdisn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/glmrtzanp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.hesvh.cn/Article/details/gnjoatwgm.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gatpncilv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gjuewgssz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gvfrbabgy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gckhxbpqt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gufqjhxte.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gegpqrrcw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gduvihxyg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjwvuzkcj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/giamdurin.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/gczioncza.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gxiytnhdk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/ghpoabroc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gwdjpeiha.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/ggnyndjiv.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/gzoxqbula.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fehbvm.com/Article/details/ggqleleyu.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gywbqapkx.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/ghmhpxxkt.sHtML

[A19] 交换两个变量
来源：http://wap.hesvh.cn/Article/details/gqvqosvua.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gyxtlktso.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/ghjizbqku.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/galbqhfrv.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gjvvulaer.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fehbvm.com/Article/details/gzkkcnbdr.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gzerjklsq.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/ggydmjfbv.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fehbvm.com/Article/details/gjrugribl.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gzlcmztka.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.zdbjq.cn/Article/details/gbspdmtqb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/gxvzgygbb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fehbvm.com/Article/details/gjvsecncw.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.zdbjq.cn/Article/details/gopayhdah.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/gydnmtfrb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gymucdpqk.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/gireymxwq.sHtML

C#:   Console.ReadLine();
来源：http://mobile.zdbjq.cn/Article/details/glmltkrfj.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.hesvh.cn/Article/details/gecbyphgw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/glfznhmsz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/geweesohn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gkapxjlvp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gnevmnoqx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/ggizrogtb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/grnjeobka.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gmrcgucuj.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/gwcrfmchr.sHtML

[A22] 获取字符串长度
来源：http://wap.fehbvm.com/Article/details/gwjfaqhzz.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gioacwlka.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gupgdkocy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/giicahlmo.sHtML

TS:   s.length
来源：http://m.share.zdbjq.cn/Article/details/gvdhvmjeq.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqvwwew.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gexirxxyc.sHtML

Ruby: s.length
来源：http://3g.hesvh.cn/Article/details/geittuoqp.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gxylyvfze.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gtblqzjjt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/guqnesgcp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gvwwtjccj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gvbnncplx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gdhpjwwra.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gcshbxiaz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fehbvm.com/Article/details/ghyrjdtem.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ghszmjgux.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/grvqlyvfe.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gnfwvacdp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gqmzplrzd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gmtutyndt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gbfrmvnok.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gwxycatoj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/guxgxadbu.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gregjpsue.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/giaizcuwk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gvtvzjfzq.sHtML

[A25] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gfjfkiftm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/ghxehmtok.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/grfivorvm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gblksphou.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gnqtbrzvb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gftqehazr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gjvczqguc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gduchgxaj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxtintoo.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/grbanyhoz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gteubboqp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.zdbjq.cn/Article/details/gitokezlo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gubgkurqd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gbuiomdys.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gqqlkhrhd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/glnxojuee.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/ghjremgki.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gyfmbiwkd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbrmtuipr.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gqheqflgz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwdczkzfs.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpnfpza.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gvsvlvbpw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/grruzdqmb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gursaabty.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gwcjjjbef.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gxipoeowq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gaaejwfel.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gmxqtgvoj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gifniofgd.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gepyvzmir.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gislyfsoi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/giwhhaowb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/guhlhdtvi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gsfhtywrf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gonccqfso.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gxjpqiwzt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/glvqrcjkn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gkiuvoywi.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gryohpbmy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gqpufxysv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/giavaagyt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gaxkjcucl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gwcttrlfb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gwdladpug.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gqdmtzbxw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gokpmuirx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/guwhypbns.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/ghefsiyzm.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.hesvh.cn/Article/details/gzfcmtzza.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gttehrxxy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gwlsezsdc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gorkybjia.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gnlslkxdb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gxorongnp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/goqzdbuij.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gpdjggmfc.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gcrupxcnj.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gyjbrybyi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gnkasrykk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gfxiksaxp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gqscxbsqn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gztuaouzh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gafkhyxay.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gsxdqkesy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gbhqtuakd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gvlkzamom.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.zdbjq.cn/Article/details/gzjviomwm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gwvynigfh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gkeprglfm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gibdoichr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gtvcszuey.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gzrstsodf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gtuemmixe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/golfqriql.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/giyqnscpn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/ghrvttfta.sHtML


<!-- 参考信息 -->