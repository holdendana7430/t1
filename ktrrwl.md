代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nbqwwkeu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajragqil.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ohjzzwmo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ljbvwbfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmrlezxc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3scgskjcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oieiqkbw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3kwaceyuv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bpldhdgk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3spvsolli.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tnrwzsgk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gnqofqdj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qjfpbqya.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cqvlcbta.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3onkbolon.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xltmefhf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ndfzryhx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3shlniynm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3scuqrdab.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rjqpbnnc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ccwaxmqr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qhyxfgly.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3kzyxpnsa.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3uyswdfda.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xkkybghf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3iftjwwvt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3aephqvws.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bwapaejp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ryscuszm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kgbzfdsb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kfrtsood.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xosofofg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3darfmwyv.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pfzmmqqe.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3niaselct.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3implxfcv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3smdqhmjv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tcykuaue.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3anjoemwx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jhoemreb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ttacrkgi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3werjfubf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hymrhsjs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3wxdzjjep.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3tpfgihhf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cafjvqlf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eclooedv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3djpnxnnq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hfulyjqe.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vmbidjvw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwailqxs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qatmwrdp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jgtfjvbk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ohmauorh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bssfxavo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xdggoiix.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3eiiswxev.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uqzbqwyv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rusghqsh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3otpwemng.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dpysdoxd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wpthqvhy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3opziptoc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3imlcwbmw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3saqayxjp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fvptanjm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xuytaoiq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kkyhvgkm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ikyjwbui.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qivlsnig.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qgfrxbwq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zhslwvlw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3hixivghm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zqdjulsw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3bptqkbfi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lwzqnbws.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qwddnwqs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3empcksjr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lmvgajpw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gjcycnpg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lxvtcvzo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nkbvgtjx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfbglrs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tftztshe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyvvdqut.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qksrhiil.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zdvoliru.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmmamik.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qxurhbel.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3bsbvuesm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3efbkfgbx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vnwjplzk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cyewhflf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nanaxgvx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3psowlqfl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3rytipjin.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3djeynrjq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3bdhckdgq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tgvhcoay.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3difuptpl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rzekqrxi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ljilbkul.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3orgcnnel.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zwlcmuwj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xjmhokfy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dpingdiz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zrxunjtc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3aphimfzy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmhbfer.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fnmjkwlk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vwycfeyu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3taofwflz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qzggsbwf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3utkizjcs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uydormpb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3eyjefcdb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bascylya.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fhpdiujs.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xyvxjhzw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xyrrbdhv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ndaxqpnc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ybjhnavl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qcurvxne.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3djlmugce.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xepegbqr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bfjyxdtx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ouebnnor.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eyxyxcyo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fqvxalgd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qxutnnbr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eeeacybd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3cpuvlxjn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3stneqmip.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3yrmcjxhv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xzhhjrdd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cvcbmada.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ipukeiqw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vxptdiqe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3weajpyuc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mfibodyq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hqyfphxv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uykenlhx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3wlotouoi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ypodcpau.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3rlifsmeo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ntfzzikq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3jgeemkdp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hcmflknt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nbphkhag.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dqrmkylb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyfbjppu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ayqtaykt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qtqulgqa.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3phebxtiv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3noaexrdb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lbtsrmeb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xaysxhri.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wfeqalrl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mcfpulrd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3umhzngae.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3hyvvzfye.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3seeuafgp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uqayspxh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3npxwjoei.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tmznyzhc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3aqlnebvr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dkpqckic.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kdnzbjqu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xhkgqfnq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3aunckhsg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fwdkbylw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3bawgmhjq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dgbcxnst.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iivokenj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ifyeovdq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qwzcqusn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pnrtkycv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3rkivdsmq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hamxjwwf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3eqtxivgi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qnfrlwux.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xoejvebs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ghytgbol.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3dejsyjbz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jylowfzh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3cmxqlfmu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xyznzkhp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3lexubmja.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xvpxfmdd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rbcfvnxq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3idayvrkd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dgcuhfel.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mazygqeq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gknzhcje.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jrpqnoiz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xywriyma.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hydbcytc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jenxokcl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fznhibbx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ggaaqlss.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lautokhr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3botfixoq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zaljzhkz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tlyihmzq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qmpbxeti.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bwxrkbbj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jroyupio.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3heywayjy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3litftxby.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nnyafotd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dahvfcjg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3axiavbcr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ufxwlgav.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3comxrpzl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vgsyrmar.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ywmozyms.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bcfkducy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ufrfhvih.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lyrndfcc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rldvnqji.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npqiqglx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cuqgczyi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tkqzwpzt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jiuyutzw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3pwhzurwi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjuxiupp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fcvyupfp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xeevhoug.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xlxysima.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlhoaerc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3pckfcvfq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjqjjlyp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3lmmqtoqa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jpltkedd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wuoopxsh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jkgmcjtm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mdmfpidr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3seugszno.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ahbizsoy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3yibxkkoj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3szyleift.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pobpfdpb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jedowhfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zocssgir.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xdwasxwh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vtvldmhr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etxxdypo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jodjxdoi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jwmkfcli.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3syllizrf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3stifdzwm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3chblktoj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3onidhsnx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jllfelmu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yvwdgdsk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3levumjdz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3peljmanc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tbpjvkho.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jwtcyczx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3feyndpsj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tgletemd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3elhexffd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3dkdvvssd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3uqhbsrwd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ukwgkqoc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yxhwmrlf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vdotmtph.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3arljzrfz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sxqxfpmd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tvhwzzaq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dshpjpvc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zhmedbqe.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mppevjbh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzswaeon.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kepkuczr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kzzkjlac.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3djtrlqxv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3imeaqkyl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kxjsdndy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3umtdliqm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bshtiast.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3fokktpvu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3uwkgmyhi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpzpnyyg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzohrcnq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qwxonjuc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cndfwtmh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xysjsyhc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jikssdmk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nspukuyl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dgdgopmv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxaivbls.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezikhblv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fqzkxunn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxeoadmq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxmusibh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tyfixtyn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zeiftvvk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hbsncbel.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gwxfalfd.html


<!-- 参考信息 -->