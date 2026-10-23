代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ftvluxfs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3nscgwetw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3jpncjzhq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3osqqghou.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ppmciovf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sypbyxjt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lvsutmic.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tnlcmyyx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3djdacupw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nvxjdbsv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3toqxciom.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3nfkzftwn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mokehmwv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bsnosdma.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fvfnczau.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uqqsyxpq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3jnfkoisp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3rxwrhdzd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3qdhtpyiw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ewvxrhyw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qyyzmgbl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fwwsornh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lfwfjsss.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctubydnn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pfpojdjf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ftyetgrz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3krutlicw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqzfklwm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rahkclyj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xhrxbfwe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3toscikdi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3byuzhmuf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rcuvmlfi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ouknyokc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3hycrbrfr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3sqbouonl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tthzprgp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfsyivtj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3adlxpmmw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jkrjzrjl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3gusgwisg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vvsfqjrv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3urdfvtiz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jtyfvpsh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3yfyctagx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wxwybkvr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3xasjytxp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3linqgebv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3fawbbtef.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vkzbxmtl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3dejwftpm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rxdjxbhc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iaqkwkap.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3tdhydhlj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3krtxtylg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gjqwljbd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hadkwhrg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3modjaykk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pnhnbvmf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzfrbnq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dphabyqp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3esehthkx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3neentimx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gdpcmnyb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3vxwbsifa.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3baxovlaj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3gpsnneoh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xulasilo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gpaxkvyw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rveyvwvs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ekmmnddb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzncifu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3fodahnaf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rlutvmwt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bmgzfhmz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nsxtnmfa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ppvmwumu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wdpyltcf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dhyhrzjd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hlqejbqw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fynupvsi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ehsrcscp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yefeketv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukzqzavs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzdpqic.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zbukyfxc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eejygkfc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3oalgvaep.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hetbadkt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ourazuin.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pbeapgjo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hpmddosf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3duxynncu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wswkfzts.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tkoesrqe.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3txmnsxla.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xevrsjyz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3spwmdwco.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kqwquigd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kphrkkdx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3cxufxops.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3jqibuqbn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rkkpdnuy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xgejhvhd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ovaxjsbb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3phvlazcj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3isgmilsb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3larxnvqq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zcbbibna.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3nqnrhyxd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3pfymlfeu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3erszjyyd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3igsudjhk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ajhfnzlk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3erjpbuak.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3fjhsfgof.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3omlrfuax.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rqvifblm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3waelhoiv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cbwzzakn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3zaxprapq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3oyekrkwa.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usnecawb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edyvatzw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkgntfif.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mujnakbi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oeiziutk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3frhpuwcl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bymfrrcp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cifxbcya.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iojsysey.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3spjfgqmp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rcygzklv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nluukoqz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3irglhdpr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmcjckve.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mjfnefro.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3snenkzuq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fizxmaqk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqicaro.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpbnbsh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xzrgclfo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qphdlzng.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3tlnfzvvg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3hunlsygg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3giridmyv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mytjtrom.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bbpzutbr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3coujbtyh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nwhjzbrz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3dgcohujm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hqcnefkh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pswsqdku.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ynvfnpum.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3honjerti.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tvkfcrjl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3grvnstvd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3omfjekeq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ydpksgnx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kpqunuxm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yhuceosq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3zatahttx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fyscjkcv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3irjccfvq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3fcwnolsq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3haenncfg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zjvesokb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwxcsple.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3asqryytn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3krbwclyw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eztxogxf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3pcrgzakp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qidorwpz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oojoibda.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ioqrmeru.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lxapdqfx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3apsgxcnw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3uvbzrmwp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3asibbtnv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3erygcxoj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3puasvtub.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfdaawpr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3euyfaykx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3anoevxdv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dcfbezrn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xgnlygfa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zunwdzqi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3pmcmqkvw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3sjjdfpwn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zlffaffe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yydppauh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3yuauxzjg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3brahephr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wwrdditg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vwxlziqc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3uihdbuqz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zwvbnabh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dzrcmqzv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3urasumgz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iktselda.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3tchszqlx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3oprtzftk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ktdasfqm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mexezltb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bolgvben.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xkmmydud.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yyapwqqf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mxxqfqny.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hfusbpcz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xycqqnxf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3eynvltuw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3lhcczosn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kyinxmzi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wtnguxxw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfntcvtn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gxcqawug.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tdsfsctz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azeqiiwo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pshfihkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpouqvwx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ruwmbnoa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uzwktnzi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvyeyehp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3doyhnujm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ugykzzzf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3odaigpfy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zorznozf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gelpncnv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lwkzcicv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vdidavde.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fmnfxniq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdvqsaqd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gakonzst.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3salwmzuh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qiyenafu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qpecnggd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3uuaufucj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vzplpvxj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ibhswinf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hoxcsrcw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbqnvprq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxfoctxl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krhtewdu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntwtabdj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xtntxchr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rwoqyzal.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ulzagdnz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3azxaoqrn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3plnbhdjk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3aclmlfow.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3moocprbj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3swdzqswm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3paesizfc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrhcekhd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3dqongcwr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3usxltnid.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ssjlyogs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mwjlfppr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3aufjiehm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aipebual.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjaaupbf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmqpfvay.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfaigmrz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rqghmlrz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3yqbuzaem.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rdvmrpbq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ingpllwe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vjhkmquy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3axiltnoa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yrcvenxd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jsqnklfb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nqwoorcy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ynnvvjga.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnonmvyh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dvzuowsj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ilzmpdmt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vturpzpl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ipernkpa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pmlalvup.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qszbwpeu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cvshfkxa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3sclpdnuy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qmiozcim.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hczmblhi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3lakjiyqg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xrvshizv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xtuuiytr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3swnakibb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hdkgybut.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wijewmrw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mamnirgf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qudapkeg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dbwwkwgs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pzgcuruv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mlveqmnz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqhwqesz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwrelsse.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hrdzqnet.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cbsyntyh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qrlmspfm.html


<!-- 参考信息 -->