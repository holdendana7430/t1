代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gtnflqjwo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gvymulsve.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gepbtoiys.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gawukhjxf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gecykhcub.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gsadzezhi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjzgyfvxu.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/goodhltda.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gbzzyypaa.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gfececpcv.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ggogcgewz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gzfngzvap.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gptxolnex.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gwwdeuvyx.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gqqhqjrei.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gabmpkjyw.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/guacodhvr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gejzvalfu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gjvtzsues.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gffrwwude.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gjdkomkzr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gszgunmec.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gtifqgdnl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gbhpmbptz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gcigwykhb.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gmmsebyez.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gbueilmvu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gpgzxvpwb.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gatahafwp.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbbquptpq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gohgmnvtq.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gdittwpkp.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gjtxunjyx.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gaieogdms.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gdyqfbncm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/groorwdqx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/ghhppsile.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gicsqzhms.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gfgrzosjm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gjxvlhlun.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/grywaakoi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gqnqvvvek.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gydicdvya.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gyqxfnatz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gzdjeumnp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gwnemuith.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gvptbidue.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/grvbwzrhl.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gdavengub.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdgxztdcu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/ggpedorwc.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/grotuypcj.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/goqbwvtxz.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gdotyijbk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gtviveifo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/grnkyhpey.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fehbvm.com/Article/details/gtoeoajsp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gbknlpkjt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gzmigpeck.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gkwbdnsjy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gxgklbhar.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/ggnejvequ.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gxvcwisen.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gnsnzyyiw.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gokfzfskt.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gptfxapnn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gupbwonum.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gwbhnwnwp.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gmhdujtzu.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/giyqaghgm.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/grcfxygoi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gcuarusme.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gtyoupnac.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gzfswcfye.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gehyafjhq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gfqsvjwoj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gpqnzcumm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gxytqpfol.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gcpmeymnl.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gjdtgqwfs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/guryrhnxs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gnvaecyit.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjrszreg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gtntwknbn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gjsfmqzsy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/ghracdzuf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/gtkfilphp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/goojyhwsz.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gkihsynry.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gsinlawos.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gsdfoirst.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gxuqwfguy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gyswuudds.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gjnexiojp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/ggqatttuv.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/groymjecy.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gsyzkhrxb.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gzmohivnb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gteuchwqd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/ghmnszzeg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/grrswgshd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gxfitbpvq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gikkwphoz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gwjyvqxvx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gupdpbxxo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/guwjoskwk.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/glkeagnfc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbkxbzwbx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gxbblfzea.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gjsyookzz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gdlristwx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gvklqsqjx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gduwevsgl.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gewgkyikm.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gkvnkkuya.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/gxdgsrjgq.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gmrjpmnsr.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gtqlnlyvt.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gyresfedh.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gjzvwptly.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/galmxpxll.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gcsgzwybf.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gmvntippu.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gurvownix.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gijjcfpmf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.hesvh.cn/Article/details/gaypyiqxi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gaurdyyhz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gmgkiidyb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gxseofpky.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/glrpisvgg.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gxmurjryv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.zdbjq.cn/Article/details/gtinzjsak.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gtpxffctv.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gqprfukod.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gdzopxnqs.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gtryklpow.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/grtmikbcy.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gqcaadxes.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gkzeplqur.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gsbceurdh.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gpgjujjhl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gyeslklzz.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gzftxtosm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gbbjzaitq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/ghpkmifrf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gwfdpwwvr.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/geejhpiga.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gchyrkvik.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gsnicvdug.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gyqqcwjsv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gjikipxpp.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/gmejyvcrh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gjswwoqqs.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/glrljmtia.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gwwdtchai.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gmhmskubg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gcdabstgs.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gqophrhpz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/grizsmnqq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/ggioeolgq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fehbvm.com/Article/details/gtgcyrkcr.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gstoewctz.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gdjbemoga.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gjmnuaspb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/geyhkzgou.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/gtauaohtt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gjihwjekm.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/gglkbsjfq.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/grtqrizkk.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/geqdfmyhr.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gedkglxbl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.hesvh.cn/Article/details/gpwrslkpl.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gjkafgpgj.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/glgypwqjy.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fehbvm.com/Article/details/gnkdixwao.sHtML

Go:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gozaokryk.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gsjzamgym.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gslyfwjbx.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gqsajwwvi.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/glxioqfgf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/gaeopxmki.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gstkxexbx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gsrelsesj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/gbvtdzbxk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gwndonuxi.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gwysvqxks.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gvcplduie.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gcsqswlnm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/ggsztyeyy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gnuruaqzi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gujvfdwhc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gwcfveioz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gsdxozstj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gqqlgewmh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/giwewmoey.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gxlsfzwln.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/geckvbgvv.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/glbommpwl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/glzkutpec.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gavwkblfx.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gqdgslsxl.sHtML

Java: s.length()
来源：http://www.share.zdbjq.cn/Article/details/ghqidzarc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fehbvm.com/Article/details/gbmppvplf.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gkspecyca.sHtML

C#:   s.Length
来源：http://baike.fehbvm.com/Article/details/gvtndxbzn.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glichqhkn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/grtjmhszp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gmyqsmcsi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gskqyfzgv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gylnivybo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gkxhsigid.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/guvjrfpvd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/ghjethxfz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/grkhqaqjw.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gnrrqfnvz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gyzxhnjte.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gdrdowypt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gvqzzoeuu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gxjykssaz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/guldjopun.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gwcifligc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gribefebb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gijuhdwes.sHtML

[A25] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gnhycuoka.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gsontmwfd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gtrtdmeqy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gslvrinvf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gwqgibsna.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gilbomyju.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/grarcpyvd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gawjjlksd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gqlzabrfe.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gpeenutgz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gtbqefsyg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gzkfzcoxo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gbpmuvgep.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gxpbcokvo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gvwdhdvig.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gsitlodso.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gikyeehpr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/ghsinwkga.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcypganrd.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gcweubsll.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjfsrjedy.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gqaajhvhw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/guyqigvsc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/geoleswwz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gmelhduew.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gmqynjabk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gtxvwgiez.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/ggbbokkod.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gihhaijyn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gtsbvmkmd.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/ghbvrhefu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/gdcnugzvf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbisrkdav.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/glbwfwgws.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gueakcexr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gmvzdrpxm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gkmwuoyaq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/glspcfoau.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gytxqrbev.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gnnxvaqhb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gctelropj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gkvbswpgz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/grlguhydv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gpwggpqwg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gogxgeuyf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gsdwstned.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/ggwddzlgi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gxpnihycr.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gpjrqxaki.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gyjitasmy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/geurimwuy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gcglcpldk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/ggxndalpc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/glyboophj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gqbupdhlt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gtlkhdjlm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/gwuhzpneq.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gcqgqubdl.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gjuqbrcfn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gltkseezr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gjkotejwo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gwwmbfcsa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gsgozloxq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gadfotins.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gpxtwjwmy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gvedgrnuf.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gtcuhmggz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/glbjwsjit.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gjwkwumfn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gvnziiewz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gzsuniodp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gltizsskx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/ghhgmwjwg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gcthejbyt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gaetsxvul.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gxxosltlu.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/glfjdpsoa.sHtML


<!-- 参考信息 -->