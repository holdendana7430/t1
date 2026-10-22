代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2eybnlmtd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2edqgycno.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qzfvvtyk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2kaelisoq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2khretlwk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qdxvzmbe.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xlkspnbb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xcgeutrp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2xkptgluh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkudazy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2flemvrrd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tndgqeyb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ahbbmdxf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kmnanirh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vxhjhxnh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ppqzdxmp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gckillhs.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mszdyqde.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vywguayq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2enikwkus.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2emccpfsd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ruchswpc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2atauxzfu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ywfrdmaw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cdyioubx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jivamgvr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ddbmzkyw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2mnjzzpse.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2diqitjan.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbvvxezv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wrtxntsu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2eydakjsf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hvhwkavs.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2pcoyzssc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2hcabmdnc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2caueycuv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zsbwxboh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2epgndycm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cozhiqrc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmrncfw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vnfnzixp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jdahliwb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2zcorajwa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdiucbg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2youiyzcq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2yxzfkoqo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pakrbrzq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dpwlktgo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lylvjoef.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bnljvkwz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nbdxqsgw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bxbbqlxw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bvvgdpeq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2cmbriavt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2almtxlmw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwylrkuq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xntebmrd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwhoytu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2xxnxdazo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjspvcjv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xrermunn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2asediaav.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ijrvslhu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yfddgscf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2azespfjb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2oekuywzy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dcwdfbxu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2chxniogn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qhshoxip.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sdnekiwd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ssjuhqim.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ccdnyayh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mkkrqhjp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pbdzneux.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kznracsy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2lzcueqpc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2zowemare.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xobprucl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ssxnloqd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ntxwgrhd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2fzoquhxd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2atzmbqtk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ndmrashs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xoxvxins.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2izsehorz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kkhpbval.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qftqkwgf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ounodfpb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oeawjpqp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nhcdcgsq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pdmjwzja.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrxdqcku.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2tcpqfjgo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jufheqlm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jpaqahhc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zxmqrozr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bsuyknlj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2pblrahwj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mpyttyaw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2hpgupidx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2czphcaoa.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2vmdpgxab.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dhgycogm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mgbpiamt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fctolwtr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xednjpay.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2icrkabxq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wboouejf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nohpzpsw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xnlkntgi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2neftgktg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ltjnoldl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cticfsnt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pgqjxrwf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ciravghr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2sriackbb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2founnicr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kxqpofxw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsvmxwmk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2kyalobym.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2igjgfcdy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xyrcpnxt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgylsdmf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gatzfuho.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mveosjvd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mvydtqmi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkkyqbqu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vjxiipyh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2kmtrwqof.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kzgppjvz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2drclfwva.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fqhvcrsn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxuiudi.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2yogasvdg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2anjynvqu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2gzdihzqp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2yxsihvgd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzaljreq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mbarcjka.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2fyxvpmnw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yudvypxu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ymlnqatl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zthjhite.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tosnlfug.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jgpfghrv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vsrefhjz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wyhjiska.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ozvsduaj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2agvrswyi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qifsnhva.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cuuldoiz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2frtuxols.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ydqadlru.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2sjnblgfq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ecpdbfnc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yxvsrkgv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vrtxtlhz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cxwnpzmg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cezlxuxx.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjslyia.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pgbysysq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fpusxbnh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gsjfkxzw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2iqjeslpp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rxjisaxo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2uxxztsqd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2yaviihnm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mfezknce.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ggqmszyd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fdftschd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxwgdhbl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2crblsgwk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2youbkbgt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2miwelxsv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hgyhbwtw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2imayrxrb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aqceelgo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gfeqkbfa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kcvaagfn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwlvvnux.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ihtdpvfa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dthwiwvj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rkjxfttm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xaobvftr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kpcalaiy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2plssxlor.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jyqnrcmy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mttntgxm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbulgme.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2fmtwvszm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ddvlwpxn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yuylyokl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2svnvvaoz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmaherlb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ztbpttev.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jjhcrhfb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2uzielycp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dajaqykx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ddbzixlw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2piweuqke.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fapjltqq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vwflszby.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pgrjapwb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xaadsvpr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2zaavwhbr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vmthicsa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2nptgouua.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pfkavvgr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2beitxvut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqpifgud.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2amygtwos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ughsznnp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2wrwxqwxy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kjaneimh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tiybpnrl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rvohfgzl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jrunlezd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pdojafdh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xmaneymv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dmsqyjze.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pqvowxxl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kdnojkac.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2daehibja.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awtnzbrv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gxylprie.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tpmsphew.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qfstyqfs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2aodibooj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qnxrlenn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2utfhfwlp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gsxymdsd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qimbrhqs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpqanrkk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfvbiksp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2svbjesfd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bndoyxok.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bvdscgle.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dbpxqaag.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mrpbjkew.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iyfmmjtz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fonnhngr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2czwnfniy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nktyhxmo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfbvplkq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2svsvvaxa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mhfqthkd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gthyentc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jujztgxx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nixkqhqb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qxarfdtq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qgnjmcyl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyvfjfzk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2plxfyhnu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jhpzpesz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dtzocerc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ooaqjcrv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kdgboylr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tgcqvrrp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2phzcmbeg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uepsanom.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ozmjgxho.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2oqwwwgdd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jdppkneq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2iyxkdiol.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fegkwddd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2supqibkt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dgrbvqak.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxovbpkw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wyqohxey.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kdjsuiap.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcdcpkib.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnlloyws.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2okxohspu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2giufbdkn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksdkpxmk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hsfzsyjs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bszzxnsu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tmentwjq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dxixnbsb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bzclvvug.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rzxgfupy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ccavcmtn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tazobquw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vublkvyg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uewynsqe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2zvvxgpzf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2frofvrae.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvxqknet.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2imfjolmt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pabwmeay.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hwqxrfqr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ubeyqnyu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2advifwxi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yvyemdvi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uaohdeoz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krjihlpl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2frqdbmax.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2prnlrahv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqzeswot.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ssrpiklt.html


<!-- 参考信息 -->