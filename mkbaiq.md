代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qsxfbpdh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bufklpzw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3hkshwqtu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjygyqr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3skdthisp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3udfiwusr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bmrflwjx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xjibyhqg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dxzmrbgx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yskkatnn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3zzwlbrep.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mzgxiyep.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3shyabafi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mkvjavot.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3biuewvwo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aihjzald.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bdzdjout.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oxumejwl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3czqorjuu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jwfxhemf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xxcagclg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hxlgfuyw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rsegsmlq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3beqcwisw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mhfubbro.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ityftyiq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3oxeigyzc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lmgddoau.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zxdgxtie.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kensqdfi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3msvprewn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3efpiqfcd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3dexhzvna.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tiajkhfl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yqhjpwxj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zyjdhflh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3cjawxmka.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xnioatsk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tiktezsj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jsruyinr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wrhpxhuq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xwfymphd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3yecpkdqr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mlnntpfc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3axkivlzq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vnfwsqky.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zigozrur.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kqkyrkeh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aijxwqzq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rasrikvx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hojemihd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozaomxls.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ejsoscwo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3entopeem.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3sfjtqlue.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yluzjleo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3tpqguvtf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3zcjxmfeo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3yvfikllx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gyigzcjw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3voxsryxz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqfjibpy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3bwvytnmk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ammvejgw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rbvznnxp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ebuqlqbp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3szpqtvbq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tpffiqvg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ufpszgbh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yvcdogco.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oeljlnqv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3oyjuprkf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cuixalnu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3khjonaso.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jzlkylrw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3oyjsjgqh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3tmyivlqy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qtwdvqju.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ilvswmzn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzwhcpv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3syjjcckk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ttfpwvhw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mxrhfgji.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3goutdhqi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xdgdknhk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qkvyqvfl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3boizdmux.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3apgilzdk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3racyzjun.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zjapgxmy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qzikpsxq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uasaplyi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jvicspmz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3iyhdtorx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xcqrdmip.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vzgrixpy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3unkkmdvt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xgwwgfsz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pvayucnk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hawodlvs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gsdibcuf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rkfoffhp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jytibxmw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mfspxrol.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hljptbcu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zwoscwjc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3okxgpyjd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdoyfegf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qenzglta.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3geuydkvz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3qjidspvz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ruvokens.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3xvtqluot.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ftypztaf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxsjjbzk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3srczzoer.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3glxempyx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3okensiot.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzpzvrtv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ehwybsxx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qzkqubzo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iltmvfug.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfbtgrvw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3awnymtup.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yarahqiq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vcdzkfyh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uuhjbtku.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dluagacd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3eogdkker.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xktjfpxm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lxwllksg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hvkbnlzz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qbhdxuin.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qpkkltew.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3icpyzaig.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dajeheyg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ulktioxb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3flsgywpw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ltxfehdy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3oojeutje.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mjxfbxgy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ocnpiujv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3imubigof.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oniywybr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xupxfbdq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzonucu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3iuywojmc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mvthaamc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3koxybhth.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3yananidc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3vcjvzyqr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3atjfkuwr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3pajrqzvx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tnfuiotk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jhpqqndl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3iwiftafg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3swhhrzrr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wjvdtjhv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qjyfjdcq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydgovexu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pikfpvvh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mrxdnncn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3otaxdgqu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tenrcpec.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3loioxcav.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pocshtmy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3lbgnqcmr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lfszspqn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3crlauerm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3cmkwrxgv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xohuyfzl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3udkdzmab.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bvkioane.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjsylztd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jnlotgxw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vsinvkmj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ievvgmfq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qustehqz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nxgsrnhb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dqbiybpy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vngxxmue.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3aqterpwy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3bsbiyyrn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pqbiawvm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhhqjpg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kbhbgvlv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fcodpijt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ywjuqghu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3drxdypcj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jjhzcbik.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qndulcom.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qonbvdov.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gqtymidv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3kcpejtnj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rrqdiywm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qolsgjgk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxzjyxiv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ffzprsif.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nlcmbimy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dltwefnd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3grewdfjg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ncscemwn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tnuyaimh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cbiiqkbs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3njbtfksl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gqwdbskx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3waliqeft.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3jmwutmvm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvuyjln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toetomvj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fwlajhhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xaijtsrj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3anyogmug.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ydyqchnr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3cgzplfnf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cnsvjral.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3petbqsuh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oypgdsly.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xuutssiw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3eyabmitd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ozjzjpcu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jsvrrijq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3sbhjvjdr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3qxjoezcl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3acafzaod.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wdscdqdr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hegyozah.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bygzymsn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3rhrizlqk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3slafjfgm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fvhiofdy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bjdsgrnd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ufdwsyah.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnqtsytx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fdmbvbqk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qrmaxgbj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lewwhums.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fosxiapt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cjpulsjf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jjkjwhvz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uyqtpbty.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcvpkgph.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tengegss.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nncuukju.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uiymrivb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hnabqkpp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqhvijh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gldbubdm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3trotdbbi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ecpjctsg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3blxmydiv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnfkppqu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kztlxrud.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zaboaaxx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jepfircj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3byvivwbu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3twstdxby.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3dzppnmld.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgqbhtx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bwkyrcxf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mxslcfvl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnzvrzeh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3taxjmxzx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mqcjaspx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wpocdduk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdttkxdr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3znhkrifz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3aueyjkan.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hireeubm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlhklyww.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zrwwelks.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuveegvc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vvskksls.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3acuioscy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ccyibtle.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ieooczll.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3yxelhxfy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ndrdossx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3koaatucm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dcnggutm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wihxddqs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xtonpmny.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3oqrqpslj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cewdrcgk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3kzghmnqe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3yfrfrgpi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zpsckatk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvrtdsmi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3igdqssvi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3txirxlhi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nnbviykh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmlcqkg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ykasywjj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tpnhnybg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbjzzoi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3phuubsec.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nbjqfujr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3goviprpv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mokvgmdv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cnqngdvt.html


<!-- 参考信息 -->