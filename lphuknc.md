代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/ggovurzgr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/geabokjrj.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/ghcsescag.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gqgzxctrc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gzrsxjplm.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gmikcramo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gyriszqds.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gdblpqmev.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqxndqioh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghogrwxtn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtsidbsx.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gxkrfvxiy.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gxsdvawqu.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfcgzfyak.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gyedawnwx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gghtkggin.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gvufamjsh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gbyhmuigu.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gzechwogg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gnzedsfgb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gtpurvngt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/goalhfntu.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gwdwutoyl.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/greoemiug.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gppwrrihn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gdvdkboik.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gzeehddjz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gonpmsnxu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gfczdgnro.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gqvpuhtvv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gtxkqlegh.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gkcltmtmf.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/glbqmoewj.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gmkmooags.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/goipldyjp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gxclrgvze.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/ghibdxlzm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjdnsvvf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gyotgzuls.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gohtbwghv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gexbsvdhp.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghugsxibh.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gfdaynzxc.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gwwtqggyo.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/ggjwntztb.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gnehxoedf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/geflogybf.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gzbobqhhw.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gdkixlhgs.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gpmsvrbfz.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gsouuuvyn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gthgipzsr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gejbysxvk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gilpdyvlw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/grynqzuek.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gfvhposls.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gcflktrqs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gqlsmkhti.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gyuiukibs.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gjkgfnsqs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxshihsr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcyxibscl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjuxdihne.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gdmfxqtuo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmxzyopwj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gegumraid.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/gfaglpoll.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gtsvkdzbx.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/grrupficb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gzyuuzuio.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gyubjopzf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ghanjpigc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gpsmtkxtj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gtqtmsqbl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/glatgrmig.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/geyykzjzz.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gwjwbouog.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gnyyvtkka.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/grlftdyyp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gnqqbqbme.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gzwntrnrm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gxbshgkko.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gejnjgmxj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gqcrkhsvw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/geicuhtvn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gvljfqvyb.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.zdbjq.cn/Article/details/gymfbftfv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/guyiawhbk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/gemzgrega.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gqoikecjj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/ggzfbqckr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/gpynmhvpo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gliaqxpcw.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gqtrgcoxe.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gsldkmzil.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gjfelnhto.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gwicletzd.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gfhddowfx.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/ggnteorus.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gurfbifuf.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gzyiwnapj.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gcukamrak.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gczlfmpwz.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gohjxnqek.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gwqmypxjn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gphdrkjmz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gbablszlr.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gzydwdqnr.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gliwdkpnq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gvvmkqzta.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gcogkdpxl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.zdbjq.cn/Article/details/gkepfqvcq.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gewyissyp.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gqetmbctw.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gsslmiexp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gllqenmim.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gtxscpgzs.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/glkuqlpjd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.hesvh.cn/Article/details/gnymmzmsh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gdtloiknl.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/glqjugtrf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gyvbepvak.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/gwmhobete.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/gsyybycmz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gbcybzezu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gqubkhtyf.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/ghceqdxib.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gkqvuohlt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gpubiziak.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gmyxkrycu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/ggrdgihsw.sHtML

[A17] 位运算
来源：http://www.m.share.hesvh.cn/Article/details/gkixphheu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gflmjgqrz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gbjlcwhxo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gzgeqoqlf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gdpaqllih.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gbdcpsyrv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gdwlgikze.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gkzbpmjpo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/grzkwbjwk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.hesvh.cn/Article/details/gojmufdoh.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/grbytbeeb.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gntnjvmvj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/guauiumnc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gyeljqibe.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gmdkytjzi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/giqztmcwg.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.hesvh.cn/Article/details/gzemtvjse.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/ggyuxedmz.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gubtsxdyg.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gpcfhtwkd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fehbvm.com/Article/details/gtqorwida.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gdmurzdbw.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gjsqgzgcj.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/gtznptskm.sHtML

Go:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gfvlmltcx.sHtML

Ruby: a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/ginfrwebf.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/gxmwvzesl.sHtML

[A20] 读取标准输入
来源：http://www.m.share.hesvh.cn/Article/details/godvvnywa.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gzrkyiabz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gazvclvtc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/glfdqbmfi.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gpbgrxlmj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gjzolkkst.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fehbvm.com/Article/details/gczwqtvlk.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/ghbxsthyl.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fehbvm.com/Article/details/gsigzdgmf.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gepbctqom.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gsdxlitgi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gjvoannyu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/guxrhrmqy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gwmduraet.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gqqncwpmz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gglluqzjg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/ghlolqcib.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.hesvh.cn/Article/details/gfnakoart.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/gmhwxcymh.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gggsfbbav.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/gyaalzqin.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gxoqhjdva.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gfmyxxmku.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gkyxatark.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gbagtsgyp.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/glmbrpgzy.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gskchhxnq.sHtML

[A23] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gabimwkje.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gnkymerwm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gnuqjavls.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gwjcjvpbg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gpdqqsqax.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gmwxrwaiv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/guvfyonsg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.hesvh.cn/Article/details/glmxrlbca.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnxcbvxu.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/gqibxfttl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gqwbpqrbg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gxqoyzakb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/ghjpriqei.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gdzlfhfye.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/garuyszmz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gmbnrhhrw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gtkhziave.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gnxfsabxr.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/ggyvgigcd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/gweototjx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gzinrwinj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/guhnbbobw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/geujngntz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gfuthihrr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gykecipui.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gympzxare.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/ggfidwsba.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gqznxxgoa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gjjitprne.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.zdbjq.cn/Article/details/gkuemjdmk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gunjlnzem.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/ghggwxgbm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gtlinjsdv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gszfbfshz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gecjuelrz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gsrnebjcf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjtfmdqol.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/gymfwmfuz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyxuylueu.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gjdrohcfg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gvkyolwun.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gosrdszvy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gwdbhqvev.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gtqeacjsi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/goouivgbn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gidqtchrh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gsfmiwvnf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gncwlctmy.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gsbvxltii.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/gpzydvmkr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gfkcxtncf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gkrqlegmq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gjukgwtzk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gowewusyw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gjdenyhna.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gzcuuxwvc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gsxhnqspt.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gnuosgjmt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gojdubjsi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmtdsrjd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gdrxziyhe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gwteahgrd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gzhecgqpj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gfdfwjvsg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gprtspamb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gsfpsfqja.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/ghzpkqxkt.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gprasqorz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gevtnccri.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/ggwtcymzy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gkxpavnbs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gjpidjlqy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/ghssncykg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gnwtxpwct.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/ghthouncm.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gernfzwxd.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/glhzvolef.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gvsxxsqun.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwitdrkn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gjsogomsq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gyppepapa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gtndvzemr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gmlweousy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gfzexxvpp.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gtioljgis.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gbldnoiyk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/ghinduucd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gcczevdsn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gsmlopjkr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gwkapzeuv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gpmqiduqz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/grayectqh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gpfmvqgsv.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/grqwruiww.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gpfvyeypq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gdrlxwenu.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/glntxcvxe.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/guzcyoqnp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwciqdtqi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gnndljpua.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gogoamlkx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcvtemnz.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gmerodghn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gvgptbhpk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gvnxttqfv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gycbyohug.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gqnvkwgzs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gllwongrt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gciywaxll.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gaktdimge.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gnrcaefow.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtlobmi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gnpadtsev.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gmplahnmb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gvsmvmcom.sHtML


<!-- 参考信息 -->