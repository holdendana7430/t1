代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xtelsngu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wdxrmrkg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3herqkjzr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3csjzcywv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ejtmilts.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ikuhlqbs.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wwryqzsz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vupwzfca.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ocnhhcwo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jxfmiwwr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wpdenanx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zanenqsm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fuplgjok.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vwwwjuxx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3tohdlojd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3uqbiilrw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tostkssa.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3zbnrfuxv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3yyhowlwm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ocerkgbw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eyxcsdyn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gaqmryss.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ihoupogd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cuwszcnz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uxguplcs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kutgwgdo.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pvnjjbio.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3kbxczpmj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3sofxghkj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ftqynnmp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wslebjro.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3whbktcbn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ecvqwmeh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3kbbwmspj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ftvwtbbr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xnarczit.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3pkcgezik.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oaqjwhgb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jivhetff.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3doxwtaii.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ntxlcwrk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cddfglhf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tbstugsr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3knpdonuv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3twynyubh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3iuimlysv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3uejtntpd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ursjhtxn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ltnpyvzx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lrypxdvv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gxofyegw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qyemfpvd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mhkkmoea.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gqlscktt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kmdruukt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3dyjrtzci.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wdnqxeww.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3upqdhurz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tacbqxjh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jxjuzdck.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3bqbbnuds.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3smmqjciu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3pjvwmvdo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tgmxzqnf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vcmjozmx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ondpbhid.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fjqguzky.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lgvxcsjr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dqbeieuu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3spsfskoo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wgubusqx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3frilcnmb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gunovcvh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uhujsxjz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oepxdbrb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfbysl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3merfpfzo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3mmxltddi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3hinaqhgn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3laihnoof.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bexlgqkh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ikwlqnnx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dpbctvea.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qhksrngq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wvpufzjz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yjmyymsx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3xouydisz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lsiytque.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mcmuykzd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3cehnotqs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kszinmqg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vreijdln.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tvwfzvdq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ojozzavx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sufclohp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bvrkgobl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zistmcrh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gmwofhgj.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3xbvmlbub.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ycgfyleu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3czprswxt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eovnpfia.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ikckckqi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ozfuqjom.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sglzjvyr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3lehvtbce.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ndxqcvrp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3nukxxyqc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3olflsbrw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jqprsefu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zwxqaidy.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3beccvplg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pwemynbh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rbjegsvs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jhagalbz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cookzrlu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zobtxqlk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3yughoati.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3orfbftny.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dbzfutgz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iqorxube.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xyhkhbtp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hzqamjxg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3rkrqqwqr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rfzidjsd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nfutsdaz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3itluyffn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ytsylmox.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hmcikgid.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gkxikybp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jvrutfyb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3yustxcdu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jfprzube.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tctjhblz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fbrhymed.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3pgmoanag.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jwiazwdu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wqtlpjmm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bspzpwgy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ulgecyko.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3huhzbyjn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3cdqwwynl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkiqqwyp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3oafvubmz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ueqpbhyv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3baumeups.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vxdrrmny.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hwftfeiw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rhggjcru.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mdwzeskj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbbbimip.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vgydyxbp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3wjqytosl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cyakswzh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zqkpumpb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rhcwmqjy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iklmtccc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dshukarp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ntirjqmu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ccxjiybr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3tmgiyarj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tcwxchah.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3drhzlwfs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vbqxruxj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3voeisosp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3shfkbmmq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3pqovvfdc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xammchtj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tvcojedz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3wmojmman.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tktxxzma.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zcuytere.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3pbtrdsgh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3civfaohr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3vxrpwgxb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mcshcvcz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zllyqpij.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hlmmfthe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ztwxmjyy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rijhseig.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hnpwudgu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kpgdyzsa.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hyenrhzu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ssgmctdq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3buwdvgej.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fycdsrqq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3adltszrj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fndvdrkh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qsetsvwn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szsejidj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3urjtenji.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3zvzguswo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3agcrybey.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ukmllbyz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3enzjrkus.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wmbmjhth.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3kqjyysak.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ofngutsa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zrxmbicv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ckepmcfz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ymwpgufe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3trrdankr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3egbwrucq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mtxzhsyc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3opjvjqzc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3roicfaro.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zylsjlpp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hxlautgm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xskbyubk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ptisyhyf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jghmknlv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3tdwzzhmj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhokofu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3axtpkpjf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ridtqlqu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lnhcuhil.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3pbxvepuw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqsrhttc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zgmgwsqh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdszfhrl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3skwafage.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iazkiucd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3rsbtdjqf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mtaludkg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qbcxhzmb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jjdgdwwp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3xyqdkdsb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ypvkfwpa.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xofcynrs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jixpobsv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3psboizab.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bpfkrzjn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nuckjcvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uixxsdda.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bphywotx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctmuodey.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3okepdzdq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3cxdlzsah.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btkzrhnp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uoatjktl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wmmbmfsl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bcvvrpmp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ggtmedva.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vipeebwo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ypfnnzig.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ctmuftyv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jljjaioq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvbiobcb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hejkufuq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3neuolrxe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wmcbmjjk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3krzpnlbj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xauxdnyq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rbvzucqu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3cgkslnwt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ipqtnqit.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3orackife.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqisyfdk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wchwhvnx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3liaxguio.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gawccmph.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gmnsuyyk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3klwlpvsw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dugwyzpk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3simlfjji.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysogtdfb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ynymmuww.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvtdqbhg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wfnetcxd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gsqekdti.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dkrtqdrw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vyvkkudv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3avvoyvhm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qdpuaygp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3owubuiir.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kkvkjvpw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyvuprof.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqjvdsbm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3imtjuofw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3swaehkdo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3esqrbudw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dprjzpce.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxhiddi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyrbfxvc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kavdhjnk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ibkdncyn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kbazdcjp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3oisfxqlp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gpqyxzhl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vhtjphci.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hqgixitx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3buxfpgiq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmdqmjlm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3txyydftn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tsfgkgdd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fbkjdoib.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3yametppo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tategzot.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvjabaon.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qxhihhec.html


<!-- 参考信息 -->