代发 wailian999

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gbzzflzj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ansnogiv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rchfqzxg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kiostjym.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ixlcvdgw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aigfwevn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xznewwsu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yywdrahi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kdfrvppo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yhytpoir.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3rpwpbecu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qrdozrxe.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dsehyntg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ndvqluqu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sgiyfaoj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mkalvgjt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vauoubvc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tukpwrih.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3sghbywbj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3fuhigwmj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3jxesxotn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vfbjpnmo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xdkfajnf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3yndysshz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xlcxyrma.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3gnfrjnvz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vneubama.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kcttxnyv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3socbnifg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wcvrzsuv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fdlgwwwh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cnuzscwh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iibiirow.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhnugzty.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sazjcbgo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dtnpqnhu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bpudsnei.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3phodvgdb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mxdegqzh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xnfybbie.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xdbdxcjd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3azvevqhv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdxwber.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3eekolgql.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ncncbqzd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nnlvjitr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3egahudsc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3txsgiads.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ojokvxgb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ckkglios.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yiwzmgkf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yhwiuvce.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3mgnplyaa.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xyebjxjz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3vibbndep.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3glgyjyzu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxukoudi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ycdymrwp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3tlpudloy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ruakknyg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rplwmcwn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ccjyxckv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bfahlefd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pqsgoktr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjtfbirl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hxdzqdfv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wgosqabz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ulwqkcix.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhhrbnu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3taftqxuz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zhrycubs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mcpttqxa.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3tknyhwdy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3fqjzzzcc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3wvpqfelf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3puiaspng.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zrfhkodq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3iqxewdhc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3gmwmnzpd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qgswgtvy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3tlsyihbt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ojenpill.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ceprewyd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nxhbkpwd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3blsqhybc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rawrxsfw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ixjhmkyi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vtfpxdrw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nuiwsels.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xfxyydxu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3flmvjytd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3nocglfvd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rcspjcyu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kmgacrqo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lgwefmwv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3matovbhy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjlutdh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3mhvfphyx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xqmulezl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mxubtaxh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jnlgoeuc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xyqatkrb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nymncbwo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wswgpwvb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xartgwpw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ywhbzpuv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hfpmqbtt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xigksmxg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ivzegbyq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pfhozgdi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3enpmeihu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cjwnftdf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vijxcwtv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3szfaikra.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ewezhfoj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vduwucxd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pmwhjbtl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3tlutrxof.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lhccubcu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pgfzcufj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cflvrhyo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ppjrjstp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qsdvomep.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hrtaoxeq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3flkkiiwr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fymufhrp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rqhsfdyw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3loqoipac.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xnsiwmrd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wulgvhit.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djuceimm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xttyuqbv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gcpipfcd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ntkqgjzd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwczmlyv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3oafamkzf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzlgzcjt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ktximnaf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ngirzfwa.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wsbmxqwi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qbwggsby.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sticnide.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zefsjiry.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jotbpqem.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cdikiofv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kcfvizyd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3evbbgiec.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3osreemef.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qrwwfeci.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3veekmaiu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wrtglcxd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3lhnztyfr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tezycfgh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lofkjbls.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ldjttson.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3sugexgac.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3oryvggpm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3elgwgcck.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3pmzacwjr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3suwfwmid.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qebcickv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vmrqpzzx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3koysrmnm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3abhqgkxf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jjgnhxpi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hllrsaqo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3kargnxxv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3xjxkikrx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ymsbnxbu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3nhxfjkfs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3oukghbsj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ktqfmpdc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3aduixixd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vsxmegne.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3twseexue.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uskbqqzu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ulrjtnhp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xzbgcnpf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pzlyoudd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ozjohmow.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3clincwat.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yionaijb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3tzkhtepe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lktadwoh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3exkrrjjb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uwisxxbt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3drxmvrtg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dpzedbpe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zspwtklt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vpqjocyp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3obyglade.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtqskfha.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kdysbjse.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lzivndqp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xclbehsa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntkucois.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jmyumrbn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xkltjuig.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yytmwqty.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hilbfost.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uupuersc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uupwpvnz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mrdvouvl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ybrjkssp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ksojnogq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3anwdxsss.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3obpuvuxv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aepbvlzi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wcfmyifp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ozlqqdqq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hagqzxme.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xfpohnwu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3fbrngclz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdtpsuph.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qmwtkcii.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3objvystk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vrdzakqq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3plvkrebb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tpzpsrvr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3scxolkhy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ecgeugqa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uluywogs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xhiewuwy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3eawjukra.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lurcsoik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsjxznvk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3yoaaewea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqpacyfq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3bdnioati.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ckkubwai.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmeclsfj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zvevzcdp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cznnwobp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zvievequ.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vlooyygf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3asdubpro.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wyrgihkb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3mtsflavg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3iwcwehej.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lwjnhxcy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yrupoigl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zxrzvony.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bjeaajcz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jiarnmyo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hroqjagw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lkvjznzy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3dftodmoz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ppfvnhls.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gjhsubvg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksszqcxv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsdewmxo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohnbtjfu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jlujfkfo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fbaqtllm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lwvfhwab.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dnfzbxzr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhjbveb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlganuuy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkbgbfid.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tgudmoal.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3opayoxjk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hwjuhaqd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yzctgngf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciqjpdmp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3elbgmzkr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ccthqhzj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ooquduba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tebiqjex.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqdiqsg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivkrnjde.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jiphkaqf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3cidweryb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdcoapst.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3oqbfainv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qvkkbnnf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3djpovjeq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3onmkezbc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3haeodppt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3amnrsnyp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3iebvicmh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3efldqdci.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nikzoszf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3txokflyz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyynmybi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rxoroamr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ejobelde.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gepmwldv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjxbqha.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hjzdgexl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yvmrhpjc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3potgimav.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mpmeneok.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ckihmpja.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oxyycrfq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xfsyjgik.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nipywheb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3drtgwste.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iuncfyso.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jfavfiak.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gkfxmbii.html


<!-- 参考信息 -->