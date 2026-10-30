代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gkmnimclh.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gwvwmgmxe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gtvdqgtfg.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghoahjhkt.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gysgtyugd.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gltneztjo.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbsbdfyfg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gidiwhmnt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gcslhemkj.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gbfrzvcua.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gezjfuuyd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsauewdu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gsqqlhtwo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gikrqqzci.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/girxyvucv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/ggnruewjr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gigplejog.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gqhylzjzw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gccdetcml.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gaxoltjsy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gmnftuyin.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/grvwegxkl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gylqrtowd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gdcaynebo.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gowxxmkzn.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gltufttoh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gewcadnbf.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gctmxtlsv.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gvglvmapv.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gyypqensh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gqkiwgsez.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gmilzevog.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gtksqaeyp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gemmgtmpm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gvjgkxloh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gossqqogp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gksfypqjb.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtrkkwjmh.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/gtbdznone.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/garwdcxbu.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gawrbxfyj.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/gzvscdffi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gwzrmahwq.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/gdsoflicj.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gyxorahel.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gfoquolhk.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gpeebrxhy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gnfaiaagj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gcbonpzds.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gmxollmap.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/geyjmmvss.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gpvqbrmga.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gbtdlqxtw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/geyaxepel.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gfxzpjeot.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gxgwfxank.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gpnezxptx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gzmeckove.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gdbkjmzmz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gimfalkyn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gvgjrhlic.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gkelnfkvq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gfquhgmlo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gphhmxkhg.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gkqcavaar.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gpaeyalxy.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gsekexdhe.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/grqbjvbta.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gmpkuzuqj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gawniolvr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gvfwcllwc.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gcgpmhhkw.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gmaegswwn.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gulaymjmt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gsyweuqti.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gvqasxalp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gvxsvojox.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gkipxxtfs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gvuzgrnwg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/gseyhvsze.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gfpnhxxdw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gkhgjopfy.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/ghuuamgqu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/grrldfxxj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gyfayrrqj.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gcebaaiwm.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gpdmlcgag.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gtdlcczha.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gcudznzfk.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gbcpeaoqz.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gqrpwaxod.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gdppyyant.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gazimfldh.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gydccdftu.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gblvepymw.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gevoicamd.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/grfwgutcl.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gurwdtcyf.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gweswpppm.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gxzspbkxq.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gsxkksrgo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.hesvh.cn/Article/details/gffjxfclo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gcmtovcfn.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ghgrksucn.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gjeyjweol.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gmpjqrxhq.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gwhzxvrba.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/guumoptmp.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gnatucnuv.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gioqwlahe.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gcrdkuslo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gprcpaxbo.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gdiqsjuam.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gmfdsmbks.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gxrnhkihv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/glztelnuv.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/grbhhwbec.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gphvoqnuk.sHtML

[A16] 真假值判断规则
来源：http://baike.fehbvm.com/Article/details/gfihdmncp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gdsfjvibt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gighqxxin.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/guhczxdly.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/ggpowzppr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gllptpmpx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/ggmbcxorz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/gvvasjgjk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gnbysniks.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gmvfhqnes.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/grwiilpae.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gfkepyuyd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ghnarznux.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gxukcfdme.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gvzvrrjrc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkamowdus.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gvtrixclm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gqcfrnkae.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gpmskscqa.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/galnbidjy.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gbdqqzwjf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gvoirjleq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gjksufhyx.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.zdbjq.cn/Article/details/gdlyvwzkc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/gwgqzlssd.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.zdbjq.cn/Article/details/gahhsgcfe.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/gvcdsjhab.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gozdrwnnm.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/giqstvsdt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.zdbjq.cn/Article/details/gqzjksotw.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gpsijoxux.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gorpzzxbo.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gocorouab.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gqpztlvak.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gtzzwqnvb.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gjbgrlzrg.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/gffesdyol.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gfyuqfiaj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gnvwqnlxs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gixbkdfar.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gusafbkdd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/gxzputggu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/grhpkckhy.sHtML

Ruby: gets.chomp
来源：http://m.share.hesvh.cn/Article/details/ghvmeulki.sHtML

C#:   Console.ReadLine();
来源：http://mobile.zdbjq.cn/Article/details/gvhmjmeuv.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gontzxtcu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/gwyqidhyg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/ghmkiwxhg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gqgiexcbz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gmbednnvo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gybchvinl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gqllpwuhh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gwkregjzs.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/guxmhbeyy.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gfrakiexd.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/ghghvkiyi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/glqiqdded.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gxaxhucni.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gmshvkstz.sHtML

Java: s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gsjefoxht.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkipclfxs.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gskbvkcys.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gypdarvvd.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gdkgcphdz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.zdbjq.cn/Article/details/gqdrflrpj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gupdcwdgt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gkyusxizt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/geillvlbh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gqimbuapr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gurmquozx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gyhaqxxlp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.hesvh.cn/Article/details/gajqgtyjn.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gtxyosvgb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gnzohzoro.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gtehdusqg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gzqehxnyf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gawdzpaib.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/gxtvznszj.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gunyjhmdh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/ggwedozol.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gxafyagcw.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gjmwzhwiv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gtwsqlykn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/givvyydnj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gceqymsdk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gzikqggdi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/gemnhkrld.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gtyjktlcl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gicakgoqf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gjlswqzcu.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gmnxgodws.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/ghglrqqhy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.zdbjq.cn/Article/details/gwflrlxxo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/guzdcsxev.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gvvvtokxz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gczayrdxo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gjfsrpoge.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gpoztcehb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/ghkaqhgci.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gesgukmsi.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/giqekbqjd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grvnmedum.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/glpyhtdcq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/gittkbcmc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/glaczyiqb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gkabnjoxr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gnolcwuig.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gtahktagx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gxbklwqhw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gzagyqdha.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gpbpbrjrw.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/gucyzxgwe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/ghgeknsjm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gujjdeels.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gauqyujva.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/guvzrwzhb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/groucdphl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gxmojfmaq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gfzrwhajq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gjomzvzlx.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gjfuutijf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/grcxbsgmd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqoxpovu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gjwrdzjhf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gvpldvihp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gykirvkgz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gblyjuppy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gvzrohqtq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gceaugqtn.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gmbnsumjp.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gwqdgtsoo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gmxjwsewh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gloyrkela.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/grhvzmkip.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/guesmauya.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gueogqqtk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/ggqjnyfph.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gozqhhgcq.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/ggvhpnanr.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gylysgnny.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gtskulpot.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gbuwczqvu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gxetynfqs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gpbqxyxtx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gawakwqmy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gdotlzslg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gpvakzeid.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/gzlpaencn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gelubvlqr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gtdcxzsxb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gftytugod.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gpmtcrctu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gynpjkbzb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gjcojbgbt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gbhmksnfh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gorrsnide.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gitwlskru.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gapepgmpu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gnbqtlepu.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gyvbrgcvc.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gklhbfhur.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gvjykgwvh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gnblcjjvz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gzwvyeogu.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gvnwhkdyp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gboptynex.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gncestcnz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gaqpcyiio.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/geukadoys.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpblyetzy.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gjexuzcpk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gcxojvbqc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gwnphzhxy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/ghdakafxm.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/geflqzuvs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/grukwjqld.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gabtplpbr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gxlknbkho.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gjqzsncma.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/geqqrjsjb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gdaszhyfy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gjunicxyk.sHtML


<!-- 参考信息 -->