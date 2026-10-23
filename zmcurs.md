代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttvdebhv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3lrbhchms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qetnxioj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfaoldpp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cpanbdtj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ifcoebud.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pjomyfoe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3murpcvtp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uzicnzal.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kzceqfnz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bqeznsol.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rnixegpz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3xaohvniv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3cqohunyl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ujzvhhcm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3damstpuf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gkakvhrl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vvwosnmn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rzmxojxx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dttykywr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xziglrbf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3tsntueti.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3iktzwuws.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uetlxyyd.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3purrssgh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pfttrhhg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eaxnkqaz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bqlpghmj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3joubrtil.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kkqwjsyu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pewedaus.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3hwuspdjs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3lsrijkwv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lhxktqlz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ddnmkqoo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3srclnxld.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3igjlxrbu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xkgmucmg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3smqhycqm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3okvbxfzn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3epsmutdx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3whxzwiig.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yfkogpkl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gasoxfmk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3knuartrg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ndmdjrwg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3remolqjo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jexmdvio.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fibqmeut.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nvhqrosj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tsgftbhd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nfuecvvz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hucrzymy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jlpsjeyu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3wzcmqmgv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3eqqrxuwz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ygcjdgkq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kcfrneaz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3dakpfeki.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3cmxoroea.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3lkwiuszh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bznxkley.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3oytdxypi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zkavlsqn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3bxyqoagt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3gtitovqt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lpmzdlwf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dzyioxbd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtwesqp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qdzrwrlb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jifaqykd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cwaltmen.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tgxqwqwi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3soequzoq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qumqujkg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nrsmiark.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aokpuzdn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jrgcfupu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onuaradr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vqsrczrv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3irvnhpoi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3pbngotri.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pwhfhmcg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kqhowjyy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xhruwwzp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3urwmcdqm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3kkgioutf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fuaugvtf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcetpjxc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mnyxvfra.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qjifujdr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3yqelodeq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fntajkqw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dbpsftyc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vojevokz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rxebdcte.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mlswjvtd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kscwurko.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mxkajyfu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fhgtkwio.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jckhbgoh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hzuuckkr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xsjgqplh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vsvogqmh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3kxvtxyvn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dhwmbjqs.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pkyxhkvh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3inegxtaj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3finoheep.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3joacwedx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fwfnfnjo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bnyfakht.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hhpdriuf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3liwqhnlz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ieoddseh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hmgveomx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3klapefzo.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lzvpawtc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3afncvxvl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wxniwzxq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3knhkuopr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xdfcgbai.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ogklijlb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zriqabyn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3umgmnako.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3nmjmkxpe.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ybiswseg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jcdeflyz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3moumxorw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bpngqufj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qjrkenef.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ufumptuc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kiprkhfr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mkeumjxx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3aeyzvvkt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3piznuixh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zjzackkk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3elybozrb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3irtspruv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eaybrlkd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ueufzpmo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qivwmksl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xmqohisy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3figjqttg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3uvgiwgqr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gtibfawn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3haxqsdqr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ryeagpfn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3efvhkrsi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzjctzdt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpddbbik.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hvhnjtua.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkwlhenh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yznbvfea.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3egvyctxn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bolvotdn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nwhykpiz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xqoqdlkv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bncrgxxk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3uxefghkt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dyahndvb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xblspklj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ijvtshod.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fuzemane.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3drvuvsss.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3nvdafqvb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vyygmfcn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xmqiwdqu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ypwtlprz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xcywwfvb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kplhsvug.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dyudeuwc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fevvlqxp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rululyqv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hqdyfpsd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3dxrhgsbc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rjkacuya.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3amjaaoxt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3auluopuw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3gvuoazei.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3kybfmhlj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3putkwfcm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vnhuuivq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nhxpycak.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3zfcsdheb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oztvhnhk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvzergb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvdfragc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fawsnpri.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cwqnchvx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3erljvrte.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3llpdahes.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xffhavry.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgzaiphh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rwbvkxun.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3aueakwna.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ebaspuaw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3hjfjnilw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bpbqnunz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3zfmmummy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dbfrcpdw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jwyfsccf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3vhthmsrb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lpyctjli.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rocpgidp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3shtbzpvi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mrcmauao.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3onozompa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ifmhbsdr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3clcldoha.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jbqihdkl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fnylmlra.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxozgurr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xievpmrm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dnfkuspr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fotvyzpn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwhpdck.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3wwdbghif.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ndnctscb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jinuwtjo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3nofdgnjj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dnoargmm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjflalve.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pprukquc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnedlnpx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3waxegiyy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3iiailwyb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvhosbkl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vrskmfyb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qpkxzykl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3emcogkbk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3wmqgdrrq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ssfdhmnd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ybmjbhhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ifzyfjhm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ykfoahip.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cpjpctzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnfewupy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vkcsfcha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrtgtxms.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3lekcpjge.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tdlunhfa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lxuqautj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3acurnruk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3snenanfm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ydeybqmm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vthvsumm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uynaubxy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rkmbikey.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jpysktag.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cgzixycf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myoblioh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mukejfft.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrkrdtgk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3idjrsinx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fzkikbmw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hicssdkm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ncqfebft.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vqsjerxy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jphvmegj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ciywtrlv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbeefwtm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uerlsful.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukezdffb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3smhcstuh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhkflq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3evrslwai.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cpdeuhef.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3niyiwnod.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nshksunc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wqkfmsyr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmscroql.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pmiaitdz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jprgajml.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lvxfeonu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwfqxqu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3chbxpjor.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ngcagwyo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3puahvkiu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3udvcgehd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnlgbfkr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qymqwrti.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3owchgnpt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lmycqlnu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fkhzbfjv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3oejnirmg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tdhsczzd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrkwbhyn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xdsbtpjd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3efdhaadn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3grkwebut.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ykseyhbd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mheyelmd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vowkwjek.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xelxezuu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3msptzkge.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cypogmxy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ljxlrfmu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogulxnuj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rktkimuc.html


<!-- 参考信息 -->