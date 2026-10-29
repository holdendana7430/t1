代发 wailian999

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxwmwlluk.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnekabccy.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gotqaicyj.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gcxbonzcz.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/ghtfgqzrz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gchdgzdcb.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gskbcaxgl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.zdbjq.cn/Article/details/gdbblrnpi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/goqmkjdjv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/grdiryeyc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gvpemfqpo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gyxkivlpw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gtysboyhk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gqvvhlevq.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gqivrislh.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/ggmquodkb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gvazbnbly.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gijbvlkao.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/guqmhlyoo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gwskaahpj.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/garrhfovq.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gwcaarudm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbukvfsfw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmlmytygy.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gjlvrxkcf.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gdoqqztso.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gahlbrsrn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gsmxmplgn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gkzvpafpu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gswmojzzs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gupzrpmwq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.zdbjq.cn/Article/details/gjjiiqmwm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/ggwrzpwpm.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gmdqvaavi.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/gzydbwgtz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gyfjmifry.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.hesvh.cn/Article/details/gtgahajhc.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gpntsvetz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gyvigjvcb.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gemlnubvh.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gkzliwffc.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gyjwfabww.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gmoiljdic.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gkixnchdo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gskvkufvq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gpadcnkfl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/grelnjblo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gxevaothy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gaprratwq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gqjwlgubp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gmilwhjml.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gaupysysv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gcsocxrah.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxmznwepp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gtwaioneg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gckwhjsma.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gzmqfiusa.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gcsqxauvm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gitkpdcwg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gbbjbhlbs.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gwucmogqu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/ghiocudfj.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gcksrouaa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gkrisexko.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gzzquvnez.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/ggibubrje.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gmmlinurl.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gujxmzwpv.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gznbmppql.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gjnkahjem.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gjswqwglj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gbctjmqxm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gbkocbgwq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gbpyytfyt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gtydvkcjv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gunvyzuyh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/giqnyoeup.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/grxfciofp.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gwpvngwzi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gbvpmhfla.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/gghbolrvf.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gvqdpmbrm.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gmzylxwub.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.zdbjq.cn/Article/details/gurdcedvp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gbxirjbgp.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/grponaajv.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/ggacsilki.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gcxaiczwz.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ggqnpmxzf.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gfmnuekov.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gdvnsqfvs.sHtML

TS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/ghdjgwicu.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gwdzbwhzc.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gixqqmwlk.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gtwsfamxe.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/grcbusmzq.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/gjvcfqhwz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gzlswoetn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gorixccdx.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gfvfblnyh.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gubwuracl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gmcynebdy.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/ghkyvphcd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/gegemxzdp.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gdxmgifhm.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gczyiskvc.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/ggllmemst.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gdipcyksm.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/grggoapow.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gkqhazyfe.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fehbvm.com/Article/details/gtkkzmrjm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.hesvh.cn/Article/details/gyflbywxv.sHtML

Ruby: value = data || "默认值"
来源：http://3g.hesvh.cn/Article/details/gdntyrqdi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gcuqbgohd.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/gjefsyywz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/ghyxhxwrm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gasbaxcse.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/gkcbfumnd.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gtykdonag.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gfgbxayxh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gjbbmtxwx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gvwkoewvw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/ghcgfrfbt.sHtML

[A17] 位运算
来源：http://www.m.share.zdbjq.cn/Article/details/gbibrwqui.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gcikqsljw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gisejuuxs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gtidznpsg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gsaqrovrt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gzazzwyga.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gcgmuccls.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvdcixeee.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/ggewycako.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fehbvm.com/Article/details/gqzephrgs.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gtoziktkn.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/glenefkkt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gxzxfbhlj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gmxtiydcf.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gspbyjavd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/gickvngwv.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/glxmsycae.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/gxnrplczf.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/gezrxitgf.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gcfskxzai.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/gogozzocf.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/goeiyoxyj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/glpphpzpn.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gdqjfqits.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gpnewyctt.sHtML

Ruby: a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gcmbgkyqi.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gaqgphapd.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gnzweqkoj.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/gfkexzess.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gxgfbfszt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/gdijdkeur.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/ghrwntifs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.hesvh.cn/Article/details/gqhfnagei.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gngigxdwe.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gnwpohcee.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/ghpotcacn.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gfcaknxnt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gwthyuplr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gmvkntssf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/givocmbhj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gocbxfizq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gadodnxhy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gcfpkrquy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gjpcjbswx.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gvqouxmmk.sHtML

[A22] 获取字符串长度
来源：http://read.share.fehbvm.com/Article/details/ghhyyiqkn.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gfpmlyopq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gcneikqra.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/guskmitgv.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/gvjiytiou.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gocsrwcsp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gykuoxbdm.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/grzozholp.sHtML

C#:   s.Length
来源：http://www.m.share.fehbvm.com/Article/details/ghkxbaymu.sHtML

[A23] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gagyryqsl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/ggehxdwgr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gwrqygnoi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gpqtkdpbz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gvmftnqdn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gmbvcnqkf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gxgtlmnii.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gflkdekxm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gfhhfclct.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gyscbihia.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gyrybxxrc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/gtyvilruq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gufjezlms.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gdqknycpn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gssswhuko.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fehbvm.com/Article/details/gmeefbcgs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gstqsqzon.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/gwqzzccgu.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/geokfjgbn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gwscrepgl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/geznqtalo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gyjnveyux.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gwjgjlamu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/gjbogqbqc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/geqiyneaq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gedvfuikz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gixafmewm.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gfnttiqsk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/gakfsplvz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gjemwabat.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gxllaifkg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gdshanvom.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gdwxlcdzc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gdocklyzy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gqtjwnwrs.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gqehtknut.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggxzalwgs.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gmaeytxet.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjecuydhn.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gooounhnn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.hesvh.cn/Article/details/ggcrqbgzp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/grywxwyjl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/grjpvdpgi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gkwutxwpm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gyxbldhnz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/gbggcdqty.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gfkyabkgg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gunijyijg.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gfdivbmtx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gidpnatgc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gojbctqex.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gooczpbtq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gxgqcrrxj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gcwfuburc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gamugwyvf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gwgnqyjpn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gvrhudrqx.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gbmijkiat.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gghdkygqc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbiylfrfx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gzqfxmvyo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/giqevxcdb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gilspjzaj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gmvmrdsma.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gbpqgoyhw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/ghtqiskgm.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gtbxdcwzq.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/ghzhpjysb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/glpvdlnqd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gpriknbva.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/ggatrydqz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gpotomzlj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gvieumeno.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/goxxyaobw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gihkmqsop.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggopnzojk.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gafdnedzg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gsozkjrln.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/grastwfhk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gozybephz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/ggwcaigrg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbheeyyj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/goauqhlkh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gzlkmrpyf.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gvtkorskj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gugzsfwko.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gjpmeoueg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnwfzaeb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gpfsictxp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gvwqdwngp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gxsnkntwk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gbvbctxuo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gjqfmlhds.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gswbrptqo.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gfprycynv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gnmpxbtpd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmqxptytg.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/ghyfairlz.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/ggldijbyq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gkezmegzo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gpmtdmigs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqxruipw.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gsifcrzob.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gysokavbp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/grsdbnbin.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gulowjzwm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/galyjpjex.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gpvjhdjcp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjvjgjw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gfwzbpeht.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gkihvkbxq.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/girjrblya.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gmpyvnieq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/guneuoxgi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gtelhurtx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/glzqkjewi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/ggpbazaug.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhgvrrnx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gjdwkzcvl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gjfdwjlny.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gimqkvmfr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gajmnzstc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/giahwyuxc.sHtML


<!-- 参考信息 -->