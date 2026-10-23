代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfwvwsne.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jioxnjna.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ulgettha.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xgodiojl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ibspbmor.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aduhbwkb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aoswaola.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3blmcyguc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkqcmfb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vedkqmtv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wjymvjtu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3pnritlmt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3jusyqvjh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3nmocggaw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hqhdwrrp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3goxsmmhh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3uqqfcyva.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3emsqlrvh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nmfpgifu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fkwwuqpk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zfrkoybh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xqoxeylj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cnqrfdnp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3twngfpnc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3exjtrxga.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lbhgmdbz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kiwystfj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zouolpvb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3eeawvmrl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vcujmfxh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3llqypywf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3haaltvcr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wotzdziv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3flskvhpn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3mjnjumfk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jbiphnhi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bdmekryi.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tocbbwdh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrkboyh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3luluqnxk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jkevcqro.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nqoewqyr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3aggyajtp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uhlogjwn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqivtcd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3aqwsykbx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fgveovmj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tyyesjuh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jnucsncu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3eauxzhcp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3abssmmna.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wdobvuvd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kzljabrd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlyghgw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tmcyhrnf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lpybmxom.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kkoooflr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ykonrdkg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zeyvpicf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owtrkpcc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pchbeutx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fiempzis.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3gsejqqwd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3krfomcte.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3glpvplzm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmtcmfvv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vvkzcncs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qdxjhfja.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3dgmwgdkc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jdtyssbh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tfrlwuyh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wfnbwtcz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ogzagcst.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qguzggmu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kedkdhld.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3jvtfmbhy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oxatunhy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zigvlknu.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3adjqfulo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3scwbavqg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hziujlpj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vircflnq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ksjqmobh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3llnhtyom.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3rywwazgl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3mxjnzkau.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3arxxaspe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hdprnflw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vgeqmxdw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vehhoxpo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rxeeccjx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fzwppltk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gbxqhsvn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dpjnyocg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jyiurkxc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zpoxniqj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ivknwwjm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xcsnfmsn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wlypcrva.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nobcnvuo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3aycszcpr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pwsglgfj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nnnilwha.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3dpsdhvjh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nnniuxjx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qjeafpwx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ygsclvww.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yyegcecc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fkckbwqw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bpoduaxe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wuismerf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvmtwoo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3udwxxdfk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xubyaltp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zqyobaaw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3svhrphsh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lavgtfvl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fulbycih.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dfvtqknq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azyywsvg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3frtfzhww.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nhdeufov.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pkzewswa.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3irqvnxni.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yluopvac.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lcikavjp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcrmzefe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qewgvmtd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wxyxmcrs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rojvpzxa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tmehhjjk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jxzxecqe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nhmshvxg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pudpxwim.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbfkiqq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wxvrappd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eihodxsm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lovaywrh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hrxtsohi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bxboivwf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cmsiztfk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3epkqqskt.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ifvkofca.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3cszthvpt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lbqumxqa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rhdtotek.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3asihbuqj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qexkjdkz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3thrlyubq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kldpdcnu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3pyhmemdc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vjsjryue.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3trvctrhs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3khdcrgxf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tmjplsfh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jgnqggmc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3oojupmet.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3uaxejjua.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jssmtsec.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3dlunrdbr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3swflffjo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3elfnxkjt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ggrygooh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bthbajxe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rclwigvo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3heindysr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ebvegddn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rtukpedx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3muluydbb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqcfoxpp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mcyghbxq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3avqtxawl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3bqlocbjc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rxvsmodz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ncsntkkk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kfgetwdq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dvjvbzhh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dtqygqzx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wsprqqbl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyixaroa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3huhzzpyl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eobhgrdb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rqgrabge.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3bzouqmxa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3emgzodik.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3vijyygxn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vbbtdqea.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jnkamkpi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3qgitkcqv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yxezybdt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zcjwfopu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tmunhhsh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3izwuynwk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fhegimmd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nxylmzqz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3itceahek.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3brxxbpyz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3sdnzcglt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rhetptie.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuivaflw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfunxyn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3eypncjrv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vedohnpl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tzjsmgzz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vqauqfkm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xerxzhul.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jfbcbmiv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nemyjqjl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3hwngxvlc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hbgtejtq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nihbsfsk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rapelnvo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zupdfhsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsklxyug.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3gmqrbvcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvivbmaw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xprlcwwm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sgrhsupj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqypksde.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3stmerxuk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uibemhyj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jjeqpcio.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uqrbwxaf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3owepnihp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3epjbvbcc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xbdofzwh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3iutlooum.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xnjyywja.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3awhtlmnh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uppkrpyh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ppicvdyn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qsfjrirj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3weywnaxw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hfmsfkfa.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hyobgoap.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rcdkmmjw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3padasjjo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bpncmijk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxmilmr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rzuszlro.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jyvjsndc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hyezadhf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jhjyhlov.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gpsegroa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xyewjxnc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hkkikhmj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjrqsxhs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jitychav.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3alkfgtaa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jdfviywg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3oprurufr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tiphhwfs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3brobkwmw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lentzcim.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsfnougs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxbqphph.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxiyyun.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jszxnpun.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tuvsxsmc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wesnlido.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkbdarrj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tjitjeyd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ifcufhwf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdfydgcm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pkbqgtvx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rtbdbrnb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3idiavbos.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3fyiauhdg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dveieccm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nusuvlma.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sfzyffbc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxbetwfx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aqklnnqp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqvqqbxo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3izumndvq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwqczhyr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rbxsvgup.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ixqyoabd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kehdcufs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tkzectrx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ufhruirx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cgtlsqwm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jvgtfqdv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nmxqwjlu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lzslmsmu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kifxbkgl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kmajuufk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hgwajjxq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ztndkssm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nvchqeth.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mubbtvgl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pwkmlmho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zmuconzq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmycfrkx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vpwwksxa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3yufdwirn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ivdecmjj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mscblbie.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dlpafyop.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zwinpzkd.html


<!-- 参考信息 -->