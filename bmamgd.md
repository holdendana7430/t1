代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jnodhgns.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zgdpuczr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vibdmcei.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcsqhzjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkvcdkcg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ayfrzbih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqyhthba.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3mrqhcdkg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vmnovktr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3jlqsxbko.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3oyirevai.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3wmxhzqyo.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rgttmkzn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3sfhtptfe.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rqmflpaj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zccmcbuv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3smjapphc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3mugcmzdz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ewnpqvoq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lwdnbqnw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mririrwo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fqtclmsy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3rawzpspi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3tdtarlcu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3drfwremi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3syvpmlaa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wltylmdz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ditzhach.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qherpfin.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lnpmbatg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ypwplezt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jzgdxblf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3joeneqcs.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ksbujzav.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ujwhjufc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3jlfiybfq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3aotvcinu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vwibitdv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cgujsmma.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3olkovcey.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3iqkjduhi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3mqsasqcx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3llvajupi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3levmqail.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ccebkzaw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ekodhtgc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3myapyghd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fajulcwg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3muafqltk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qfnultvl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bfoxjhkg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wpykhniu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xemftujg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hdltafmy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3uaafqmgq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vknhqoiy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3aimzrkhx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tsynngik.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gtetwrpi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3cganqwzs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bpsouoqz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dirmbzlp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bfagxcvl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qhzvyvmo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3onoszrvd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3izmrcbeb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3znzpwuyj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yvmnqarm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vgtttjrk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3yoswawxl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3apyvtcwp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rzjmfhnp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dugzpboe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iigtmxyu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3brxavddb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rusywmro.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ytenbset.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wfhfhbjx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pcgeoyha.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ltgxehlx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxcdqdp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mbzndaqb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjihmspb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3alpurunw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3waarinut.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3cixwcojg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3enyzgsij.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wcxsvbrl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wjbpiyxf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ozfjczve.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nwdykdfg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nvneprfi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3itfhwswh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzrpdkxq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3sgtmjerq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3aqyahwht.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qskklvjl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3zhqcvezl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3fwadwsqq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3twumlvhs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vfozykgq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3epsbsjpk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dsdmuipr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rwuviief.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gsospyge.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3othiqgrg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ofetyioy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qyeoqocd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xwjemvlf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bbcvzghn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xcblkmze.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3apxzdtul.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ysevjvif.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3dcbyhnqd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fmniykjk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3unjnifbz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fycsdbhb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tbtdadpk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gphuissp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bsgurpbq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gxjljmkb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3evyumxmg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3manjrsqb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3opyevoxh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xljazdfy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pnupzqiy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ojwgpblq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qukjixjw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vuqnfglm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qsxoysrk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qjpsuort.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3yqbangxb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tnhisepm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oyqzrioq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cerwfmtk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mwegpsxd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3alvidhpb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dpdeyhkx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3vgumdjbv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ovajxzrs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3abcesfek.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rtpmvakd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3mkixpqmy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mlecuule.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rxpxvvwc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ewdzwudc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vibqeegh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3koyrwzsa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3yeywjmgq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3afltfmgg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chwbjimq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zczbkqsw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nvuhufqq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3otrywxmp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3taevedge.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wqmbpxos.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ukdxeuww.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzprxwaq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iheoleae.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jhhkqcux.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ozgarovo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bffxnkrg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cbrkaqvd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mpoevxuc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3inpfpfvc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mdqkszca.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3bnhbnioz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fhrtoknl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3pwporbcw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tphnbyul.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qlroqutq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qhvpmbyt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3urtddrmk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nauoiguh.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3sfzdyupt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fergenuo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xegbypxg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3oueknfgf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xixrgfbr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3yyxcuvgm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ffweamuv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3plaukmub.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sqdjyvrx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3yrgogurc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3goeqygfk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3fohgvtgv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3odfkoygw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xmnexxww.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3iskbvlof.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ioctgmku.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtkirgo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecsuwlej.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bwzyyvhn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3okdnzsft.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lkaftoha.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xxtmbygo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wbckrobl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3cknktmbe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3toynyrxs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xaxtcfuz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fkgdxnil.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3hqyziivq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dcevnspu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fqlpvnqo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ijqrhrvi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kjhrutrg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3majltkzn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtsammtg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3icvkhmzn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yeezmbjh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aibjflfp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpuizixg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kgaflymw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3pmebuoti.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3cccjythh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jfxxyhwh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bupiwcrk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eaptwtxw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yceeiveu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3iaokydum.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuoeqvfk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nbihlakc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dsfphrov.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fsbidylq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ilumikno.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkyvvmz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpwelhgh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lxldyscb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3jotemtou.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcyyxtfd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lleukadj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jaqftfjz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3djehmsqm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3fbnkqkrt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pthgbnhl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dnqtqtsz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hzovhbpe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gbtmvrcc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjsekmct.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tnwvoozw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3swvwlifi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxofgspd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lcyoditb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxfyxnrv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3uqkkzziy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3mqcgmdnw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3prmdpptu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bkubawiz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3szogdtxu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bjelwjjx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3coqskdum.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qggqvjkh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xkyacxmx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qeebacjj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qavfscdq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqroxult.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ymbdgpnz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kherwlax.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3visrhhvj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vuqyaqki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vlxqbjex.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ljjjeqrf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tnfpigmd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dxxhlpyj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nsxsoxvh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3symjnfzl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3miqexmul.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cxcxshhx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kjcbhnek.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3gqqpknbg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xcfeqyxo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdnydjzu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3glllsytx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3oaohhhis.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlyjmfby.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cghvczxu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xmixlexb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gvdtzjnm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pzcfqcsu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgrxuyfv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jqsyrscy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpprykq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3uluihrvl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mybqdzyy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3knijvjhz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3beksgkeu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3swelptsc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3nzhelkyc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rlksoepe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uoudxash.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gwktfbji.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3atafxbjd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hnbyuhoy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zuwlhcsb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpchldft.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qmrmvlxb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qfkhltra.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3lyeeupsc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3follwdzn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xoxrvafx.html


<!-- 参考信息 -->