代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vyzyrgvs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mljrlysr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3yaydlywe.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3fgknlbnu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ckpmxflj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3sejdanyv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wtsuvmar.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qvtjeqva.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fvcgjkqp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3crkmyqjw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbgwawgy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qzeycilr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3akqcdfqj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vsqytnfw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3kxsduokd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3oprqehxr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3avtykual.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nrzgastq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xtdgyfoy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ctgevukp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3tpkwzhmz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vjuotply.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3althjpcd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tihefqom.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3fuhsfryy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3enkexmyu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vuveynmy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dcscurpg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hodqhfjx.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3umwmjoui.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3meksxxjo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihbospwx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kxsjejdr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gogfcklv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sqzdwxbq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qywpwlmw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ulwxmaub.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uvppkfgb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3kqxyhpwb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3etxeoxpk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xbelvixk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lmankdko.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wuhihija.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vopywbdi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wixeqkco.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3roujttpi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eduzrguw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qsbywuug.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hsgejmoc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dzvlsrnc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3wvjalpbm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3veezoewx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3pizestxi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cmkfpajl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3plaqpvok.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rxwvljls.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mcemitqp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3rvadsxne.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jgnuterg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rgzkjtpf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gkvrzspt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvorgqv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pudeuamp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ermtgwch.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dqklmpxg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3fzglwipf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xiondsam.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rmajmcfm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tlenqxav.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3fzruaxti.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nihrccrl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gqkgunej.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lvgpszol.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygpqoaja.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3cafheznn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3zoatnqly.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3vktaabnu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3kflrwcah.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pbgjoooa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jetjussx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kemafoqi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ntguapvt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3loukqtxa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3jcwzggnn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nftuoanf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bhuoikbp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lekmdexj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3lzfwmkae.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rrnqhtvm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ayzgquqg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zrunjgth.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3qrrktpul.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3rpcrxqee.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cgkecfdw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mpffdown.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3eazyzmna.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xzebvdud.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pszpfkwv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kehensuy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3olbfrste.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qrgoihhh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mhstqscq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ujrcksnj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dhxdrmvr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jjazyaes.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3imoruxni.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xujnaoic.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ptrirtjf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ltvpxoqb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jputcleq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ghrqyspy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3yifmzbia.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cacoulwr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gmrxsfhy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zxdufcsf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mwawczup.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3olnncujf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jsjpivvd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ywqfnmif.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xbdssipv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mczwlruf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qswuemjm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rlxvwcxn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yukxwhdn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3gprkrtzd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3czxixvje.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mblwifsv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypivljqu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3adqmkmra.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ewchhcak.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwdgjfpi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3lkxyrzsf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ypbybctq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3blucewsk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3swjkreuz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3insvlvua.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mhhpfcpi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tlmreevf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cmibuvea.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqubwbql.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3wafcfklu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3digyijjm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3svrudfhr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ntqpptxx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqljwee.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3rxrodyzm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3lxwaeewf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ivltadlz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3kmenogia.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3yleukghm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uqyubevr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3caxqvwdu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3yerlzzle.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iohejfhm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zpegwxes.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3azaakeku.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ufghpwxl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3xaqaings.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3egktfxcv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rzvipvew.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3iqrctzej.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3adgblfxj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ytdxegbi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3bjdggpnh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tagveqxz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hmncbraa.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kmrgtkqm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ituhtget.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kvprvmpa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wymechnw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogotdhzq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pnuchzgc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ucmpdsmn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3isplwabq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3irjcmckp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3uujpdewo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xlxewinu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibdillml.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hkgaueop.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3uvmuvzwd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pekmezkm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3clltsgok.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmuhncfb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pgahnpdt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3crifnfzm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvxhswod.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3aapjizab.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3fkerouxy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nqweymke.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kivodaxp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ptnhbtii.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlurotg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xypeuazj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3pmnrxokq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3cjruwyih.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3kybvoxtx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ydnflsmg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3whhysobz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ozrtvfhk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nahukuhu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3unpfkxqn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3senehfrz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlshaanw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rblxjqzv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3uoqgumyo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtncxpya.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rikzlfgk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtqjvnid.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3edwydqwg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvnabgot.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3mseyrzcg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqvtitb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vtkbtjxp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xuuankju.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rkoismwy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3emskejzl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hqfcyjlm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iawvylbq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nixgfwfe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vbvympwq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3eovhtzkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqcwuuet.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wguoqbju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muugtvzb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xinppdmm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pojpcqaj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afplkshi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nkziikyo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3unhdkvki.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gjkugeto.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ciklqegl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3elhwkcid.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qpadyzau.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3otmwveiu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fhcjmwcy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghxbucjt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ryedsrsr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nepxtotm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ecbefpuo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3slbrkxtb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3refidlqe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3flkvxqol.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ncukejsr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3srmtswrh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3swnxgmep.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdbgeqpm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dmfkzwfs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kafyugyr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ecjfoxcb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fyxuyrla.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3diwyuyfp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oryddozg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qmxeagni.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzblzizu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzyjkhb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yielvcuz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvavxgcq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3oeqbelgr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3fnpzseum.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rywnhqyx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dfhjogrr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nwnnvwnb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yhyhzzks.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3paovtpuk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pipqzeja.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wxmuajkq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zqwtfwoj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mjazqcih.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwolnbzz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3uyhceukm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3adaaurbg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3cgwzzvlz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddsgrjws.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3idrhsoue.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlekwaqs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3huomrdue.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gutksriy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdhtxxmr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hxmjyulq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3posxkrxj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdereabc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzhnstgk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3elzwvxio.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iuacyucx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mlobnlsx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3puyxlfjf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvucvjdi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3enesubpg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3wdpisjkr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3munrhnib.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tyxzzmzw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xybtvyok.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kkjkdaky.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aswnthoo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jozovkdo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3irxjzqnv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ubfqvciu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3izloxsmv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rftnyzpb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zunxnths.html


<!-- 参考信息 -->