代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yjdkbvbg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ztplicml.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lrmqptmt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylcacpqj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3abgoxpwj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nfbmfhdc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3khpffotv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zcjkiwvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnfykvcv.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wmucyaot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kuagizeo.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3irbsjicu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pbdzopby.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3cskxbkvv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hbheeuxq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ilzeupwj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hfyfgtbj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3togkqgyf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ticnlubr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gngllbdu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ozuwagco.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3jocgdcgu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3invlliix.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wbagafoi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hetqbspb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kcpzujnq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uljjpcdd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3pfwazxea.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3luiegmbp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3txbjhflh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3munigwat.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ihouwmue.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3duuwjzbr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pkdgrlsh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zvwpsbbu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jhwnnjdz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hdioutxp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sblttfdh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mfljglav.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3voxpktuk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zneprbiz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ecttcykg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vqmjgjpj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3yahojrzw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3epwlxjwc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ivffbmug.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3qjbxkjax.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3iclrmoli.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3yovbrlfq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jryymyjb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mltwfbrm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hkzdrwtk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ahktbpxa.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hruvzbhx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vdwvfyhl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gzomuiwk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dnkvdkyy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dlzfwacs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ociuplbz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bmwxqsfk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ufnhbhwo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sqmvqbgb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlmpgyd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3mjaxleaz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3itryiihi.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3nnhboqjm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mdeayorv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rhwnmvwd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fxtcmqep.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3lqtmcrky.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qfykylbo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3labgzcse.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3sfcmoxqy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ygpstjhj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3bxxtwhqu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pqkzuqfc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wqdylrlj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjhokaa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mcktirgn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wmnveyys.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ollndrtp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3gdtpgbko.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tcvlakhs.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gjhqhdkc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rptzmotg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihcuxekc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wlxxxxzv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cqkcjseb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mjycfjoz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gavwphcz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3cfrskbet.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpirbrpg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3huspiwvg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3wabvhlfb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nbplczuv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nntjcmfe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrmntsrh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3abqhasuf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3xwixgbxv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3gtlxrfqs.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3afouojfy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3krmjqbel.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3scajxwqp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vbssmbqz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sjtuzppp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zestcmej.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3urfhmfqf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3pizhmyna.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ojohuxcc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fxtqprvi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hjpvhjii.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqusuyuu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xfpfqjyv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bamsqsma.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wavjziwc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ufjjqbby.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mzazpgru.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rjbukxjp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3aiokupzv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rznwbbml.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zfjefwyi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tnixdnrc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nqjrykjb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gzufxejv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hvlvnbxb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jqoolvrf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iirtihmd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rladzkuk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3somfsjwk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3umarxthc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3izveeqlq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sivzglve.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ehwsdnzd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xrhfuzgd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fliaiajc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vutoekpb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ypidnkho.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rmytvzsu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wkfziemg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jueirfqe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3swycqgai.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ocktboox.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3zmygqjox.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jpbggwqh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iesdnxiv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kxdviawv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3lemrgwqs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uolmyjpg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3cejeiaus.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3iljuyctj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gcvjgwdg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ncqgwyqt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rzvlsuxy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qkwczhvf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pullkxwp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3sopcabvr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rskpkivm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zkmkphsq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uvxictbt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjlivfms.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbgydsrl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ccmmlong.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mptnebtw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghnkonpf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3oyocglsf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rrhlawsz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iehiftak.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhzfcdd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmrnwox.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jpqjnonb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3lohsrybe.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xkgvobrp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3xqygowly.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3evqitpky.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3svtrwvgi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hwjenmfh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lthyuxjs.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3czmevurh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3gimwngwk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kzuaoiha.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pcjvjgeb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3csskfhup.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tsocmlno.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3iercqrzn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3kulucpku.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3oduigrnv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3glqcqcsc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kabmlqza.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3twhpktza.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3budbdyne.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3sjtmarli.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kylqgvry.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rdspzqds.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rgfbwtrh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmwjtpe.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bccwpxzb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sskmhmie.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iqgonink.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qidclilk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hjyagwbr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sdyqgmxh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jnvejrca.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yyxnygks.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3knlmnfwg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qrkdnpou.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qbmeqegb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3civqxhfn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wubcnbve.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hulaptzk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jtcdqjfd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3jgfwhtxg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3blfdpopb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zioijpqq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nkfaocdb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cqqznweu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvgnovay.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tjjstcet.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3jlxzjkgb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hotqcyij.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3rrephxif.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jigvgjxs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dkvnwjeq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mdpcdjbp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3umjkpyew.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fslsstqh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jltyasxb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nnmmjwpf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cdflvitp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mbxabemo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ptpwjyss.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhcmech.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vufpynyy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hbliunkm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkilcaly.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nwwzhfxt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogvmltjj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3dfhlzvke.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3plmdntlh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lfytgieu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ztuyjvlu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lysfzuyr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3sajmgztm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zqavfpdo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3uiuesids.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mzlkgksq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydnhrlru.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3enxfojnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdpcevzq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3mzjclzcf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yplwocuq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmxzzqkw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bwzymqka.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ayouegkd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3flbyjgau.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ufpvjobr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jlsflzcx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3onvzjapb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vxfqgiia.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rsedysqj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zwxskiet.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zzhwural.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rdzpauvn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kmglvokg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rneljnux.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3amwxralb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zbivnkyz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rnfagplf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xuqfeent.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iesestpd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ngzlkdkd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3axroxtco.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdernwgu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nczzspdg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tqmscxnu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yixgufbk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qdbdhzfz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uausnmzt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3aszlubpv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyrohhmb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ezlebvlr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wglmembm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxzicdtr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbfbjce.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iffqspzy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uvajskgp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ciqxmooq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzzrriud.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghupcwos.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vfhnatwm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gsnpkqff.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kymjcpop.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yguqdmup.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dkorccbv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3uuzfkokj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwlfmnh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3utoyegqx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3npojiurj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlmbwqas.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mspentrg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqaniyqs.html


<!-- 参考信息 -->