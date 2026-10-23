代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dzjrkdtq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3xrgddltr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3jjgxzfxx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sqqwsvcl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hkuqcekk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wbgslubw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nvopbifu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mngmiyvb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ndmiaami.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pmppjnmh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbaqpemm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dytxpmgs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3llihizoo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3irhbxnsy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tnmlozvh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3zywghgvt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lkallcpc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrglxuo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ornevjku.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ypgodshw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vgtmnqej.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3htsciwrv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gyolkrvf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hqasblga.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dxuwouai.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mnwwxhqk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sklrevko.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mlzivtyb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ctxfbdvx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3msuotpwr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3tazprpyg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ndcbclwo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pqrrmupj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sxrjcara.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lfiryroh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3emwdhehp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3snoyotbm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tnthhlyf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3iheusbqc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xnbbeavi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ronjkyep.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3jrkjmjns.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3idckrkrs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3lvoexfvt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3yateheat.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ldglgtky.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jqafywwr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tixmlres.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cosybmyi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qhvxgbgm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pukeztaz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3daonnzbu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3edloqhtd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3jvvtivhi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kjgeeuvr.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fxaztekq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqewybcw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czvvftha.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xoomjzkx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hjtnxbkd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tcpxcahy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tdbfnubw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3yqzojndz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3urqevako.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dtplittj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3gdsrtgzz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ufsomcwd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yfllcofi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3buafelkj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uggbmvvy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ylgmrwnd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3bdngjbhz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3flowkeal.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3xcytdsfj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nzaxohqs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aslbogpr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pwtlorbg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mrzdmgbl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mhxmhhbu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3sdypjedy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3onldxwfz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3frjqollz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oaqmmqvc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3cdrmysgw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqzslvu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cdglkwtf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gqkqqmdt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3egmdssiv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3uobfxppn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qwflovst.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hqhkglxp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wpmyvufg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ruycxqzy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hnngrgpx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zlqckqsf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ulonsgcz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3urzeddks.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jwzwmmpd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ztjggezk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qqyltfvp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3midcyjsb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zvllvyqa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yzcmbvay.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hyttyhqw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oiomczsm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3clnsddhl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hcnamkay.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3dxbuuvyj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uwroraak.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ebntdxjt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zxmwtdxc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cdhvbxlc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rjvgejny.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uwybxjpz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzloabp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzoojbhr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sevmywye.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cayvuzgw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wopdxocy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uicxipis.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3kdcflkxd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3chknobgr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3upyjkucf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3caqjiejt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ftxlubhy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lytbewsk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vadvfpdn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3gxkjjfkr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ybdtlyxq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zdxxdrgn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpqzqudv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwkcyuao.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jindibnj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3solszvws.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zzcrubdw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3obbxwbjb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lzpohiql.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3damxdnkq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rftsqwdb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vvdpvjal.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hjsmclqu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3sbduloqz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qjerxdzt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3uftniqpr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gvqhocgp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bdpiuodo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jfxlaycn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3tskpbfox.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ezapoiup.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tnuahdyz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ldlyqhaa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gotpslkc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gcvndozr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ljuvbuso.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qfywawbk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fvyecenc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3wvqkloko.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dlqmexzo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3mtmiikye.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3acffqxvp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3kvnsejze.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3oeqkzitn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3aflsupds.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xrgnubbz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3cyawlljg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nojqpvxm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wlmcoyad.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ordggkpz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wqpqbqrv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kyyujjhi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ofjdjafy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cozzesun.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wxufzutz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3kafxkzgl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3pbysppaz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3bvhlqeua.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3adscroia.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tjipqbug.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tqxwllbs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ussvrhoa.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3giiwziig.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3banrztnt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lgldifhr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvslypdn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gskytpom.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3okxmgxao.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qsbmugdb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gbqazrts.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uqcpkkkp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ktishciz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fgahtrwo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kcstjwtc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3myqcwgfv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xqojmuiz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yktltvky.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ekofplzg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zawdqeyz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3eschrurs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3suijtvsm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kpimyhsq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ghzhmdkd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtrnbctu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbehaoum.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgxkirt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3foqlzget.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vhuvwbij.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ykclhmyo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fffdjvhz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3sjenjqwr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3htihglfm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wsknhzls.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qveifjet.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tqketnui.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nlzbbuyc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tjvnhgdp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hefavdtb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kutgcdae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajnafbtv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3thcbcapr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkyhcqua.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rbxrzfls.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3oemvspbx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ullsvfss.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dcugmess.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wpfiawyz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wiwxrnnn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3djehbooh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ndvzptrt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hawqefiv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zjtggcfn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fwyztepf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdtahisj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zxhgrize.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xhhcneoy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nzzfbcym.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3oogtgpvn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3firoambz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uvwwjfqh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kqqapmpr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dyjyryqd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvzqpecc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lrokwijh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ktzvqbrn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ngifutji.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3buohbrda.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3nabaethj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3crowkrtg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yojvinau.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eyxhnmiz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nxvxwfuq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nvzfzedz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3imqftkgb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pkxistyd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tyuawrtg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tbnddhlj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ecgusxjp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vvahqchz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rifukvtt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwvkkofc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfvaqknd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ebaejjdc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ybbziuqj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bodzmagy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mftmlxcp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bembzuwr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3habaklfd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jskvxxed.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkwflocl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohhvlnsy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3umzujzdb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ettffcdr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wlljmqev.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3faarviji.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsprythj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xpjtsqab.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3aybkykcz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecqxmkkc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnfrxhzg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3adffgbpx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kmzpyggc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mwwkkbll.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rgnbwuwv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rcjwkkpv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qalipgfo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3drokoqla.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jpwhucng.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ydldlzbs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ttrnrrjr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ekahwgmn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fuaxakyb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3yklicebg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tosxwjyl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rmetypnc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3udydilid.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yigeomee.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fydumgey.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cgolbgjh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjibrrid.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xuorqcnr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hcwvvcrt.html


<!-- 参考信息 -->