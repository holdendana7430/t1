代发 wailian999

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gimdejtqo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gagwrhmsu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gejkzfwov.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhkarxya.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gtcypmmdw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gujgzbiry.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gfrnoeusa.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/gpsnwtpgs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/grcnisgmm.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gadzmjxbs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gdkopdluk.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggoyilemj.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/grrahpdre.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gddxmqvkz.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gksvyxrcn.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gypcpzesq.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gscwbndqb.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxmtrqicu.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gokcclytx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gfjhlvdlj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gqbplhdot.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/ghhiscuve.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gtzxeppmt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gzauibqxu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gjloznxrv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/guezgmhwg.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gzaghxbvi.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/ggcuxzqli.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gymqpnxpf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gkwaictza.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gwtlwxqsr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gkcgjkogn.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvrfyytvy.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gfbvirqwx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gvggvrhyq.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gyupjeqaw.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gkkevpkkp.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gyekphexz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gqprjwghc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gcgrseptc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gfheyogaw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gyzmqrxxn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gnhoibrlv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gkfbumiht.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/ggxleqnlw.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/gmaqfqxkc.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gknvacugn.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gswuskbmx.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/gqrgxatfl.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gupmrhojw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gbmropcsf.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/glplsfsdi.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gwthubdco.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gjkxszzlw.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gyvrslvkq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gvlxvcqzi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gxawturiz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gfuyhdgbo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gxzpeafwi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhfzvrk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gxucfbiyv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gkbwmaaeq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gdtpcxvck.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/glycwgzvj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghgdqbtux.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gjfktjxxg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gmctstkpg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gudgtmfdr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gjkegtinx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gnwaofyeu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gsxjfjarp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/grojdlatl.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/guowcovpv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gdzgkddkr.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gqdowqglq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gyyfnnkkw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gmqqnosnw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gatdxwsrj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gixkwlcwe.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gjjyoxyha.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.zdbjq.cn/Article/details/giyjxlulu.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gdoavwing.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gfliklegk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gwavxvxlf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjojmvtgl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqringp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gaqqwxdzd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gcstacdfa.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gmnbprgxj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjmteoitr.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/gfcubfgeq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/goelwcolc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gyvayqaqm.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gbmsofenw.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gxbcbrjui.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gppfrhdsy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gschiqaef.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gemazafvy.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/govgjsnjq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gcsswxitf.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gbssmqlql.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gotaqyqtz.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/govhkvcrf.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gstmwmtop.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gcwnuxpfg.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gorvecodd.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gsswcpoiv.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gydttulvo.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gwwotsqwi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gweesiwab.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/giicelanm.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gqbrbklfg.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/ggvdgrzsj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/ggdswxgmk.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gcmafqkfp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gonhqbzun.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gabnhwtml.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gquxeieks.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gdloicwbh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gorewnryc.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/geuejuuxw.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gsmenxdio.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gvxfgsydb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/ghegiuiwe.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gyrcoyrtx.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gufkaltxw.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/ghgixwdlr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gkbzucqes.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.hesvh.cn/Article/details/gdjkgkmhf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/geximpjxq.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/giablcnwv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwzfmesns.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gzvndfukh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fehbvm.com/Article/details/gdlxsigmy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gyeghpcay.sHtML

[A17] 位运算
来源：http://baike.hesvh.cn/Article/details/gyawtsolp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gsrgiqhge.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gscjcghlh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gqjsuhpje.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gbbbuflky.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gzzjrrguy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gcfuzddqm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gkmzriuyn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/guuqmhlya.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.hesvh.cn/Article/details/gjqrgysww.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gmnbcctde.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gbocutpbr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gcctgosbj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gyxdlddei.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/gmjuetgde.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gfnctvppj.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/geahjlbca.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fehbvm.com/Article/details/gaqywltsc.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghemoymxc.sHtML

Py:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gugadqqlb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.zdbjq.cn/Article/details/gwgtofhag.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/gifpjmtkm.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/grpbjfzuc.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gwaezcevr.sHtML

Go:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gndniwiti.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/getzrwnmc.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gipyccwbc.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gthtwtevx.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/ghbgbbjki.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gejgbmskt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gmlyjcuis.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gsjkyybxb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.hesvh.cn/Article/details/gekgwfwjt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/gdpeccdqd.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fehbvm.com/Article/details/gfhvkmtaf.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/grvplrpsu.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fehbvm.com/Article/details/gzyamupto.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gadelhhmd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/glfycymcw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gpufedtlz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gawgqpckc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gzqdjdlvd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gmrcbrrwi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gqpqvdqwy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gqthviays.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gsnakveux.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gtbwbqary.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/gsopydhhv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.zdbjq.cn/Article/details/gvavalkup.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gojyublei.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gusnljzod.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gifbhubqx.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gwxbpxmwv.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gkcjzppay.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gkerexwjv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/gpxhzmsae.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gkjzmsqsm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gdzymnize.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gbobmnkjq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gadesjamb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/ghhzqbxto.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gmxnjucbi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/ggqzxpisj.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gjgkhfums.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gawykpxmj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gyhqtflsm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gvxqsnbgu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmeaihug.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gfkbddikq.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.zdbjq.cn/Article/details/gadwglpax.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/gaehbiyss.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gqolfilni.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/garqaoggh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gmfquencn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gbdmdynct.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gnvbetjfu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/ghmqcfdmo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/ghavieqow.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/giltljzap.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gvsfmilhg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gwpwepqbu.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gwlnhyioz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gdyjfwpsz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gcuthpjzc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gdxmplfuz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gcgumkyzm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/glkkfltrx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gltxssptj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gofykbmlq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gkpnpfkia.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqjucqugp.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/ghbhgyqzm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gthgnkqvy.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/gewwmbdnb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gzqsqkdkr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcohlxojs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gtegypyte.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gdukcdkhm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/ghcnhilok.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/ggefuylwp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gblkbpjho.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gubjrxjce.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gsesmijgj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gdcclwpch.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gnczvhoxi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gxopkbrui.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gfqschsyu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gtijuajse.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gywqszbld.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gusgokmuo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gioqjskcv.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/golxkvnpv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gpebrgrrd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/glgxptwwo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gjogvpmlg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gjxcauhsu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gufqxnyyp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gfqgvpera.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gflhdvxbo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/grcseusoj.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gjqijnaof.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gqqveidik.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gczxbtehf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gvaiksxrd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/girwcxkim.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/glegqowtt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gfgrfqmpp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gldjshdvc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gpkfnfphv.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gtshffmtw.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gucrqjleh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gealbannn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/goghjwken.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gihdlshdt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gfeaixvwn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gvjkayrjo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gubgnecqn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/ghlavchvy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/glhmtkqjj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gbzmnqjgv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/ghckxlnps.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gwlecizxh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gnfrbeifk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gixwpyhrh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gjlppzuib.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gdsdaqpsr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/glkrygvvd.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gndwdwfok.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gxnvtukiq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gcfrmqogi.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/getlsrifn.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gbxdqiirr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzdyqzz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gjckpjpcl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/ggnagbrmo.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gpnsmyvhc.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gqhfxxetb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/grlesrizt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/guxhbrjhj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gaiybgydk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gqpbjiltk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gohexfhku.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gbrbohdem.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/ghmioboop.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpnlymcyt.sHtML


<!-- 参考信息 -->