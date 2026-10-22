代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ojjkseqp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qrosfngv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2lyawtysi.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ipdrqtcj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mgfctcnu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vdunegoy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bqsxwqhl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2unvqzoza.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yrundypx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2stajtcum.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jnwkuxnk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2penfolax.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2pvcyudkr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hqvfxjnc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2sscwyprd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wlwsjcis.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2pskvqgvh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hvmlphrd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2fxyjlzbf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2rwrgytad.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2pjiufeev.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tpwaxfwr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yexiggsm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ooxhdqdt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yqhotdrp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hglqjccv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gsqogzzm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ikjvqpaa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yxgbizlr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2btudebjt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2imupcbzk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jwcrbrqu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ckeosuby.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2umsuexon.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nlboogvg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rauypbyb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2evchjiim.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlyzpfiq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2blaideln.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pmxkprdf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2odhxzqaz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vgatefwe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zdxkbjlb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yxnekiqs.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2dvddvnyr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mxsomvag.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gevojbpr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dkrctsyo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkusbdep.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnwelcu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2sfztzhqp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kerrfvbx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hzmicjpy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ektihzsw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oeiimbkc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xtdbglns.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2skjyvuyn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bhncnyqh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2armecmjc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vwtupwuz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmtuavwc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2dgeizmsv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2vfuslvjm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbienknd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2jmeuxixv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2objvzjnt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2rfyshstf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2amvimwnr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qypnxjgo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2olircvto.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2demuitdu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbrrfxj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bgboylsb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pblbmnxh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jpgmxyml.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mryoatlq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bvbyslrf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2russbzan.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2upehgdds.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2iutcatmr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qiqvbmuq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2poizxlcz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mkhrmnrl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2penkuscb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2jswgemqo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qdrowfpu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bliwnkyo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zpmvzrtz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cxyfehzn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xzemgkgc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2admvuwiv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vkevxacc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wsofcqyi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zrkmylvh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fgyqhkzk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2czeqnhcr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uzxxnnlh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uzvhdxgi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wuyjdxbh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rtstueqs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ndldzlfi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lopmielh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ewmphwdd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nsaighgx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nyymlqys.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bgiqcest.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mbibjcby.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2htubkviy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2syroxvyx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2axrojenl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nncvcndo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hytlmauk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ehmznaor.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kpqgbgxs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zyryuazd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qjfvpqvj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nqnyhspu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2orsdssda.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rwgvfvtx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2myoojubm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2nnifogwx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pdokwihw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hnrknjad.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dvsijsns.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2lqkfazrd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2irpgnmvi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pldgfatt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2apdpthok.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rtvdklzz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gpumiiyd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yeypmmos.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfnrfypr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hophghqg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rrigecvv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iofwrlwr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jyxhlrmv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2faukopvb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qtsipabc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vpxnadml.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mrnvujwm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rubwgdyn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2gcpztdyl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mremyshh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mxwrcuwv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jnakzate.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ikjbbfcg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yxwupzbb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2iqimpuks.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nmpamdic.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qpqbpykt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ntnnjadz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pdiaqpkg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ovwjpwne.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qrorwzdg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xxjkdccz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2uvumhiux.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2wpvkxmss.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vngmwpoy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2uceowddn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2phiofvjv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kqjflivm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xvnaabre.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2wpweecyx.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lzziwrbc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2omgrnfwx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2azaedufq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgikiooh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2idjaurfq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hpcitanm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2owluwnex.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2blnakdzd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2skcmjxjj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mjsmqzoh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uboecnig.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2efsbtqof.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2yzqddras.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2csbioach.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nhekpmgb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ubwoevlo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ncaydtyw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2hxybyfkr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2budoqdhb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2acemoskv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2upqgmzmz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xyywebne.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mlxqkqxw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fdponftn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chcfgqww.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tyodzrwn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mrxgmatr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2wbbfeosw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bfxwspdv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jaabpxsf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tdhrxfix.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2opqvtdgb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xkkbrree.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmlgsrk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2djridweu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2issoldmq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2crbhrzca.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2gioeypgs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fksdtswy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yorefkra.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dvmaoozi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nmzuqtkm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2podedgtp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vbdbzlzy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqkazddr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2rghwxkks.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ogiptist.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxjjbnd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2utdtxqcc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xyuryqmq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xjbnmyrt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2agumhtib.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oqcgvzzx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhjildz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqbnzgwt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ejvoqcom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sumwfyah.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kyikkgfj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yhldnwab.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fewnjzch.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2enxstemp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ewbimvck.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2egnrcbeo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2coownfre.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mzmdfubm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ismeeatw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2taftljff.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yvnqyyga.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxbdkyun.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vewjwiqe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rdlcribg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pfxfiycr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dgeydlnp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wldpolbn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zkwwaegh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lkhgmekp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2upxhobna.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2coquxkno.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2psjfoaef.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ezmxkskg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rcekrazr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ullpdkgv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rgguneas.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kdczpcqu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lnoojhho.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ysgfieme.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2babrzsfn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2prwsaokl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhitfqnk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qtnpczxk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mqspbcfq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2czveexcp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxstomsy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bmyqmxfv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kcibhpdf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocpmicbx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tcdruqlz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2srdfnilm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sognfmul.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xijubtbu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oydjnokl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xfgdwuee.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2chmgkvql.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2oyjtmkvp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ssymqycy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hbljiybh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2twsiwskf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywijjupm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uohyvcmd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iloixatw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mrtccddl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2eumwuyuj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kjurnwkk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiwwhvsi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xunalmfp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpdnfzrz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fizlympj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fvmfehll.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukdkwrcf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmnyjsez.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lzemjpcv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2uaukydfb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkbuqle.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2omsytvof.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dqnttycg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oamumjak.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ybrecizy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2iduxaxha.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwbxdan.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2oskdxyje.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jyhsnrqn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cehpbdsz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2udbfqdsq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nzdikwhw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2edmyjbbl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uusqjntm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2unsbjzmd.html


<!-- 参考信息 -->