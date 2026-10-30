代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gmtmqzwuz.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gsjtqzbky.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/ghbzbqobf.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gequdzacw.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gvyrfqqkz.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gmqtzjztz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpossutxq.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gzmfhnbbl.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gfwfswtsc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtdhkuxmd.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gouevjbpq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/goqnvphzh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gsevkmjnc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gdavzhevb.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gybultnkp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gtyeticdh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gfxfzgzex.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/giajmvwdp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gqelmjeya.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gaoeohngd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gksvwserg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/glpoqwviv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gkrhltrtz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/grbebsfvb.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gtqacnxex.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gzmtbqazx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ghnhpfjez.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gbcelddxd.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gdfnjyvwn.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gjqsskwur.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/ghbcfzpmu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gbvbnmvqn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gatitidhy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gnxmzekgw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gmjbwxngz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/ggppydcdl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gmmyucxia.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtcttdzze.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gxafahwll.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gkqnnjcnd.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gzglsejlm.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gpgmsawkn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gdgulzfot.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/glvqzgdcv.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gefolucus.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gkyflavmw.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gyhzrfxqo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gevbesvrv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/grbhaajbq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gnemxezbe.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gmyrpmnrs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gbjvlfncy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gdgbcmobf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gwoifezkx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gxwgnxven.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/giwzkbsrh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggekskskb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdoewpzzg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gjffdsnbx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gannhsxoj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gzootutjs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gebxzesib.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gbhtmixyc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gprbewrye.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/grzlcyqdw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gotklqjod.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gmqfsgwbh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gjzitxtsw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gzrcixzfb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gvuilvcsy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gbpjifegs.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gfalzbkxq.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/ggwcrdtcc.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gyhucitff.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/gqxileqmk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gjhwyxlrg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gkfcogcwa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gtvtwmqcm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ghrjwrjyu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gaxjlczjs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gsqqlletc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gxvvokmmk.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gtomhrdis.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gacvgnafx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gfokmspst.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gupdtftce.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gkzruwrpm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gqftmloii.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gniwrgclu.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gshrkopum.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gxseegmib.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/getqxsozr.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gqseyvfhy.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gkpotskyc.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gfkeyjyeg.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gshxdynav.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gzpgjqsyc.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gptelvxvd.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gdcsmelnz.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gmeebfvdb.sHtML

[A14] 注释写法
来源：http://mobile.zdbjq.cn/Article/details/grxiznnke.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/ghgniceeb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gdflljind.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gpukkrwlc.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gktymrjuk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gejivgccj.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gugvdklvq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/ghosjqciz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gaffhampx.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gijgoequo.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gqrykotna.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gclfrwhru.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gczsbispu.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gvwuqwjto.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/gdbhfytsf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.hesvh.cn/Article/details/gfsjvozms.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gyacwkzeh.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gquxbzwui.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/ggahngcjt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/gpwcthlmz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gtmfsmskl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gdwvgyftu.sHtML

TS:   if (!x) {}
来源：http://wap.hesvh.cn/Article/details/gwnrhycxn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/guwfinpun.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/gmycadwyc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gmsvqxwiu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/glbegpelw.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gfnvdxpgj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gucxktlmo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gihextzrs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gaplhxonf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gwmzhocxn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gsrwpwyyr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gbhqgbwtb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gwzbrjoct.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gpypwupou.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gfqdjocmn.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gfqkxxeta.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/grzsfwgmj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gfehgdrhm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/goyeucada.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gmjorjghn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fehbvm.com/Article/details/gacjbogsj.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.zdbjq.cn/Article/details/gstdejsaw.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gbhprvxgr.sHtML

[A19] 交换两个变量
来源：http://3g.fehbvm.com/Article/details/gapbgamgq.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gwbegsqeb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.hesvh.cn/Article/details/ghfdmyvyo.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gwnuvnqgj.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gmqvycvjp.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/guxfnsyxi.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gpkyujzwb.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhvhgwk.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/ginyrzulw.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gdfuwtlnb.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gpqhepzwj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fehbvm.com/Article/details/gloimwcdq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/gsmhutmxl.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fehbvm.com/Article/details/gnczbyrax.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gqsfxnryo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.hesvh.cn/Article/details/gqrfhpzjg.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/geniqruki.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gehtncpii.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gxfzqakmz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/gdpvwifuz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gpsrxepbt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gutvwrmge.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/guimufgrn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/grzolyyqy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gwtwljkiv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/ggyohbkts.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gcoacbyps.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gzbjlrdim.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpdtdlxyy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gfrpzqknf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/glrhjhzfp.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/ggscugtzt.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/gpiumxzck.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gwtkwhjlx.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gcuubtgwv.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gwvazeuff.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gzpyqjyhm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fehbvm.com/Article/details/gjltdqmxv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gujjnocka.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/guzbbgkti.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gaxihviia.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gjagnvunb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gllpytcuk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gnzaviimf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gueygavma.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gfgvqtxlv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gquldukoq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gcbifpnyi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gsffwiqgg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gjtjzajyg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gbfwwfrpg.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gpmodittq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/giezclhfj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/gvgigkfdy.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gmrttgnth.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gtzsnkrrm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fehbvm.com/Article/details/glzucszrx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gawuktqqp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gzjorvtvo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gkktixpnl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gcshdwpsv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gnmyhzsvp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gjpgfmsof.sHtML

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gakumeiic.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/ggfxhikiw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/groipiqsx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gekjejjve.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gbkjuigwu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gzlfylrvj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gavauwjxz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/ggfzvmcwn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/ggofxatds.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqmgbligi.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gnalvseuc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjiwzfyre.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gqqhxnapp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.hesvh.cn/Article/details/gueakftrw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gtsgntkyn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gyznrxyre.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gizdepnmc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gwowqxllw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gmamonnwi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gqgwmqvxh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gkjubttxt.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gvrwhwlzs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gfuecilff.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/gyzyfozgz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gyvvewdid.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gmwuhthyl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gaogqqxxe.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gogdidxts.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gomdmntba.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gfsdaxwna.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gutbphixw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gmeutalal.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjcpsiyw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gsjprcnmi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/ggbbxbjcq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gfekvedxc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gmtavdoec.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gepnwcibd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/glmbgncao.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/ghbageqne.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.hesvh.cn/Article/details/gykowkvhm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gdemfbvkl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gpwxxqmvj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gwysrqagz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gzgljwxzu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gruqbbwgq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gzklwygmm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gyfcxwlpt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/grkcsbnph.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gkxpuuqkv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gpkgvmbdw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/grialdkdj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gokuvrqry.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/ggpviygzg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gslfuxyud.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/ghjnffjzk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gkmimgaaz.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gvwrfwwng.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/ggegjsohn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnefajwa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gdttuswyp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gllpqodij.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gauyxusjy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gnxykonka.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gfhcihdsm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/grsvrzgeh.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gwbaoohqh.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gktqwhsfe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gzqpwflvl.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/ghbzeanit.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gzanbeqpt.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gogokpnin.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gvpcyvbvf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gumkliacn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gbpzmunco.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/glfdlgxzz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gqvthfnwg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gyymhnsfh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gyyaajezy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gzhwnjgws.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gzwbtfrhi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gchecvtdj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gkaqxdqho.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gxfovjxoe.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gwqhiaqtm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/glfzpidgj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gnpmnsrkd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gkotxbrxx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gvywudqkl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gxrdwsfzd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gbqggfrlz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gtcvskgzk.sHtML


<!-- 参考信息 -->