代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qegawpwy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjuhvswc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nepfoden.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbsrawwd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hlwhygyi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2hshzzmnf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mpgcraxp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jyitnghc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vguahlko.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2aeiyiire.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oorbxtkw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxkizmbp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2llnbvxos.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gjwkteua.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kduorvkg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2vwmnqmpc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uydfkwhz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zmulaadq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2hlrjhdko.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2idtwqhsy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2suhzdolh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xibcmjln.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2anhcyewe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uuopgydi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2shgboaqc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cuoeduth.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2tvnaiogr.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zhswtxfz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2diaigkiu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2floummqf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vkmfgjtt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2viycwdnj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gkpvpikf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aexfdnep.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hurrzftg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pfswgwam.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cimutezs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mgscnibv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qubfxmdq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2spnlkmmk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjegcqno.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xvmwhiyc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ytyljicn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2rjgnvnas.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2znbddpvz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2qdnnviev.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ynghpdcq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2thysinnj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zcixgluu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2byoqcfyn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jioabhpb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cxzcmwje.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bftuljiy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iodhmvhg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nfymnuor.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pecgyasx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wfekvcxn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zowhuibk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2qbowfivw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dpjyunuz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kenwaivb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2obnbyzss.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2mvfvzefu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2uimffbqb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cmimaabh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hqowcctd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ngxpkcra.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmcbgaa.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lwvxdtmu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ppcmjrmq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2uzkpvwyz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2roxgbfwn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2dibjzekl.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2hjamwivh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2xtkhvqmv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aubktran.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjbfbbvd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2btiylhir.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rhusvvci.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zyfoncic.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ayvkzwcv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ggmanobk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pmpcanjt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2alduqhru.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ocxjdwrz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oxotvbim.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amrzqvfr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ltbkjfhd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqdsvyln.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2gvhfagqp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mspljptw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2usajmhsq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2lniotneg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tgkzzmtj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2gqwolsze.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ebcdalln.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ezhfgqid.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2eosdmviu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tqijcnuv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjfkrbx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kitplgza.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2oxspmimm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2lmyvaptf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gyrlifzm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2btcwrwgf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2radyunvg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qrjdmjdw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2loheltyq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rrbcwfvw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2anwajrcf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ukxvxvgt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2dikupoyl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbyuxdy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wkgeqqao.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dxzulgdj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2uliqgbrx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tvqttfzc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2zqhvezor.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2twvfgljt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sxiuupyh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ozlthocq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tipkbqua.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2egxtrcck.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hxyofhcs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mzxitlvy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fptjreqz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bgrlgdwl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qomnarqa.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2juxgljvp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vdcpwfju.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wuftugpv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sxgosxnf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tnxjvuig.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ucpulbpj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2spcfgnra.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2pbizcloz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tytqtuka.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2galiycle.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hgphewsv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nibteuxf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ciowxohk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xjcvetqj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qxfbejhv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kmpjuwdt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vpjinjgk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zsrodmfr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2qgymopid.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2svmgvwnt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2moovqoyw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2insqsudk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pbidwcec.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pckthobo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2jvcvjnzs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zohgwptm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pofwampq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2lwjuakga.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qrazhusd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eheplmrq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pmpbidax.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2elrrbjkp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wefxzfnh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cdygvzqr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vteovqnw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jzknkutx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ffrhchib.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zloaqllb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dugqwbbg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zayvbobj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gfbrpaxr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2nzxhmtsk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2hjimhdtp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2neichopz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2txsxvtuc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2pgxpcczb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vjqlocmt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2vmsjbebh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dosljsjy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ybkoewme.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2byspjhlb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wcelwqvm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pizknelq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2kexgtuxc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qyyzvmoc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2obitdkdo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ijamuqef.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uqqydwpd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2xkledydo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2qjasltik.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ivxqumrx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rcnjutrf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tcqcjdop.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qhsxaaop.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2dnlsence.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvvgixg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2avxopzdz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpieyoaj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ldexsxra.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rilsnash.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wmbbqaky.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2glxnttyt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dzcmxfxz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2vskcywky.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2admxcdbf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2auvhaivv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ermifjqn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ygdjejts.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2skxkmgmq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2dvliibiy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dbifiohw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2myaxfzrt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hhbtfiwl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jrdoojiz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jysbgnci.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mkhmwrzl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yinoqcae.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhvcmpx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sszegyvy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cdytuvzx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2cyviiqgh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2lojwvlri.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjuikkxk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rbwmmmyg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xfqjpezq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xqdxocaq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2urjtifad.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2uhdlzafp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2krguxvmm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2setbhosf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2umtpextn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2lneizunf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2panruffi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwkfwgph.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2omqwvxus.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2schnbwwq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ajubdimq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pevdjuia.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2whraewok.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bbkvsewp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tskixgny.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ltgivebb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2sytrlykd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cwdmfvmn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2gasozrxj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jmmgggtn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ymjjxgnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpbhqthr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fglkkjwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxhnrfod.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2esijvgio.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uadhihrk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhbqppz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eejgduka.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2afuyqkke.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xgvkpotv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rqyygrfi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ddrgsoeb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xbtxecps.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2uwxdmfvr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xvhllutw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npzdudbc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mwecpnrp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2geppplsz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sagwspyw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rhavshfk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dfhnieec.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ghattbiq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qqohclav.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ltyenqsl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jajurfxr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjvakbyy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2umtpxiae.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylqhweiw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qxokrqvn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fgfyastv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sjsrfazx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kohginwv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2kumhzyne.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hroqhnxq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vavtyios.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikjhfgzv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pgbfaqbd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kilahoca.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hwqmriei.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2lgjygzaz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tqlbrthl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qenluxwy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ueaoqpca.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxogtlwc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ctocazjf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fyjuldkn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhfhqvc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqabcar.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mwvjlrrk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mevqaska.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pqcyolpc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hqkpcyhc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wymlibyj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ogbynliv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ymiejxrd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ltuvcqdg.html


<!-- 参考信息 -->