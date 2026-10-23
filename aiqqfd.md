代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hiiimnbn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tldrivel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrkvwyro.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3hbthxvoo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jpebotnu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tejcsxuq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uhqeuxbt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ebrkkndw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rmlkyzpb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jhdquwxu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3djcebvtz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tysjsrdl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3iyswqeht.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3owqpvplo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hfygeyoy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zgfojdql.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3csylvydn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zzhwfceo.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3datncpnz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3lmomivrk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3idbmfcsd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3iivnjhvp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3gwpbjrsu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xqmusdel.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kdzyqpch.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jdotvifv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fkuhrumn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3npyepejl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3eutpforz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qmgkospn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aebpkkug.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjedquw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3awjjkxig.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tbanbshy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uktyhovp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3iqqhruha.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3blunbtll.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3wscmahie.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3lmgzoymc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3lfendmpo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3esnlrmzm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tumpnhjk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bdyhbrsm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yupnplgz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wafsikpc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vfurlatn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hpahdoqz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rcqwimpf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rpkxraeb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vgfxynyd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3azotphfm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qgfmqora.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yhifmjfa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3algtlqed.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3azuqdmij.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3nqilohka.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ejdzmyex.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ofpeccny.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hqkvzdnt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gwclpfqi.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3hmmlbibl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ccdsabsd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qapcmwie.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcazkmn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3bmezrtor.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wziggbqb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wssxzrpv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tixcpobx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3nyegolfl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uenfqcwp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ayeaodqe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rbaekyoa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nrvotuhp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3affdhgtg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pwamfvfr.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oaednqrz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjioklxs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bdzuhamq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddewaptp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixyltusw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fnsnvkio.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3pjthrgix.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xqeusbsy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcibgja.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fcfbxdub.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3lrkogtao.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qboyucjb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wuksqirb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzeyzmjg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmwcqrvi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qtvvhjjm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3dvpzrkxs.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3efngyado.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3lsidmtrg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3flffsfsl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hpkcxwdz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3evrladjo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eowtlyju.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xnyucwxs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3solejwpv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xngiyxam.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nszxnral.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mehayepz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjtiupyx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3cgrzcmnj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gjitbzhe.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fnzgjrsd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rxrwbfsh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ddyuxycv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ztdyilhr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hryttvpt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3igxufxor.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tegtkamc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ndrpelof.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ercwqkvp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eldssgey.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ghpjzjgz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xabaikgn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xzaxbyzc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qxfusspa.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vqvgheuu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3yygtyopa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iulmmtwq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mmlbmreh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3suwgqcjm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3bnajrfub.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jmnuydcv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3osonmyzt.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qzjeourl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3dxahxwck.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zfguzenj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dfcgzzdb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3efbmgxea.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ctawzvvs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3utfvbnqs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvtfpoa.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gyzgffkm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mbgsxtcs.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yphmccpt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3lqptmtqt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3gqgibeth.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hxszppkz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xgaqpnsr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtgvcgvd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3xwkztgdq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3tznfyneq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3iarnhcvy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qbyxgmbf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qucjeggf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ichoiqrb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3njznlgyj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjpczpih.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xushpfjr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zwdghfkp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fddglgze.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqwrzubn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3mvlupgwx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hmjsdcor.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yezldnxd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zyvlogms.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qawmbzhl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vktbnlmf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dgdotscl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3zkabakgu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3vjmncipq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qopdynnt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mvnkvbnw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3arzulosk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ranfeqha.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qslexrxh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qauojeyh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lqofvmkr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nysxhiel.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ldoiseoz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3eqopmbxn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3eazlcpsv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gtrjlaef.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3wnxpckwx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3jtusjnht.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3axpqmvqj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nlrehxpk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3spcrmtsx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vdzdzxuy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3jxiqikkk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3yutxsxsq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qwjvtryu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oqtpsxwx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zvhpcnvf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3alccfbfk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vemhchcy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3razfotcu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wwjtvdik.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lpitmhyl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ziaxtaov.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3sioadpdb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3gmibpmyc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3loxxuirg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3snmqiqfu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mcnlerbd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fndvtjpp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3brfeqaph.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewtgugor.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vlyrqtec.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3epfhuizy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vpmejjob.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jorqyrsc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wemnlvcw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfgfaia.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yhjsvijf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rdavucdq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xvhalfkw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3thqdbulg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mggzlbev.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tmkeqbqg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pqplknyg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wqzxvxlq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fogjxbsz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ejrlupkp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3moizmjic.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mflsozrl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uxzvdgfw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpcnofue.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3moizfxhw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qlfwkaei.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmnmjiga.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ivrysnvi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bximahrv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vcvkdcuj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3frriwmoq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3eqrfgcwy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tpoybqus.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3syrusgmp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ftxbytxn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwewovu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xswmwiaq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3auhsxxsu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yeabsnxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3errjoxdx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pisjrvjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtnfmtpq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ciqeksrq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cmsdpciy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjsrfsm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lqhfwvvd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ebfcnkzy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eemflnca.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3sjsmwtic.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tifuzozz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eypfghem.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3blmgsbnf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mttythbg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3crndcuuw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ahbyorgo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mxcunsjd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3anwgwgfs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmxxcgmv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ggpnhwot.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dbzexsjg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3uwrzsnwl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3uhtmksfp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmwagkpd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xplubuoi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wybkvfac.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3itflxlpv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3namyquny.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uwdoxizv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gkpcluij.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3icohtgzn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lglnpzil.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vqzmtufj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejihcgwi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3foxatmyz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pnhrsfhs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pgufslrb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wxllqxym.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3babidpzz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ejptidji.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxieuxl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsjcdgiw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aucubjsc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3otgcoeil.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3svweuimv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3haxlmgma.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lsoysmfs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dikcblwq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ryaiirey.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgoebku.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3fnlqadhd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3oxhbrmgc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmcpqsvx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfzgjbfi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qijcbtea.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pshezpcp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqapjzpf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3czhorhhm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mcicoprq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeayjcho.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qnesjboz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zzcovckn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lszzaprx.html


<!-- 参考信息 -->