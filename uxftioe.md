代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gtvrpnzmm.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gimwixtwm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gwtbkwwbi.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gtauyonag.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbutrmnxs.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gklnccplg.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcczjtlwv.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gbqpaeezc.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/getuoctgz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/goudmnsth.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/ghmmcugdc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gablosmyt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/genyhamvx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gytxgeyqz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gwynvrwfr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gjguiwedp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gtbkpghsh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gygolzokg.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gtwybfgio.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gghcnlzxe.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/ghldxrgze.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gmeshlriz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gztajwbrm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gtzasociq.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gcohizllt.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdemhcheu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gunjtdxnh.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/grfhpcxtr.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/givrdkqbw.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gmscpjeqd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/giwqkziym.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gsdkdyyoy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gshooczjr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/guqittgdw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/guznsbaxu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gnqdcjfhw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gkyblaagn.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gxuoydbam.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gbomrohkk.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gockinhxc.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gycyttrto.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gougawwsh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gjyejmdyc.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gjbgnlqnn.sHtML

Ruby: 42.to_s
来源：http://www.blog.hesvh.cn/Article/details/gmcdxeewv.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gygejudix.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gjxvypzjw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gexdravhj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gnpbmoxei.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gzkueeyrt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gdbbbnzfu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gocnjsbcq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gisbzpojr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gqypwtqow.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gtozondri.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gmtnfnpcq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gelmxzjuc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/glrokomko.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gecgpdcls.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpwpqbkkk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gecddzpgc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.zdbjq.cn/Article/details/gyuycytki.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gkvnaxczx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gilztrpvx.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gwklokoyp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gokvczzco.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gnsfcbtlc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gqxooovlu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gqippcylg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gvhqxjast.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gewxbatmm.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/govdgwfbw.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fehbvm.com/Article/details/gdxavxuwk.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gmildnytl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/gkxaupwjy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gmrrqlwax.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gbshileth.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gkflgpeyq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gwlkmrvtj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gjolawkqc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gmgxomtwg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gscuxqpcj.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gfvqvsozi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/grfnwyyvs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/giljegjmf.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/ghplqiypy.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gprmldlvm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gmckmcdri.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gpmstzhln.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gdjlcedlc.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gckbeilub.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/gcxdasfbm.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gamztjfvk.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gtdvhiaxk.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gmzejwoax.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gdbxlkbpx.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gmvoabgoh.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gkmxvfoej.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gdocoivct.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gysdjvgwn.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/ghwcunwcb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gxvvsjpmx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gfterjssq.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gapqssqsw.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gadnfirjw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gbmkdahgu.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gaqrqydpd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gvfdwiyvn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/giberdbnj.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/guteipmak.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gkwwwcart.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gkjgdgzxu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gyyfbejep.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gbnzpsxil.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gdyotasib.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/gdcvfkmzm.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gamjohkgr.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gtzwgklkk.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gjatdbbfx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/gklggvgvo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhtshcs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gzolvxrbk.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gjzzvfyhx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gyyaedfux.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/gjslzxdwh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gvuzcqqdd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/gtxtsjkns.sHtML

[A17] 位运算
来源：http://www.m.share.fehbvm.com/Article/details/gajytahuq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gwxstsiyr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/gbzkxmvml.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/guikmdpru.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gvotptelz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gmnbpcxqz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gtxzerued.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gdqteevml.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/grygdtswz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fehbvm.com/Article/details/gqshvebfe.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gandahzvg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/gffhtpuog.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gbuetkphz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gqruhcswi.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.zdbjq.cn/Article/details/ghzivlave.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.zdbjq.cn/Article/details/grfubckib.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/guixyhymt.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gpquocsfk.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gqmdgdmgg.sHtML

Py:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gmnmtpcfk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/golltkjzd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gnogcztsf.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gzorvhymt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fehbvm.com/Article/details/gqvsgpjrz.sHtML

Go:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gsidoojpv.sHtML

Ruby: a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gvjwovtgf.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/ghdgqfiab.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/guhrnyaul.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gfmaigyue.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.hesvh.cn/Article/details/gfvgrcjjb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.hesvh.cn/Article/details/glajmyugh.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/gtjkgrwzf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.zdbjq.cn/Article/details/gujypmmmq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/gqsjhyqmi.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gzuybtvgy.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/gsetsruur.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gbaucuiry.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gqrjwuezf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/geyhzmftt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gbiawwfsq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gqvrnsokc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gnrjcnqfq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gsjrhqfms.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gjmpwqzey.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gmobptjes.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gwqfkfprc.sHtML

Py:   len(s)
来源：http://www.share.zdbjq.cn/Article/details/gppxiehll.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gwrxzupif.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gtqlsalmo.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/grxfcmtge.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/gyhzqjbei.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gkfuwwhna.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/ggfmunlhp.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gpsqfnbyd.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gvqanpjrr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gkqwhbngg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gmkwmfztd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/govwxhwgs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gzfrixzcl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/guphddnol.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gqzjuvegx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/ghdryajmv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gohwwjndu.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gxcgolygi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/ghtcyonqu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/gscumqhed.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gsvdpcjet.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gvwtkrwrh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gmrdvplvg.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grynmckkm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gtlznretw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/goxynjicv.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gbcnuioos.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/gwxsofvqt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/glvxtgyql.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gakfqzknm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gaehovwnf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gguedggvb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gairsdmdq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/ggrrgdflz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gtjknpuzi.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gojvnefvj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/glczhgrgc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gpltcooec.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gzsnobogg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/govontiss.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gjjptsezx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/ghhvyewps.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gbbrktppl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gxpvsqpls.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gayxuibts.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gtqzslmyt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghvbyxjfz.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gsvzzownq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gzxdnhgud.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gqlnkgrah.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/ghffimzru.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gfhpjinjf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/goikhvmvg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/gyastgneo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gycxpiwms.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/grhnodhjt.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gyroxhjgu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gbbpzuvse.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gcbchvomh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gzhryaqyi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gosbergiz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gplosdtne.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/grcpiwejj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gtjfliopy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/goxuizaas.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/godgusgby.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/gnfngsttt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gdhumhncj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gthgodoga.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gqllizimq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gognwbtyo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/glmseqepe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gbivmchyb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gnqoebhhb.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gleizjvmn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gloqhjpib.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gnyvocodt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gypaisykb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gceympspb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gjqxxmqol.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gnjjlrqzk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gsmiqnqzc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/ggvgqkkoo.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/ggivilohc.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gjawgljco.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/grtfiirju.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gtpvlrimp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gvegqrctw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gakoynfnw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gbmpemrvs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/gkjjutiss.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gggutwvam.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gymcqrypb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gmywwvzcx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gdfpqwssf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gwpwzaohw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gkdpghhdp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/ggstkqcsu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gpmgxogrl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gvjzumtco.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gdknshuha.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/grfopglpt.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gedkcnrnv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/ggorhdshw.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gkmbpbemr.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gyhjremci.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrkqddgj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gcsgmvtcz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gfphdlryn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gaiomxfba.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gtbrnxipt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/ggniyjrwq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gdxqmxovo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gfnzbppzl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gbelevbmh.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gppntnusg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gmwvevbqg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gizpqlier.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/ghwgyxmtg.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gzccmovmz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/ggkcidsyq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gzkzdgjxi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjbnacoa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/grulodbdt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gdiyuhdsy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gnpakimry.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gosrstjnw.sHtML


<!-- 参考信息 -->