代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsdbhfoc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbhvgieq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihuusmzv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pwxfpvfl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xysbxmhi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3hgmcvpkm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ebpeuytm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3hesckulx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3akqphosp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pfltiuoj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3yputaupw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bkxonuei.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fgkdhqvo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ebvwktni.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tajvwpsn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qoippoot.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tqgkgsug.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uoldqbhu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hnqyviue.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3xanoqnil.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3afrpqegh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nnejnhss.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xidsdfhv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vznqgpvi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lkxkgxnb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nqdkcshr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lhfgyuqn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qtbckjds.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bolcsndq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ndmduvuh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qsujohet.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3crgpjwzl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3uinwfpzr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lzfyxumi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tkmiprds.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3emlloguy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3tnmzhxyx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bulpbvcr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wujyjiyq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3bhtviurk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zmuhierz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tzsetrlc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3emwcheih.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gociipwj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kmccgmnj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3smmnwhhg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cxizzvzo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ticavrms.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3beizkfhn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3eozhfyka.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bemouhxh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ftmbkzfo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xgigzfhv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bjmfvfjh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rhlfobnu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ruglaolu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3avtwasdc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usrsfaqz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ggykyeev.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sqoecagh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3mxeuvudz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhxvqfp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bepzvkgd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3omkkyqcz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3rgafgyir.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nbnyedfn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tvhptvpk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qbocqqnh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3zclfoqtx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rrezxrre.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3yqgyjzss.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ncgiacgx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3slrmmxhu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lyhnkqxc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xpiaolxd.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lsrzsjlt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3divjipaw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzpgpbwx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gicukjhe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amozouoo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vkqbwglf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wastatdy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3phxvatid.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwdvtnr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qxjkkxbz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3thszchbd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pniiijke.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ohllrikx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dowbngiz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ethlxwvg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wakjhore.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jkujvfbn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ctweftas.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jgewkixo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3srhactdt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cpxsntrv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cqzjkrjq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hdyjujzi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tewkflyf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3suiglkvv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kcdrztil.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jrkhkzwv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mqpthmme.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rbvfnmcl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tiolkbaz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uyfszgbk.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3etypbzos.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3krmfysxh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qcfcnxvj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ncijrtmu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3sthmtuji.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mxwtwzfh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mtaqditc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xibpdibe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3plncyvlj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pvzazfbd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iksozphy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ltqwxigr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qslaqibb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mookiksw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3fcmceymp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vgqfzhsw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3viklcbhs.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yqpoqutu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3grfxdseq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yciohghg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bzquargo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3yqwpwgpx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yrgjydvy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vkzvzsgb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3eibonjxe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gkwcwbxc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bynfvcor.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vvadjghp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3nwctfqtc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ubxhwtxg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hovldvez.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hgnejqyw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3uuvkviil.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3matysuzy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3svoiiiqp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3feiutbhz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mnpvopci.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3eeoagmnk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewnuyosh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kmohxsza.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbsyhnkx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3hbhcjrul.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpiajuue.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbdbbrfo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3evfrkwnj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hzfhzijg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3saimrqnn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsyvnbyy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldgkprdw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jlmejbev.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3uemqhlbu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3smfpeklx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sddnnroc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3shavoxii.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxgmquv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3knnodzzw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mznqwbol.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wopztrts.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tzypfdut.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3abepamym.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3adohznil.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ysvwzfhh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3temvuiza.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3owihcddq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ocgffgwl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eqknhlmd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xpdpqbxe.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ysnjgsok.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3prjrgtgb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3peabuuci.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3qeienmxp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3yokywatm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ztnzodzg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3baolwcth.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjivhzd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ihoxqfls.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ixbzsxta.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3svkskuzg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3auhqskbu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iqtbbxwa.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mehgecpj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eawdhyjr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xcuznfrn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gmtaeveh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3psecyypy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3yhxhynxp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cvzcejcy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtdygrj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hqllwzhd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3llagidhc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bapgfhom.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bwxxmbwd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dscevufw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3eaonrhea.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ppiggdoo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ykybjvgw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rsljfgge.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pnfpkpph.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sywncewg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3czfwcecl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pfpohmlu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zuysbjjd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ehzksoeb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wmlpsoqh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vmeikmaf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ihrfbuxb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3scrwacxr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oclogumo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3imxmrgnj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3mnefsffv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fpnypnjp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3cwpjkkxj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fhotoqoq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3setzrfra.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ymsjwnrq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vthvpshx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3brbdoemb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wtkkxjff.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iutxxwsz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sukkbfoy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3uqbdjdbq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyawikyz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vtmostlv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3yvyoknsj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rqlzbbrd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3opvlekef.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3eyojyzqn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eorxlhtz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3lwtedvya.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ankffufv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hucirgmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjoofarl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3aefqmyvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoplrpyh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3uhqmglga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tuqidbzv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgtcnijs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kgfbcgbu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qtfeirvm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jhbnuwgo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmshhmbq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3chipkobm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3odzigtdb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ecburjtl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hqqiiqpx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuyemfbh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3akdhddit.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3otjqnnxz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pbxnppyf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xgrmmcdr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3gcbuorps.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cbbvoduj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ngyschin.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ftvmccbi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcrrwkzb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgwfjyzv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3telghsyr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmntmudv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wbjcpqwk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xbxaaxmt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nbqsantn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3evleyzoi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qpjamzjq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzbofphn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3czbhfoxo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wapbikjz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkiuwayw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3neenqnbf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hjaizfyc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3swsjiriq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rcvtanyb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gjdcsmfh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3huwxuyds.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nokmvtye.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ljijnrjq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gbxmzspu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yaknljzz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pptmwkdg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhswvzre.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gjnmdcyh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tgjcyjrk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxtzqrxy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3umzqrnaw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3krcdtzbl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cuecnztd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bobdwlzn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hnglvugm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrfqkvda.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3upckdoib.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3olnvywem.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qjskupig.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yddmibmy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3isfhwgbw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gddwbsbk.html


<!-- 参考信息 -->