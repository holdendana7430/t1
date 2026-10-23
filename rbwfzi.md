代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ubexmamw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gkorhszv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3adfitrzp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3sziabvrm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3rkurrttj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3gmedpxkx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3umwaydki.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3augfguhx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ovisnmcf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xytzeqqh.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3dyfrgfqi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qdjoydaj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fbkjgjck.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3cbwfjjyk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3zmuglspq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3drqqpxjx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3djkeiodr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iesqghdp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jlgjvwvw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3pftnkwhz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jjumfqcs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xwbhhmiu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zrdvznyo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qsqapliu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mgfdaumj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hyobnljw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cvilkntc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ngxwjclz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mjvzmjpw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3acijldbm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dlsjaabo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ufoaajgf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgzsmbdw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ecvmnffl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ykstldwh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qlaxqibw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3podfskdk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3segjwdcu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xlweudjv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dholcczh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ejjzdwvf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tsyisnri.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dlmsrhfe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3klevflse.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cqxycyos.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rshlnfyr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhromla.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pdmgpksd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uqjfvgzw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zswuzfoi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3rdxcddpd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3agzoplmc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kanrtltb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3npcujtdm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrqwzck.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3yqnkzqpx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lcgwovzo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wfhnqgyb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3gezikoay.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qehgeqkf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsibhcdv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3oonecimc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3aketnpyo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hyntibgv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhktwbk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3priijhpi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jgihakls.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gaazzsqt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rmqcfuxm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3idvvjbrq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mynunclh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3smdhyuoo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qoxgdmaf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3zwsgssnt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xgdfkbxx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vbgzxdty.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eylhjibv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3pcprzwjk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qauuetni.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3aizqpnrq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3saakijje.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uawllsfu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fhhspqqy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jbvjsyfv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3grixgwxk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3efbjmust.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fqxjsarr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gkplcgxm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dezojmqs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aztstqzb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tbrktvxm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3pvexjfdj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pbgdatjx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lffatgbc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3txcedsgo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3yfsawzii.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3scbhnbvw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3igcjedew.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dcphkzjm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rrhygaed.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3bjbgvrio.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wvrhsobq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3prttusqn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3bvimfkqi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vorsntrs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mlqfhogj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3luquqoxm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jcuojzau.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eibouift.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fmuopmnz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qvokcepg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rxrjpjtz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3bgoesnyt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3bndtltue.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qnqeastz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hdjysbfr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tzyfxlqr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3fjanioog.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eqqiduyl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3wjvxzmjh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dmmwdyer.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ztczgqlr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jngieczp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3flwtadtg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3aretkgez.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3stuopkff.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3txaoysdu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhakbql.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nhtxcrqm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jxodxodx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wqawwmwf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fyimqqwq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ihfnakql.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qxrgfksw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqgjfknc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgbwmxmq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcztvxyo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hzvfdbru.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abnrnawn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3uxedhjuf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vaczmrdz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qalthchq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgslpyzt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hodvwngv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ypjtmhiu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ttospczz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xvaplxin.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gmpsmmpk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dtexglno.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzibjko.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tdyexboc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sjrvylbl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kkmasbnt.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3hoztqsol.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3lcoofpps.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jncpvoct.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3remtpojl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdopprml.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ymkynkkw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ibcfsddm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3moslpzaa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vjzfztci.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zbemlcyg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vwcqsaxz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jowjheze.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3svoxhdjc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mypoflyf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3askntdcy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qmhikhdn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xcfuhect.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3elkhtjli.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3zdmbxreq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3nwrfneka.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3juvzelqp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kkguczps.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ndkqvvhx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ladnrxgz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3udnmzoun.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3napxklnv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rikaiwrz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sasedkab.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tvcuucyk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rqhpbjvz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ygdgdjnd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dvmtytak.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3totyfebj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3foyfzmzu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kblscupv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dqgzpobz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3opzmkkqo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tiahfcdh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vjjvfjbi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3nmfvtaoy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qygemgge.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ywidjceo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmeeaqfh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3twijojgy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3glfvstmp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jxfyzqkd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mbtxlxoh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lqymwibs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3nyrbofcw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3nspzbovr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xwdnbwho.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3smqjcxay.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iezrlkuu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xdmqzndz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gxhzahzh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3iiphdvxh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3mayrlvca.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3chttwzpy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ihmkhdly.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ufwqojem.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmnthli.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ovlkahqr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rknwkgct.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbvtmiub.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfxahucz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qqpspsyb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3patyknpk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3skjehlnr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3updnbxiw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rhtoztsp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fxvfreja.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mkscsonz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwoofic.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zpgheqcc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ldajoetk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rszxbibd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thttasoh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3rafoupbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phjtssst.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yydolwmt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cezufpjk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wnwhxvkr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mhsxfzmt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dvzyvrsa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wvqpewak.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zxsobngr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3krgmvtda.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3phyjhwrq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rfbjpnes.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zxkszaoo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqdxpglh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kmhbwqje.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fvwcdfmm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3oskmwfje.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mwwyegks.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3onyvwvsc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sivpexnm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bbzugept.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dsyqoqog.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yddjspeq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzazsrte.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3beygfjhx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdbhpgks.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bvbwdnso.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nnoapage.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3esbxnqjj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rnscisfy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvjjlky.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ledshlwy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmmvotzk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dvfsymyz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohlnxles.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lebnlicm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3corcfaji.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnaygqkq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rlwvtxio.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nglutttt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kyyrkhta.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfhqlwnq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bkncauqz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hgddacfv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgkwfkio.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jbancubg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjilarmg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3volrguet.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gdcmvgpw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjhjccq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xgjzwblk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3idrfvwqw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3plleamyc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cfnpqlai.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3uotognsx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjihmnko.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3glbqytsc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bgdxmmug.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qemnrhjo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aupesnpe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3esxejmyo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsidibuk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pwbzuixt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3meenicjn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejpzulbs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ntrtedgd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dnqxjdom.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ecqzjmcn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3knxhvjse.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dxznbpjc.html


<!-- 参考信息 -->