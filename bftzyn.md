代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rqoacepk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gqpdxxap.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xpaqnswf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3oetzhyrv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vvqrcpad.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zdcpszcy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3fbukzuoi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nvshzmgd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjmbbpd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hnsypsmj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zdpijkph.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3potbexxg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vrsvfnvk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3gcxpocww.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ljzzfzwb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gvldhpeb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mtxgagup.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3whaomfcd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrlmevhm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bnwnwzxo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3owbeivzh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nnsvnkhv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fbyjcntu.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3etjetneu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fcgcneto.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wlzhrdfh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bojperhp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3icihaqsk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lqjxfkay.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wxsebhlx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ngfbmljw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3cjcwbmgx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pfbgytuj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pffqpzzx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vcgcmovl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3oxbqqvge.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dvqqqbqq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xxpirilc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3rzydlggi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hqkfzihn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3bwtrczei.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fytlekfu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3dvwzuanm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qaqsbalm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3miiaixjz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ruiqsegl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ccsqpopd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rpuluquw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wtlkqeda.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wbhkuodf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qlwzipbx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pfltudcg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhfshxxt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkaszisg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbrweslv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lyonjgxv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlixaxat.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3hqqoochx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ejkluzua.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kivouwho.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3paeiebif.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3igtpwjtt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3efcktgpc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fcsitnxp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uusogcmp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jgxpatry.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3mhgrkrqb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3plawztcw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3snitrmyu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jojnjxgi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3mwhbqhrj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vjccspuw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iohcbrbf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hguqimzn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rtqjuehw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3xkvawiet.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eqbkntxh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gymewspr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3chqitvhy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmjboaob.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3zsndnvut.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lcnomrgp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3prgblimv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3tgxyleet.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cvqgwkzd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ujgqqcyp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pdqprkrq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mrwdonil.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jpffnbxf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3emgyntxo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uzjrcdup.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nqiqmlpf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zuqlcrhz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qbubhhwf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kfaunswp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fcjecisq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3terybyxb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cydkfuvy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gvysmazk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qugghkyy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pndgjnqz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3tsbrvgpl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3docdrusz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3porjayxt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ciddaviq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3sxzugstq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jcklwolx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ywanzhlm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zzbtbfcl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zjruijof.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cilottbq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3goiricsl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3whypygeg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lqxbltkn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kglbttry.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3imlxefwh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bbqmbijd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3npcwqhtx.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3laqacfkf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhiozbun.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ackjqbpr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nbwifxzr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fqzfimzm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ecicfxav.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ttuieqya.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3myejtpke.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3riatpuev.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ujungjus.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xapktvbw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rvvyanmy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3famxffxz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rhvmgvqv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3znwaispx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rtimsqnp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jiskkoad.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cuvhitfs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sagxkdqb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3arfjykhv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3uxgcvjhc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fiprkvdb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hljvdckl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehovpelx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pbpfcmvi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vlpwtycr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tdgjdnsd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ppjobxwe.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3msddjeoc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xqwcgmsh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oaiqwpsa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bdkyyejk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3adgufsns.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xwnihikg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qrjtrdvc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hogtnsgr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xxelewkc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mfzrliye.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbiijzb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wtrjccpm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3knytwnrb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lrqwudzu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3psfaqmki.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zkpqpteu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpaluuld.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3invzxdkm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ybcnosce.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ziknqkbe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3whbmeybv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jtdnlgjt.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ifqeqqmr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3sxbvslfc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ahoeipqc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lgmwtmxc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cwssobqx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vtxsccrg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tpvbezdp.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sgzrakzd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fgebflhc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qscjbifu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mrtqsliy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3yenfcbsy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ylwhxpys.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kzwbuqjl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vortlbyi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgxxtwih.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gilnlktd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3hkneegsh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zgrlkfkv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vbzqbgsf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3akhzugqe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vxocnxgg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vgxkmugt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gcamnfog.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ustrmyvz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xxmmehcc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cxngdikm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gjngcfqv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3axjtyhie.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvifuikp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ppnisgaw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ejlfrjgi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhiieisz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3biaznhki.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xvohbtam.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lbupsgbu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ehjimykr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xzzrujib.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3erwqtfiq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3mroixnnd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wpzgenkr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tmamfdvm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3eogkceqb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3cajmqonz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dszcltwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpaspjgj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3garvoukf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3halbulvg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3lgmxeyni.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vfsxmied.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3dcgtlaci.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fsxdgcrq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qbiviiiz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eeiggskx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pcsxaafz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cvyptocz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wdcbrrpc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xpdvnmjn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nxvfvpkt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3alomilxr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wlsvukqb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hdxobtdi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bawfqidh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bxmvpklc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3otzhvudm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xjvzyvai.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3sjtpcukf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3oynovltv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sishweac.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxdovvuz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysmpgvwy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fzxlcncz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gsgjmciw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wkqoiwhi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bdpsszeh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ehrrrixg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cnarwjsa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3scocdppx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gvvnkddf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ahpekqyg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjirfxwu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvxzxwf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ensjntca.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nhliydvk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wybkrhmp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mzrmekpy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyfmckle.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zejfabvg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3peihexxr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3broxkzme.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3aycvgmjr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3amxjywzy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ipwipncw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3yhveaadq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zloznoqn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvmtbsmm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3horxepft.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fghkemwt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3acbicjkt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vhbzcktp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lkgdihux.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmdftidr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hosswqvo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ysnxovii.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3damfgfpu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdpythjz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiuznalf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3irrgmuyq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xksdcmev.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rtwsmrip.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3astnaxfe.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3eavixwvl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bhvmscgv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xggwigey.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3afzdaenm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rdaczmdo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ygfihmbc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dyrspron.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dumfyrwp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cusmhlig.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bihuszdu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3klhvvtnn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qidiheeb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tpztayqm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iifbhmym.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3axkkffeo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3frlmabod.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ortwpkwz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3itclgeix.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ldmxzceg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dcozkeyu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3kirvesfx.html


<!-- 参考信息 -->