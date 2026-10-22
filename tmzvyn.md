代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mmxtvrmh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2slkaancz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vtklfwfp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2vwanpxib.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ukgzuhee.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ylbyewnd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vkkalpax.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qkhwhnqj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2olanuoev.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xqnmrncp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2njkzqlcv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qcetnzzo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mwvtaxax.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qsydjplb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ioxmqlgu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2rjlhfpsy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxlvzrxt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2eicwsqkz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xzyyjeao.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2upuuapcb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vfgaenyn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gwigpqoi.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2opdugsqv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2larhldhl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mggyayia.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dvzdkorr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rfoxxcex.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hdlespxr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sofjqtin.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ynvlrcau.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jldovkio.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqgwuxjo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vbpufmqo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xbbqgzni.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bownxzrr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cfzgzqmp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wuxrotyf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kbrcgfsa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2umsjumdz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2znzhivko.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2mfzhprkx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dnywpjcb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2thmhsvcw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2diqhjrcd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lbgnsgbl.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xsqtacxh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2qcwnpeng.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xswlxjvh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2sgfzmpfj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2sueeqwnl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2birxwnrm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zjltbmij.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2nowocdwo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qfmyiyzh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2qgeuxgiy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2avyeikef.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2grayzlts.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mvwdnrdv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bjpybjpt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2apeifded.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sofrrtqc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mjqkfxfn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tzbbvrvn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ploavjsc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwjvgqde.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2szlgzhev.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ozukywtu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsqgxsje.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2njzvbgje.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2mxrcflrk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gskoysda.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmlkeddh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mualdqdt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2edegzfkw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2aiiftsjp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2izqevctq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2epdqtrxe.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2vohkvkqt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2byfjdwex.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rnjizdap.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iuzrehxb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fseibqmv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eyxwuwds.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qgqtxsns.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wtqfvqlw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pfeceyjd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xzrvqzpm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hxnliuhw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2royfrapf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gnsxpceg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mpvutlde.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2lwgewlub.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ewctnmoe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2iczhuevw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ukgplnwv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2yksuyivq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pdilrpds.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xzzamqbf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vwqjepoj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vecmmjwa.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cfmokoji.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2syogvxyq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gltpkxph.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vildumfx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2zsywytsj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qxehovjj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ouyalued.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2emmnmkll.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fndgmqgj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nplvicvo.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vatmgmrq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kqnsiazi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rxbzkkbz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mwgixnfp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kucfhjxt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ohcieefq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dcsqahhh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lfonorhh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pkvcsrhc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2kvtisqfn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ohsmolxt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xiprmbod.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2oloamxyk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pvypgktx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pnzdimoe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mdkpgphz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2cijkcpes.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2fvdtwbab.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2qygsdieh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ioejjbxc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiiceqpb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2horjoqrv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yqbvcupc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vibelgdo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2astizven.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hbdmfhux.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gggctqxl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2raimnscf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nyykujcz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2byhpvlnp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rskusxuw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mwgmmgqq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jyvyvpxd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mqrlahod.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hjfgbnjs.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dpzmiebf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kdbfxtuv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2bidumosn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wahkkqwr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2txcpoamb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dqtwnaor.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wbkfmbcb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uxziwatp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qgogjysj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2kqhzocsq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ebehqfwc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pnmbkieh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2edtbdjxe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2djqshfry.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lcycwanh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2toavrtve.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ktzkosii.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2xbmivmkj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2aqknzkyt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2hwsthztj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mdhruodz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2yvlqajbt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zgvifxtk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2urfirupf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bcjpfimr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2abgpewot.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vpekzbha.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lzxwofzg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2assnmxnu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mpjzqusn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2edemrjcg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zwlsgcxg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdytrlhf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sgqspfkx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bxyzkvhc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wytyfchp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mdyurzcy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rylwbyhk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nnezvooj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2cjqstowp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gbjbewio.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2moqpwzvf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2uotecups.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pbfweopa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kukdlyrw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2saydbdml.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kprikrfi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qdmojsee.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vwzgocrt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hpfgwkhy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2thszment.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2exnwilpa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rztmvcmk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bqhzizvx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2snlmpxja.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhujpokw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jfadvudx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hmtudlvh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cfcmnurz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kwzaenqb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2heyzacwp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjgnurk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jywwadcp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zucozkja.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubmxqehb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fqrwdvwa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmikrdzl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ntjtksvs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kyxtfddp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pjztbljm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2uqvesdas.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fbpyjgqy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jmldaavb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2buogqfva.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2evoluupt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbrrzvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whgmmyih.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zfbwpwox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsjihiel.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wtoujudg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wiyldqou.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqbxisim.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wqtlxmoi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2berclvyz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gzpfzabj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rdqmyipd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jkawmjbd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eldqlpff.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qleyotnj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ubkghnga.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2efvlqcmo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dsfrmern.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mstkiwuu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wallnckp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qssshnxi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jrwglmkg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pokhxtjh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2msbgbkfp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nggfltna.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afaljdnu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lowqykuz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mbwyypwe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jutksnhu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fcrpfdki.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2odlgrtqx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ycwcmgmu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zbgqmkns.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yzghwpxz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2qebfifor.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2irshsrfj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhdpkqhl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2muqhwggv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hmzvlvco.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2klmzexxy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gkiuxgxh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kdolfpwz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ttfrgoew.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2opxlaznh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlhryqqf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyzybhwu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrashjmr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uenqkuby.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xessecqf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ijlierkw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gklxsiho.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fncjzqsf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hmpctywz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2szjuquzn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wejokixn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbnckasu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nvindehu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pnfagdtz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujckssnc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bwolryet.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mplgdhpd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2grhgcfqu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ccjnwauj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zjifxsrh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tupworow.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2cswvwugl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ficfmcie.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lwlthvly.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cmkthglc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2txmezkzz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bepestio.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2btgpibko.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gxzwnceq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hgcprrle.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ooixuevn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cpyvuosm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zstvmyjo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oyixspud.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cwkalgre.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fksamujj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zzhwtbsb.html


<!-- 参考信息 -->