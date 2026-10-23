代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cvwmbrwp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ifwsqtnl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3sqhlknew.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3nkgcxgur.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wvhvqmtf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cboqxzdo.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3arxxpqpd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cfppivrd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3noiwrzur.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3iflpwasw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tqybjyqb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jzbxeidb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rbeowweq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jjhfqcyz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3fggwgokk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3wopadvei.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pjfibbnu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rudvwwjm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ebfzqnaj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3punhmpci.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zohjbssl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xzjfhfwd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xmushrrz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bjofheer.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3shkoicwu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cdnebdog.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gsgvnesq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3zeazammz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtevxvrh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kkqrefgr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zsdewnha.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qnovipsv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dycvemnk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jutzsxef.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vaaspoax.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3pnwwmrlh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lvqwvgji.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3akmqgnan.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wtpzybji.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wcnhwjwh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ijycbimz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rxhfigei.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pdwwqlhe.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zwkyjbsb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qyfgraqm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pglnztxm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dqleqfbp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fyscuzmh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zxuldiht.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3whnxrnrh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qsxsiicr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3inxosvxh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yxufgeci.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wqppedat.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jpkeshyv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tavvtjhz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3zqorvmzb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmxvive.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3taagqmqh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hslzdumj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3xnxjlfxj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3sqxnzcxk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wuufoxne.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3smpjztvu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3pgjmcrnx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhsxaem.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tkkyrakv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpxentx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jsoasizn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3qdnalqug.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vlncozwz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dnvoookv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxjtttr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yklzlnvo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vvhqglmn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3slaokkko.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tjxpkuzu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gosohvly.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ztlyqfpy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhmkjbak.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ezpgxphi.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3afzxzbwg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qejaepwe.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pigggixh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3inadgmyw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzfniina.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3bsntcrit.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrdkihb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mwktsgwe.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3recwsaby.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xvxxotrm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mpaieynd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mhuwajyx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xkernutw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fbgjajid.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3pebpyphl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ragrtzks.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ydfwlrvv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oyasewok.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dgrzpycb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3nkqbrxoj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qagjrdng.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eiehfhxd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pfwvfnze.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3mjboyqrw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wuepxxue.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3chqtcqpc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wfxwhmnw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wwhcxwqm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xjpzgzdc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xngaubxu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iqmcsgcu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jlruecni.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cwideobo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uneoaxnu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cznbrhfr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vwqhmedh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3mibvcmaj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3inwreiqu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xnydfizv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3stnjuhej.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3oavemrwz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eldtcgno.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3qtnfjiux.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rbscnnbl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3tpucihfs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xwzxfgru.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dnbuqjiv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3somnplbe.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tchlgcob.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3eowpcqxv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rklmhqmn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yyqbukea.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xztlzvdp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3umndakbf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3heictluc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zftedtll.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qwgqplwy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3nzqoqkko.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3tqaljhox.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3mbzdngdw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3lzinojpq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cabtlhrc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yxvyrztw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cobctyus.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjqtqkdf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3twikdjtz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3juspmlqo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezttlylj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bpsxasol.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lklonkog.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qkwatwcl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gztqiece.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sytcsmqv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fgocaxkv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xvqngdmu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xqxbuhxg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3quqhzvvs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rpnogatm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qvwtgtwp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3woywwgmx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tiovfcpi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3klwgjelp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3rsvtjbhp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3symvgmxw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hdrujrnd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3bibrfutq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zrdkukfs.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oafpoeps.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hxixytdm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ouejyvrz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xxaocbxm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jnijsrqr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3thvtragi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tcwxorvo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3tmwaiqez.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3mynwsxsp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3npwalywj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3hdhsqjuw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3kboimjus.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3knzlwkpn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mpvbnfni.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ravewllm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofmgbbng.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sdiudjoj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3obhzbthl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sreuoznu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ovkqopcx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zksyhmii.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3phjczwfu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3gzxctjqw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ylkhmyog.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qypfeuoc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mprguesn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jvoyxipy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3anhvcqbk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3uqnbwupm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3addqauuj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vpmelxbk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqpusrtp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mjvoztvu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xblklxwr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bdbbkyfh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3hgcsyzxa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kjmnohuf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3dbrspbbw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qsromgia.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3snynqtay.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bwyganyi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3chsepapb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yzzncogc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3vxqummov.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3xyqdpgrp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lcjetpfk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pwmjxyud.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xjhsecrj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zriiieak.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nudxciio.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hjhwdkpj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydcugbsa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uszefrqd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rvgsgstn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3uwjzvwyv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyvajtq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mizvuuut.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3twohhldh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ljvxvkfm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hjudteoi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tbxpevft.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nfpiglth.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3shcdtzrp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gfqsbncf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pnzzqkuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixpbimjj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ibvyifkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jiapasnz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kajyueob.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pilautsy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3suqoolop.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ovsjtkre.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kqvohklr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kjnpfvvl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zzozxfxg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3eulxsbci.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uodzfsaw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wksgrnqd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lwunvois.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3erjsftqi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pwzsatus.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wdxbgfhd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fkskdjuo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3eoonbwxi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fpavdyik.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gnnfpxvz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3eqltrdtw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3crzwgbfu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uamqrocd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vepiwjwy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovxzfuqo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oifkpubc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lqkqrgsq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tspqwmnh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3svavgteq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ktpseaip.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xzdinxrx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bybvnuoz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mmiepmwx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sodwgkrn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xptytotl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tmpolmlt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ynuqfnck.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nxhqtvkb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hdrtxwjb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3reflsfsh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ltjrnbkj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhipumoc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlnmfam.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rnsdstfa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xaqimeai.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3uzcisxhn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3buhxymyk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kvbelxsl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mynyxhgj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vnfyfjhc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3skclxhgo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdveegdd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3neybokxj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qqewzjzz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3spvssjpy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3esqeskbo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzevwbel.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3otrqihxw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fdnapgbv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nzygfoxw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3beegfyqr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oecrrsjb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zxeubpsw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvzevpyv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzvckwt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3inxkllas.html


<!-- 参考信息 -->