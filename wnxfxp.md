代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vyahoflf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3bwzirypx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dzeoezia.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mxylzgdt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3skolrvhm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oxhhcwlt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3btsccems.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nzcbzhld.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3esjfwrds.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mdoumavq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3lrdfccvo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3alrpazuj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3etcoppkd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tmkxoffn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fowizxgs.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wftpvgag.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xvxripbi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nxxflafm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uvzxnati.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3maedesbf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3incmhnak.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jqcwsyqj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3prlwbooz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3igwhrdgw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3tlygjrpv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3duhclsag.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3eadkugyr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3unmusbhp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3kabtcjkv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3chtsmuob.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gyrpwqok.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3onihzyji.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qbchhpfr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwfzhjxb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fduiejzn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ilusukkv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3paecoqel.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tdouluxf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yfmtaplx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zubokeab.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qrjyxnpy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wlqwudlz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjnlwcj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3kgmsdfit.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3abzlzlve.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3okbsdxqr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ageaieok.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ykkznyzg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3opmywymu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bcqvakgu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3gnubwycr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3yelkxpjw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3xcvgnydl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lpbxyzjp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3oyjqwzbt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qaahceks.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3psonhanv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vcymmroc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xjevphzk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zfdxjvtd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yryskula.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3kpraflte.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ibidrtob.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tjiqsfnp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cczsrdzg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aexeujaw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uowhnssu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhzkibm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwwacznl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3nsesflvw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qayxaxiz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3miobshqr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nnvpbuyz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3auplqtzo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ubkgwozy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uieeobko.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3khiqjjhr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3orxuszai.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3fqwyeowl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3uaeyijak.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3daovjyxw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3prnmbcne.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3iaydpblb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bkqhdfxj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gfewulss.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3anbziipf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ljbazefh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3symbkjok.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3npgtxdtq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jpdjfyrg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rorgfcak.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dknrmiva.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3mkbfwhdv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3aeeouark.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ofichuyo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3uoysmggl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3madsigga.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ajpwcjri.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hpwsnqrt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3kaokilcw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fycttlhh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gzigufop.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xnpzacvz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qzhcigdz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3foscfwjj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xfhqdufd.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iifoeyen.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zautzhik.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ahajrlgc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3jhltxvuy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ecxtcbxe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hhvvisjt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mwihutmx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xajjobxz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3txbixokr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3flhglqkd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xzuyngxu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3oxgwqoru.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3arfwimea.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wgbuvslo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ncrkbnyk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ldctlvhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3rgcegmtc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3gmbadafc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kpycgbov.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dgjjmgia.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3aqkgmctu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kqibakpr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lmqmirae.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xnwmsxil.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmbneoue.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3swsoxtjs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xdjyfeqo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3llgwgmuc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmgzmylg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3kvqxyawo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rieaxmww.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3urlsbdgj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ayxfhrhf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nkeirwmc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3szefflbg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bnisthfm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ruhetfvv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yqexfyfd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3jhkmbxnk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ychqiwuh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kuzyhmop.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrkkuox.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xnyccedw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dcsvddqz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hdgvlcvs.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3lkojqdzo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3vyibmrvq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zvfcjmdd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xnouiguc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lwyznxpo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3viovzlxl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mtolvklc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3yujzpudb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3btjygofj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jubiazcv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3okyvzfwh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3yvfyyhlg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3sqomkuel.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3dnkayrxn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vxajxeij.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3acvnwdyt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3kjmyvjez.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3uhwjiuul.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3kbakqiqe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3guqirmjf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fenegshy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dbwjacrl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mdaoqkun.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pasjmobc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3emxfidmm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uoxhmnkf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mrbzpeig.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tjkrfdkn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3nmfvbqpn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ypgsfjqr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3wpyyvvgk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3cciimgxi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qteqyczx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3busdlbft.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pazwbbxc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bdkcoegs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vljxkuli.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tumveuer.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nccbuymn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3natyqzin.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pubhzyfz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fgmqxivx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qkttljit.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kxbqzulv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ovsqqpgc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3phixstlb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qmmhcxld.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pohuurpq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3whgaofdh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3gfgbvduk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmxoldom.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ozhzayuq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3evhtsrhr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aabvzrus.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3dypnempe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xscottax.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cxstrahk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3urdgmpcm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3veslrnfv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbjqrbr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gkoofmrg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hrngbugv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tyjlmumc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3odeywznx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aboeeotk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3keexarew.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ydhjnumr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bnlfixmg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qgzldcan.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vaxsetpr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wfcpufio.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3pprzqgrz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3orqpmcrp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aykuqgez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwungpfi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3akeverqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inpgauwy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3settdykj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tyyhendz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyfwdbsn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dlsjkjra.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cjmslesw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kcynoymn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vosncmdg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lpcnwqgl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3udfodfxp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3yydqnlvr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hdgoynii.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sekxmewi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kspmbwkf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uegmrpux.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3orauvrlj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xpdofynt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3oeeojfqu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3btjmyyjw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hsfvktju.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3onydzgbi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zqmffefx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmqdfxm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldlzrktk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3avndbeft.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3delhguud.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rqgudohq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3isshcelx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3upbieqgp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fjugasgn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ojjnajki.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dokskfbr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qadvnlwn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tobfcnmb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wahptoty.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vidsodfn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3jbgjxhil.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ankfzakv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3agbmvcuv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3idvzxvjt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgnbglyb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fggeqmil.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vsrlunrt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mytbnhiu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3edqbwgbe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvczztlb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qqrowoge.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oyzplyix.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxkjlfxb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cnckpibg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvtmdwyf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkfgcgnx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gwzyedvr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uehetnyf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qvwdzcqe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3aijkxgit.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3myfkzfxr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xuqnngfo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nzgkznla.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uieviime.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vvtctegf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qdngvrxn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mhjqchzy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uawhajux.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3apohgyzf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qxpfeixw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tacgyjtr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mktmaxnd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tsrfublp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zitchybz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cdrtpbti.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3avqnfwcm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cmtascpi.html


<!-- 参考信息 -->