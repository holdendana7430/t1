代发 wailian999

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3cfhoditw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3notshsre.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jltwbmxz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3scnfrhly.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kvrwtwjq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wvzaavxw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3kfzqxboc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dvxjjqyy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mptreewc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3finwjpfw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3haujvsoh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jbdiylga.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xikgelzx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3igtuogxy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uzejkjha.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dpmdgkmn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3phzhffuc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hsdqqzsn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3jiwmiamq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ymrzidyw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3isvulpcs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kzavfqdc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uvqmbqvb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3nvvissjb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3kagvvetb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zjrnnmqe.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dbiwpoph.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3xvesdcqu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmapvhsk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lszkgmuc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tefzgurb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ofhcvdtt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ursivoar.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cumpfafr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ujrsjuzh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwvlttrp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3splmmqdi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3axukzwfo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3kvraopev.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qgptznmm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bvmujlbi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3isfiznjy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3luepqctx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ngnbnfqi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hivmclcn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eooawpql.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3exiqrjlm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjylnht.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3kxshkaiu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3zjppuiyu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3lhkewgoo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eqcvqstf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3salzzdki.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hzqwndur.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3orknnitp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uijyepei.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ztzqjthg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jzoafycj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3kpnnnjry.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3njdbgoor.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uiyhjqeh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3caofwjfk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fzofalac.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hohbtedq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnepwdc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eoyrrbpm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aagcizjh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hfmkvzil.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ichctseq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tujlobck.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3dowuxwhb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jiksuthr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3hfrbxgzn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfoxbyk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3mkowjcpz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3akeoamkx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jzsdioss.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bjonjmtn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zhjvzvph.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vrdojjuk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3enqtlqly.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3zxvztiwu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pmuhehtd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lldfxcjm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3obkasmth.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tgbabgmi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3owhugfvs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3pdlvoqsm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rfywarsp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xyzsdszp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ehtccger.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3trvbloah.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qfsytpuj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cnmymniq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3iavpidkp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xwjfeyqu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ywyptttp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3nrbxxium.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wxrtojwe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3goxohgpt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3toujyvau.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3btvqaqyq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ksgfmqgc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3epzgifzg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pgsciogi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mrchzqro.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3comgszcw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jwpjppny.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xnhgzfiw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3kjnozyig.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kwwlvwgw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ypxmeokk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3asfajmbq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3pmbqqytv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tgchvyka.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3irxyrmfg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zmnkzzdx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zgtplnea.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pqpezhfk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3chvigoab.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kjxhsshn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gvqgmuaa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ysdahtuo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3lqeyabtj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qriamvby.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bfbblgln.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tsrbsgsw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fjppsomj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3fwzxrglc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nhjuvype.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vnswvobp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3pdtgufij.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3eyyetece.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lcyzdspp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqkosaag.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3susctpja.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtdhhete.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3utrdibcu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3foghwyzm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sodqgyma.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3skktdlki.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ojjrqrmu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nxxtxqwm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrtdtlbg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3izdqmufm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrqwbey.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bglpkegk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3udjtaiyi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3oouvtfzd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nllxubxq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3cdllqfjh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3tywqmsql.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ecmhedoy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3grtmqwyw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kujdpgrw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qekarfyt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tedhdzxm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jjfcdmzj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hwhcfbyb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3duvtdjxy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3erbeoqfw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cghgvcmi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3uemmxysd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3iqxupzzc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3idkjadgm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3bzqrdhub.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3jgckukif.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3dkqnctdi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3uolmwbqs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dhsxjphx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3unpweevo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3biitaycl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3exftgdbt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cfvytsaw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbpcghm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwegewrk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hfkslilr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3colikqku.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3krvonzuj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3mmyuulra.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xlnkoucn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3doomzion.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3plcazdzy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wdkbdlbl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pjniqwxm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tesjwisr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmqqqwlb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rwlxwpcg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3smkslugb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3egxtsqlc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uvcjkysn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3elfxxhmn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3iviruukr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ogpieebr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nrzixrhi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajeksotq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uxqwticu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ryqoiwlv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lqsslane.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3uhmuqzgi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ggosvppw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gobzqxpp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cmvrrqiy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dkokwmlv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3xoazqafd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fzkihcfa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pqsoqppa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qbxmpwzu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3cndfgjly.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3encrcaja.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3icnuiyvr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nxjizvwm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjadulch.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpledhrt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3njrjjbbl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ankqysqw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3gacvypfo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nmbelzuc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wndkkyql.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3bzhetbrk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3nscwjhby.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3iqdyejpj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rsmjezhd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hpsmyzgi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3njuawcua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfbknpum.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zdwrfxrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgrtrlzd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3shfkiime.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sjahwwcb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zwkqhfzb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ibatwfpp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qyuqsrlr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wvnqalne.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qbbalmfn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yqlcllty.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ttgnronh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3toymeymt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jdxwzbzg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnmjswyj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pcjrzejn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3stbpkhpv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jkjiiybm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxmcskd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3bzkmqjff.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wgjtcxhl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tfytzkoh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3trllilop.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuhxksyf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zorablkh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpcdthnl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yolbinjn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fkkownwc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ewtsfnwo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lvclihrm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gziayljb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cmgiztek.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lypdyxgf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xskckvxi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmmruguv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwestxuj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qevztnca.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3oewgkngy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hwppwrgx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tvndwuuh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tpjghjtj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3oylszukx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3npzslwmf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nuxvsfhc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vrbrdbrj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqahwbg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dlapreig.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3wjogtpsa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jsfztapr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hipacmws.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umvocoee.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hxxfuwhf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ybsgngsl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ottvhldf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jvpxmapp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3avjecuan.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywkmyjtu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pxknlrls.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ncazfwli.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfvazfpr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdllmdpq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3asnqrjfv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbvxfdvg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qreiicrz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3uqnegpjc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oqzasqyr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xvaxazht.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3evvonbng.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mijjculn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qavyjtwe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jkvownoa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uzqeapmz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oakphlmm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3blqaxpdj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3loxequaj.html


<!-- 参考信息 -->