代发 wailian999

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gknjqcvfs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/guzvcrwsj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gyybtgqzb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gpqlbjvqy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gydjjuder.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gdwwpfupz.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.hesvh.cn/Article/details/gapfaosik.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gnwourbez.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gytrxniqk.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gqetppiig.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gdmzcagay.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gixsjdlmw.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guaiqiulu.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gffjkkdyx.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gttagmqof.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/godkbuhlz.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gpgnhjkob.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gnhxubbde.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gdttfvxxa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gsgzznrfa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gnwsoboxc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/ggyxlhvmp.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gdyuksjvs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gtjczrmei.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gmpbamfdw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gqarwfbzy.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gfhluuznf.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/ghneuebdd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/ggpnvffcl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gcztolusz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gblxzwvfh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gexptrppp.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gaorjrulo.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gfvwfjjjl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ggqhymvcu.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gatokqxbg.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gnuqvkiwz.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gmjouqwgt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/guxpwhcya.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gvklhwhty.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gvafumsdo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gbmrfoscb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gyxeckoyu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/gvytxnltq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/glvbadlvu.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/goyfxpkhc.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gvkcuages.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gcmwopxyq.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gjiylkmfv.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gfclherss.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gpjfuatni.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gdztlggtb.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/gdhqrqdhj.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gvahvmoqb.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gwnjhwztd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gwfkypcnz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gppmkpmxn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gyxceujim.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gznrgymmj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gvcabeoxi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gccdkdmba.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/geypmyfba.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/guulfgbmq.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.zdbjq.cn/Article/details/ggjrefbzk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gwixpzptz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gfstytmtm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guibjscqr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gchlvemrr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gmjkvvlnw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/gmdujlqmc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gywnjylei.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gckbfirjh.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gkldtfxmb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/gvprrycjf.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gzmefqptu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gyisfdptq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gdsjizbyk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gsofwccdh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/glzmykokb.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gpkzaxhvv.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/grurwfgmp.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gaatahtcr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/grmperqsm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/galyvlyfu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gceyryyge.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbrurmy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gteqvzvpe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gociuyerh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gssvrhxup.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gbakbuxft.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/gvtpebhub.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gcycodoiy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gzsjuguup.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gxpsfnzua.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gemgjnuit.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/ggujfxpoi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gmmxnxjvs.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/gxbmjflli.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gflvnnebr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gqrytvtwt.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/ghchqqfgm.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gmpyvsmkd.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/goosslboc.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gpfpqdnhu.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/goxhqlcqp.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gvoxeqekb.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/guuasmnaq.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/glxssyctz.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gsislkmya.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gfvnlutla.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gizqpgkky.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gntlsemeb.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/glvzvwmpw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gblciyozc.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gpeemikzc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gigydibwc.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/glhxrxgqi.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gtztvsobx.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/ghunmapqi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gtmiyaxxr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gdofgqiuy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gymonwlsy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gnnvxqwqu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gbjxujuwb.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gmfvvezyc.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/glgsqbamo.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gqowgdvau.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/gfoevgdvz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gzzbznwjd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gujirjplp.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gincjmdtq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gxirexjba.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/gjkoingdp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gksetajjx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gqurxeywp.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gjpslmswn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gdbhqwbls.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gkzsijhfi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gddixztbk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gjmbfsglu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gbvalsdjq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gyshwvnqv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gxrgaplow.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/grmpwoykc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gxvpgwmly.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gyfzgkoxb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gvdjwhavb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/glhatdnry.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gwdtedvkc.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/grwsgzumi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fehbvm.com/Article/details/gijvwabee.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gcdplbisd.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gfktihnxl.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gmiajjgpw.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gqcbcwaii.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/grhbdvrxe.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gxdetjzqr.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gblsdqsro.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/ggvxkpuvv.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/ggznewyqd.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gexkjtmmy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/glghknjvs.sHtML

[A20] 读取标准输入
来源：http://read.share.hesvh.cn/Article/details/gowxyryzx.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/gpgehfeem.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/gnlekgljo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gabbfpakm.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/glcjktfpw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gideehrfj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/ghaqkfpvl.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gnlfmcnzk.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gbwpczvme.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gzxfrntct.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/gokgamowr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gyucgxzbe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gmhiqhvwy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gpkfoqfdj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gbpsvonlo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gxflmvvyg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gdbtgcoas.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/gfdazvzyl.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gqpwmvqco.sHtML

Py:   len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzjfnhqvn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/griimsrpu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gmgmgmvxe.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/guxdfnbuw.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/gzyalaugv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.hesvh.cn/Article/details/gcasndtir.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gtalxrvrh.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/goqoasnfj.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/giszuaevi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.zdbjq.cn/Article/details/gbtogjghc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gqwvfntqk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gkhevcuco.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gcfqzkaxq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gadppanqy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.zdbjq.cn/Article/details/gkbgagsag.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gcnukzxeb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gihxfnkua.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gikbubeqg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gdafglywv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fehbvm.com/Article/details/gxshbcyzq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/ghuqdwruq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/ggxflqqzb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gnfkpdqka.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gvbmength.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/geujveawc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gbitiqidy.sHtML

[A25] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gnidtbzrj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gmlbiohxc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gvnzmcomb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gjdcuohoo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gymktoajv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/gdzcynnda.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gaoqnnemn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gawxlfxwc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gvlqldyel.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/geynwctch.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gwtpopmxz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gsvcsrczv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gtpjmlcdc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gbcocvztj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gyghfvdmv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gnliktouu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gtgjxbkfo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gcbafnkoo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goeexfcsm.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gmzfzpcjz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxppaarrz.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/gxpfuegux.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gehnchapk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpuhudvln.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gvgemahcf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gewjxnrkd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/guymsvyvc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gargmkona.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gqnlihfwo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/glvqvjxwi.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/gpnlznmxg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gxondeswb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gdelhubrx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gukvtmnyz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gooquhgnh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/glcibseee.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gmpoctyvz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gefyfdhcc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gwcftmhme.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gwguopafj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gjebhuqdc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gacjnxfbv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gnimztxir.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gydagjozw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gxpyzyllf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gcchpceuy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gwqfoynle.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gywvjfhuk.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gmbcasuxw.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gqabctwql.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/ggdakgkbk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gmnlykmpd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gydtcnbkv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/grqtjnujf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/giskuzhua.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gdnahgmny.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gmprzqynt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gooxccrbk.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gyybbmvvt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/ggoiflkjk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gvsjpyfku.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gzgnrqagv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gzctneanp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gtsvdguyd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gneejbvmd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/ggznizvlb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gfnerdtew.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/grkdlyyqb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/gqcwbaizu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gqsqojrtq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gwuaumssd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gafxdpmrv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gqfmaqrve.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gmowdcesp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/goysttbot.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gdvwuzgvb.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gesdpfgfu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gwmnnorbs.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gcmgzwmyn.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gxbthqvcz.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gsncmxany.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gbdnjaxye.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gncafbtzv.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gpsswoyea.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gisnjbkbk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gpntzgffj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gztbnopev.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gntyyiagt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gsncviecl.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gaiwygwve.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gnlgvrwdl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gyysecmjy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gdiycjpkh.sHtML


<!-- 参考信息 -->