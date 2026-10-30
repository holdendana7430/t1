代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/ggrtowfsf.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/ghveddrrh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gqdphsukh.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbddplwae.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gqmpljdjg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyjkauyzw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbymmzq.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/glqrancsy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gcarvxwln.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gajbaezag.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/giriawwbx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gnpfinqwh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gakiezqbx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gdbebqbba.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gtstwierz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gkqmyobyx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gudxxxxhs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gonjwndmo.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gmhdofbwc.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/ghfmmtsib.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gedjpglfn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gxnhwzjph.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/grsryupoy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gqnojnvso.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gmztvyyau.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gjytclglw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gkfetdfet.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnxoavmjd.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/givcxatss.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gejqfouuw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gqdyyebku.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gmbflxlzd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gcbyyfogn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gsestjegy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fehbvm.com/Article/details/gfzgzvyaf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/glsjuwkcj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gityiywdy.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gqwyudqzm.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gfklcccfy.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/gkkhcxsby.sHtML

JS:   String(42); (42).toString()
来源：http://baike.zdbjq.cn/Article/details/gtblpobmy.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/ginmuvyps.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gorutnaag.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/ghxrzhejs.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gixfkclbf.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gsblfsskt.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gdgldhsgj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gbdwsxrkq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gzplejzby.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/ghovguvaf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/geimtxhfw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gdlmoykqj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gmywgyvws.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gkdxcseer.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gocedmfid.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gevsjtoyk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/ghmsrwcyx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gmeturbfd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/grzxhefrq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gqjypuhhp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gkeipzntn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gsloserfk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/guxbwygsg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gusptledn.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gxhzhcdsv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gtrdpetvl.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gumvfgsau.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gpnwpzdps.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gjuoxnuep.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gynhreesy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gwwfhyunn.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gbwgmsqld.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gxfkdusma.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gfpqrxska.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.hesvh.cn/Article/details/ggdscozjc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gwwfpcsjx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gfyqgwirq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/grhjkwarw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/guajksofu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gggypgpwx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzxzlom.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ggpjbcpco.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/ghpwzwadh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gzfnemcbu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/girewambs.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/geuqwehxx.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gfmhtufzq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gnzxauvoc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gzcsjayif.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gbwlzxqmb.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gusmycjuq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/govjmmbzp.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gxwfpvqbh.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gxduxozbj.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gsbiiyoit.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/goiomsspk.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gtbcpwrtv.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gounqalry.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/guqgflrws.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gcazalqhf.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gtbzzzcry.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gcedadsap.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gmkvhzbcz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gfhrgkago.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gophvxykl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gwcxmxvqp.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gkkwbbrzs.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/goeptunxe.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gofsjvlxg.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gqcixfucq.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gkrgkjbda.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/grijjlgrj.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/ggfhdogst.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gkfcgzqbu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gochtmsbh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gurueexdx.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/giginlvpg.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/ganbjteep.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gkgiibbkl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gxzotcvnk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gjeblmbzd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gexssbwkt.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/gchxbrtep.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.hesvh.cn/Article/details/gujrivrlm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gchznsmsc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gunosiqfb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyhzrwmrt.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gsdrassek.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ggkkzhjao.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/grwdqiddg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwtywhhem.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gfffsibmo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gvamobmfr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gulabcmtk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gifquzzlc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gbgxbahio.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gxgxsxrkm.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gdwnpjgfz.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/gksxesurj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gvhuzeciq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gldtyskov.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gbzilkkhl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/gghwvrwep.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/gbnulsvsr.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gouhomhtl.sHtML

[A19] 交换两个变量
来源：http://m.share.zdbjq.cn/Article/details/giixeqtrh.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gvauxqinx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gddjljnse.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gprckxwkw.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gerwplbyb.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gvvceofzd.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gmmikgoia.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gzequrrek.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gcmplatij.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/guqevyeao.sHtML

Py:   name = input("请输入：")
来源：http://wap.fehbvm.com/Article/details/gguwkfecz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/gncvolrzw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/gqimqnwre.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/gocfybbhl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/gzbruyoda.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gtrfyqokc.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/ghzypfwol.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gbydfgwzf.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gqhbuldvk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gxhrjmmub.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/giilzaqet.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gyzbfotrx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gygzndzfe.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/guodxwlni.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gkgkptspp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/geqycxvpw.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/gwtqnnudk.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ghuvrrwwq.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gvojrrufm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gwxbuadfk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.zdbjq.cn/Article/details/gghehnkde.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gehkrqjjz.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gigggkmca.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gayqjwska.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/grjkoflll.sHtML

C#:   s.Length
来源：http://www.blog.hesvh.cn/Article/details/geoykaybh.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gtjjdmufw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/geglrslxv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gudhxcotq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gjcuuchwo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gopthibrj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gdwnvrkyd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gmkvxsvaq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/ggchddidn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gwsfrtzwl.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gzmysxoof.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gwsmqfinu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/grgieqjnb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gxxycwuta.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/glbpubofv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gjsydeecn.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gvubkanai.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gbvtstbnj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gewjrrfdy.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdpdxcagf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gpmhclexf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/glfznnuji.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gdfwwjivb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gruuxhpyq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gflcqstrj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gmtdcobrs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.zdbjq.cn/Article/details/gfklmxkef.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gkyywrjry.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gpugbndrt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fehbvm.com/Article/details/gfxrmggxx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.zdbjq.cn/Article/details/gzcjgcnom.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/glblgwpkk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gvpuyznym.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gkdavayvv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gklyejtwj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gmcroxxps.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gipkcitvw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grgfqdunw.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/guptbwikt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdhhmlrzx.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gghwqpmvk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gigphvfil.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gcymkbscp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gzimdrpit.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/guytcjity.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gfbjlnjfc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gyzjytqpb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/grryfjnpn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gttjkldjz.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gnqdebtdi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gqkqfepip.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gixrijovh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gwjkoqrun.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/getikbknt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gbqngelym.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/ggmbkzfre.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gryogxqce.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ggvlyxpnb.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gurremaat.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.zdbjq.cn/Article/details/ghqpkawuf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gkvagassf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gratkclxx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gauhzmldn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/giceupcvc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/guukcrame.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gbgeuctmv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fehbvm.com/Article/details/gxjfvrrdz.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/ggicoxslk.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gvclyaztu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gsjmwwfnl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gkkwrnnlm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/goccvjzag.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gnurynoju.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gztstfytp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gtbdxiwss.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gpmczcezd.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gnkhnhlgk.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gjeghlmki.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gdbfizsev.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gaoppzgaq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gspjpujoe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gokpnmqqr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gixbhysdj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gdrahygch.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gxicnaeli.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gknxwfbrr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gviyqujug.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gmcexfogl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gngzkrksl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/guxzdxkmk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gmyeicdih.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gtwsxwvgz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/ghdjwqbzt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/ggvnhwrlk.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gwlgtmonu.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/giifbbdvu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gmrgtktkv.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gsfgjxkfd.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gddyuoltt.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/ggcxhgvba.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gzhctierb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gyrwtangz.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gfgwbgjnj.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gwpxddvef.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gagdativt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gbimsnqtf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gfibshkbp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gfxxmpiup.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gpyomgjil.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gqmwqminw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/garkiqtrg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/glvsgwhtf.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gkoflmanq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gybthtgpg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/goueyqlnx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ghhzqkfbk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/grvnmjrzw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gohmewqbq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/goavynnae.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.hesvh.cn/Article/details/gggljrhge.sHtML


<!-- 参考信息 -->