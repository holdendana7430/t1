代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2aixessdl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uzmpsgan.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2swngninm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2rnrbnbjf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hzztjqxa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2xnhqnuul.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ikkdmqld.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2stmtdfpc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rmcblgeh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xgzsyqks.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bonyglmb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ulihyupy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hbgrvyoj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ygcmdwpw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2gnorbces.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpjtsct.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ikzdgblq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2aowuxjwg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2obaigixg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2eaacjihs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2syhxrmmz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2bwblidsq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ngouipkh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dadedxjx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2reldzudm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbupwsao.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bchalfal.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hiyebhjc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hmhkuaib.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fohecrlt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2crwcdqya.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wftwsicg.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2egnjjocj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ezfaaprp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ilgsbbms.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2udaegyvg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2orkobaox.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ywyudzvo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2vurnqgyt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2fjbwhsbw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qqaixilr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2wvyoyijp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cdzhqzim.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2bfhdqkgw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hsaweavy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ldibflek.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vhkratli.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2brmtkhgd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2gbmcclkw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qmwewbta.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ngjonaib.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxbuujm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vaolrwdi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fkyownra.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2jtblfdqr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nvbxkvgs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sxokaeqn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ohzxqvrd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kwkxkdjm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yjlzsrul.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kcdfagjn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkznfywz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qtpiacwu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2etceovzm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xuqzaonw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ezbrypuy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2snzsbhau.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tgjevbvx.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2knofgdop.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2thqxybrx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mvjnvkka.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2swumcvqw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lesgodxg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vxfzllmf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2havjxten.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2wmmphnjj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kkawjkdn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hacsqatn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rwaljyfz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xrhpwqvm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xxijcyms.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2afljmnej.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ikfotyap.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wzspcrar.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ptqxxoyp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vciclaeu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dljetnqh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqkhohdj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2lvyixqyn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bvabfivc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tfopxxdu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qdmxqaqg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2fvtvftfi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gsfeyzzt.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2sgtbggwm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2svhkjgsj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uajttuzq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uebswhyd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gbvoefvq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rpfxsshg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gwgbsgzl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zhokijfq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2osuwoyow.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bweyoorc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2psnextsr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2uwmdexbv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fdpmemfj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2btyaygjj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vdgxceer.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2afoxwcss.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jwhsfsfk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2cixuxazr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qimoxxmf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wxglhemv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ryuyqoia.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eippwhwg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nixqhwrt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dtlvhppo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2mdldlfot.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ppjowlwn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2utrbjubd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ebbrsywz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2dalwtomw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xfpwxdcy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2urejpuqf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vuysrecj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2sotkiyef.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2xwrtwcck.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2vwiafdnh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qearxmxe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2boszopgx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2gtsmiope.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udkeoftc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2voilmbyt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cfvwttwh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lgmyesdc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fssmitow.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ppjrfitz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqeqnzee.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tzlvjipx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pjeluwrh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jwrgvzop.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxqtsbn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sjhedauy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2aoifwbwd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pluatddk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2dwxfqrvg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xxdvahdd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rkkikqtq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mbgqjkaa.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2digaqrdj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ldztrbfj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ggkltrkv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bymdxatk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dcebxtgk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fwktfxmg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kiuirzur.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vhgtvqqf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jlvtpoyo.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dimtgxkt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vxpragit.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2cfcpkmas.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2htsvvvjd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2edppoqvd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2odveyqsg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xgevikac.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gnekvtaf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xstdyzfu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qnnyubcw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wokklggp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jrqekiyz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zvuepbdk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdtohiu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rasjspou.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nqbpltuv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gzmxqsbk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jyetwlgc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqoehznp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rkfzshif.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2dgdguxzy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2unicckug.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2oaobxexz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nskuwehl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uqretmof.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2esacpuoa.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2czizoqza.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dzkjlaxw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xagjvvlm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ltufvqom.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qekanhvv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fwjtmzch.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pifkncbx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oviwmgho.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hlvwqouh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qdectdyl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gcgequyw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2brhdagfl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rfxclfpj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qtjnwqlk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qbmlkhir.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rwpfsoks.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xewegfaf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2voqupydz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hurdzemz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ghosjrsl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fzrkhdpq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkmpcemr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pcmulicv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rrydxasd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nixmvzsf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2zqbcpora.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lyezaeoo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mgurhzmr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jogrxgqr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pcpmdfek.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yjjvmbqq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2agvkouqe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wumuutug.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2xtvnvbqw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gjerfpnq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zwusoafr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilojoxtk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rzoqrjuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbufdifj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mfjwaodb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rrmvkupj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcjqrcid.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2trwytlqz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tmdirpha.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qvvmkdwh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hedapyzf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xajsmqat.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2augppryi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ajxrewda.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ngtvmjul.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kdwlbppy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2igqyznve.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bmivezjl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2inwviwgb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xlekwhls.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tndcuhjg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wadfhqhw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2offyadgg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zrvveeha.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlsbsesq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhiqakj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztlfxtbe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qhjeuxbh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wqbxzvnz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2olqqtnlz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2eozwelzw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2turxdghg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vnzmbmjr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2edwogkhg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oznqcguu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mfduluar.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2plxvpqxz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2svuombcd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2msvrqcph.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2phcvurzi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tstdeqzh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jiizhhgq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2yhituzko.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yqlkhayn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jtdyxpps.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2thjyhgox.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gxhrtrxp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2kcczjrcn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2yvshadvs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uwngbpzx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2atnggfmq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nntxwxsr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qfrxvcdy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvxyawqe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2figjnzkf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mgztznze.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qbrilkxo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kucjtavk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2efkeovwv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2upcmprii.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfbfdbdk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dzqhwpif.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fhmwihwa.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hehmvvnh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fdhqkvdi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fyrizwjf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ylwxusgh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cgsjxyyc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ogjrreji.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhuiwia.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fivvriea.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2petvqoaa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xteffyct.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqpdnqqs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2oqdxgmmz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mmggpkhh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2frosnywp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2basfiwyx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhnlnfwy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kmvmowof.html


<!-- 参考信息 -->