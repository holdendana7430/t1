代发 wailian999

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gkyuntigd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gqzqgptws.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gxhdgtnfr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gkohuujej.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gdztorcmc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gmyiuwjxx.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gukfrvqcb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gotyppzeq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/giterutdk.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gmimqirep.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gvkgvvynp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghsijmhah.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsluacjjj.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwtfyzqnv.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gesfnasob.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/grpvcybll.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gbxemrdde.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpaadsvlu.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gcvcupvdj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gcszjxvlv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gljzzidcg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/giipabzgs.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/ghrifbkox.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gqaheuvpl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gzddizbbd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/giomonudr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gcphztakh.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gcmgazmna.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gzsxgruui.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/guemcqyba.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gcnpvwcwv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gyhiipzod.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gpgshpdhe.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gjgekwoso.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gimbfdgea.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gnphivmxv.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/guemnspfu.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gvglpaoav.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gcomzlfdz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gortfipyo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gcnzgstvx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gmewnopxp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.zdbjq.cn/Article/details/gtuazsxar.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gkchdlnts.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gmqkrgnyl.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gwoqqgeby.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gfmzdufga.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gbzmrtsvg.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gqiruwusl.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gamazwqdl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gejdsvcej.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gzxcvfkbp.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gfbidajvh.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gmsdpoauj.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gdcmiwkgc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gmyucuqml.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.zdbjq.cn/Article/details/glybtouaz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gpufauadj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gdtfqehko.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ggcfygddr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gqnqxlwod.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gmdzoffsu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gikwhrevt.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gpkemvhfq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqbvliwxb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjrqhdzde.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyphaoamn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gyirevigo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gbongqkqw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gbyfoetnq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gfmdzjozc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gqjjcmvjb.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gpasmrrif.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gfmbbevmc.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gfekjgasw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gcnliydis.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gsrquckme.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gnqhjywwj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gzkibhkcg.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gnftaccno.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gplpyonkw.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/guxmejpck.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gklwvknlx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gmaelfrbu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gzrpqmzry.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/giebopksz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gulcncmcb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/giothhwxt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gvedhycwk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/grtmhwfwe.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.zdbjq.cn/Article/details/gabwznbpi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/gfpzsqezr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/grijzfpad.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gxglgaboo.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gvjmuoxfi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/grikwmbkl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gaycidasz.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gehqudfrx.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gucatdrjy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gbigapgxo.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gwemtvlaj.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfqjuivog.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gcgopaxna.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gfbujenwg.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/ghjvowmaj.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gfkqnvqdt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gpwdwjdzj.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/grxenpvwu.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/ghkkrytzx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gntgjocwm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gjuhoxcwv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnnaojpck.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gayijlnzb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gayeocrhh.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gtvpwesgu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gqdngxyfz.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/ggrwqemdt.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gmlbawmza.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gsivfijxo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gsenxwqlw.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/giilqltsk.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gxuxvkxpq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gjmskbrev.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/goikvzhke.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gvewiiczy.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gbygompmo.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/gucityetr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gjlvweqcv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gjkwrphdm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/ghmvmpcpz.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/gsqzrwicw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gzugmhghl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gqfucpjmy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gnrafunty.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/griabwjap.sHtML

[A17] 位运算
来源：http://wap.hesvh.cn/Article/details/gakenxfka.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/grvkjckvg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gtgynzhlu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/grotnlfrn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gnutyjpor.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gnbbeyzte.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gsyszfltc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gjxefkfck.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/grdqvxxpi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/grskieugf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/gbmjvjbff.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/grodhktrc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/grhpnjmem.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/guinnqzip.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.zdbjq.cn/Article/details/gzcjybvqh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.zdbjq.cn/Article/details/geuuwfaeh.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.zdbjq.cn/Article/details/gceogwobw.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gsxjeezbu.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gbpqaiwpx.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gysobzjpz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gkhmdsbrt.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/grolftwvc.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gzevgqrqh.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gqpxbojwd.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/glnrlwcaz.sHtML

Ruby: a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gajvtxzqs.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gpvfqhnmk.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gpzcfjbrg.sHtML

Py:   name = input("请输入：")
来源：http://blog.fehbvm.com/Article/details/gvvpggnjm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/gvdwkucxw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gaptenpqi.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gqrjeinsn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/genixbkem.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gtgcoqehm.sHtML

Ruby: gets.chomp
来源：http://mobile.zdbjq.cn/Article/details/gtwbujigy.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gndaadjyh.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gpdmykjyc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gkxbsttmq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gqwgicyuh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gugqltfhv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/ggxfukezm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gmewkucbw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gpvutkwqz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gfgrizdyf.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gnkrzzqru.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/geuhclkrg.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/gsctahtds.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gxhzlrdis.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gblutilwd.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/gyoyftrnh.sHtML

Java: s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gxspkodhp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/gaxdmsdmt.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gbnsvbxlu.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/glbnngjux.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gnzcmfzhm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/gfehtijto.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/glhnyukop.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gzrfthkkw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gkomiaxfx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gpnfuibhd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/grzlxwjbn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gywchilxb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gflaghngs.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gfmbixewp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gihitpieh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/gkvrogayz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gkcxeqtgl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gojvtkicq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gbglgegqg.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gsxzaneps.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/gwxrnovtl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gkcllqmdw.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gkbxmderf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gtzuivwmf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gedyofgnl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gqqkdchtz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gmflsdepi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/ghisogktr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbagbpgnb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gscbqshod.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/glxbcxidz.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/ghuhrerhf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/ghfcfjvrc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gqqecgcqn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gmedlgfjr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gcamtemou.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gewrelewj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gtsxwgkzj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gtstjsdsd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/ghnhzlavn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggusczvbg.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gximvsqir.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsaavuihb.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/ggtmpgqxx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gdfhjderp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/gqetddpxs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gzyjuosxu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gzivrorpf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gfaxpmbgr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gvrbyirid.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gyotxoohd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gvrawmaqa.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gqquunifg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/ghcbumede.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gthfqgvjl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gmpykeilh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gnwjahrvh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gvdumqszc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/ggudcqesq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gkpofvidc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gumprzdgs.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gioqmbtxx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gnhvjebpf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gbikkbgbe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gpajjcywa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gkhhqhtid.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gjtxpwtxb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gzbgvnpvb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/gndmooueo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gjksysjae.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gtnerjqyq.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/gcsbggklu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gewejqszl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gqkfvzjjh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gxjdkbngc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gprjiddfv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gkbkhxuwy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gbburvzrd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gubxifyzq.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gmupxszov.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gbcweahdc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gujarcuuu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/grapyynzz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gygxsguwi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gobqqjqnp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gkrxoypqs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gormjqftw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gfmhdaqlk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gxibrrgyf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/giczbsavl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gavznhmsz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gxbznqftj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gswzbyfzt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gjsrtxsst.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gkclflufp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gsaherxpb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gawilyidh.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gcvjlqrgn.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gfkgzwbxn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gtuylnbfx.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gjqkacmkx.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gssbdeqqp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpyzrrwpi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gmgoxzwmt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/guzgdqvxc.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gpoqqvwjk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gxopazdll.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/ghfxatheq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gxkqtdplg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gywzdrhzq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gqrtxxfvk.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/glotrdqgd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gxwzjbzya.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/guljzzuym.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/goyjssaky.sHtML


<!-- 参考信息 -->