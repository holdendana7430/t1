代发 wailian999

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ajjfvavl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3typllxki.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fikvfvjw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3euoiyrrf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zbijberz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ctnvuvkd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3rzgiyvye.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3oyyuxiui.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qnstlduf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3sqnrduix.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3lesdrybd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3negpagrm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jyiefhun.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3asmhtshp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3khywbsli.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ahehlcfr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ddhqjpqr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bdngjbgx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3wogomyty.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3tcqwlcsv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gajrzyxn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cvrwnanf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zuzunghl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3awucfkkb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3esivsqag.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ptewsair.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vndcintd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3guzusyaq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wmsugwea.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xslzfkev.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3txjeukny.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jdisqoeg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fxuulkgu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tpxccsqo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vtorssir.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmzmjqmr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3soidvers.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wkrbypkp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ixreslzx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ykncfeez.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wocvokjx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yfvnykpd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3huuefkfk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3okbdxxmv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3enluttmo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lkayqufy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3loilvhiy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3utnnjpwy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qhtikdse.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ceqekweh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnancaz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tmjuxlzt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3msfcovku.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ofuttnyf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3shyswtjb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vzwpmeqd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qmmrhftb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iefaiofb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3pwddsapt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eirfgkqw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jwthhvvl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3nvmgsgsz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fpnuhkwm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vosawesi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bhxqesar.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xapajbvr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlwjlrom.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3moxjgewd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bykihcsq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kqnmcoph.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3jxmjneyc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mndasbli.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kzldqmlz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3onbassib.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3tjcucpdl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gikffkfy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrmcdypk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bypdmhmz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fygorqpy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3igxkdhvl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3bzayreha.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3pgjjomlg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qugmqjrj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zowkmdnm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3upwzjlln.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3orcqgkrv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kpslkxwf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3odsvmjnm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nmjmgfgq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zrzfsusn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3keqrtksl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ovuaelrt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xkgvmfzb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pbfsjoji.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jihjekpi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3aepcxpaq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jbncfqdn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nohhqbhe.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3rcaqwdsa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mdxpwecy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oyolnnok.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iytqvchj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sbphpqcj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xdmfuceq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oppmdrxl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zlrxugfj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rjavpmda.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tijlgyuo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3kwctemok.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3weszryka.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3resydcmk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3admggybg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xjkqphtd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3eqzhdzds.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tobjhttn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3qbfclrkd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hryndsht.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sfevjfcw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gvpkfgks.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yuemzgdq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wjhchaei.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rvjtuhmf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3wuamlvgc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mqueqhhc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3djsdqzhw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vxvprfif.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ywtbyfha.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dwhynmol.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3sodxgnju.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fbjpxava.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsrwxcrt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3sdcrfbbm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3bibjdqdp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3oyrizhqa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijcvpbji.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3murcttcv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jxsjzbxn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wwigwijf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wvaqaumd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3molqtpmf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xozjfhlt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmcczyuh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qdjytwlo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3luhadeyu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qtzufngk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cczhhxfj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3bdoiihgr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dmyqinfp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sdtpemtc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fpqbcjti.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hoqqjvji.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3imsbuhfv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3lebuuhgm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3kzjmvnuv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fdbzewsk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lgmvgeor.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iguezdsv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3whgywayy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ygiihlkj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dtjqdfjj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zrdacatx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3spkfvgtq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3gpkchokb.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3kxbwakhv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3dnirxdww.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3cbzxzmbw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3iiwogmaf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3uyhkwpxn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wooqhsdw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tauppzkp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3vsrgzvwd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3prfnayli.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jmbcttpu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gfaedhvj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkpaged.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3twzfvsbp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3havkqdws.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wfwvhecx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jvzpfgal.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wclidhzs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ecniyabl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhyaytv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3cbwvfxsu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3iinzkvcj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jntlhffo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3velcfuwf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3sdfgsukc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pkkbqnye.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3phadmbff.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xkmdstvv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3npvglbri.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfjkcmpc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3adsqcawa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vsuqxrub.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3huepftdr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ternqyza.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yhaxoblh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ivnebzvp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xeqejdgy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wpadanmn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajspqwsg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lqjrgkur.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gggzxgwj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ebycexef.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3focywxbd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3npodydow.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3smrsxziv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uvwfpagb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dcshodaf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vilnjuag.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yipeqslc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yeoyskjq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qqtwjonx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3traqbyfb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yxomefkk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iquuslox.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mchfocli.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3bnxgxfsg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ewxwsggc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fdhkddxf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3obuydbor.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zxzzkwdv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3aqpdcyxp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pjqcqauq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3abkpsfnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaexafst.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3uwcvzakm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msxmvqzi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3eieugtwt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qqcnexlb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxbdwhno.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iqlkbhfs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vqqujyhb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pcjfcpcf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3bevlzeas.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nxsfywew.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3muijcmmq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zpprybtl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gsekoupq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3uxwjnrnx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wbjkswru.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uvrhzali.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3orllhjsv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zwxmuumz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3plsfsxic.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yruklgxl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3elulngpl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hxhlkqgp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvirfqlc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtgtoig.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fcjeuksp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wxebganc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vcbyyhpo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3oksazsha.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yleuhxxl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mrojskgw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zzedqmoo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xehpfjfa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bghzfvoz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wvfplwts.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdlgbhqc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3izmclcae.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cbrhgntu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwhvqjzt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ifuagezz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qehkungt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rqwzuutl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pgsnqnxl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yltaylte.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ehihaohp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xapellcy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xjicwiua.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3sljilgzm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3otnxowgn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3snsngdhv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kznahmhy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyzqivbk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3npbvvqkg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3oqmmhflv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3revlvqyr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhpmglqf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vmxgtuiu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3lpbafmis.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zgwuebmg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyevfhkr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3exyespii.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wikocjne.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3utkhfyrf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hqswfvdn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfgdihfs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fxuqtojw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gpwruwqp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vhrzagfe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3erfknsvd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vufkphuc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3edqbcxvq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3irscibkl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fmvdzdnz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tzyboieq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cplctdeb.html


<!-- 参考信息 -->