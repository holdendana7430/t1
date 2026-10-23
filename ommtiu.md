代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hrwixeiz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dkdndqkr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tbruhadn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hvvclzbz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3dvtzndlg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jscpqdgj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tldzqmqk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3aoyobxmd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmrjofjz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rxonslsk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3sadmjktf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3udpnfcgk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3uuhnzavq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3aavgfbhu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ukwkjmkk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wautjfsj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivbzdkzz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dytjmugn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wnrmkutn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jlwhbyum.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvrohilm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zeqylmua.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qktzpcsx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xznsamdw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fyryjxmi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ictlybxp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3xesdaoah.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ixauyybt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vasujpxo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gxkztjdq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3jiihjidc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3orfdlddr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3inwzfmuk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rqbcqmmd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3umepdprh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ntaixgaa.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3mmowrqcc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rnuttsva.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nmmzzofw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3lzutlqni.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3fdbxbopz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qwrjrlbn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3cjagcmrj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rubzsdkx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxzhxad.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fkysdnym.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zbcagflp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxhbdtm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kedgelpi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3qtvwtond.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ifgyonsa.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uedddurm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xslgmmxt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxgpyart.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vxvlfaft.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ejxlkpyd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lendewma.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3powfxwrd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qiwplobm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xckrzdzd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3lxzbelmb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3nboocelr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mnouzate.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3urgllsea.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3llmlkeow.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ktwhsqdp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wjjtnxdu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3isavfvke.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qovxwgtg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ptmxjqbx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xyishwum.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mgqbipwq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cxadwmxu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3unnoddwl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zlogywvl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3naasvynx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pxjkyssd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nsdiscdn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3irhjfujw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3drjagpwz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fffexybn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3nbhpvdbq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3etpwtxdt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3uryyfvbp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lozvitdm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bplftcwy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tqqjzgna.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3nojifgfo.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bianncmi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jszcyetq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eeuirogj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tonalfea.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sygaeylv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hncosrlz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cozsuvno.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iczxblqk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3bbdabikh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mqbblnly.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sqyzlsay.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3epsrdqza.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oxrkjvge.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3iqkuibor.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nmfhquma.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ehsnuipy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yaqczcdw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fxsxlokg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gfjejpyx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uvrispwn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yugrblsh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3onrgtlce.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wwwwjmzr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3slbwlakp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3pxsxwofs.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tlxzralr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3anbibxpa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oggmxuim.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3jevwnlgh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qyxbnygp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkpqdffc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oswforeg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ymuncdcd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3asxgyhtv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3iqzdonqi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3quyiptvx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjyeeins.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydjvnxqq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xjtpsegu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rlowrwil.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yitpavwu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3czqbnvrj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kasinfkx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ubttzxlp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qroeixte.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3poatriiz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kwxdavjm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrmflft.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xgauqyon.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3abvoaulh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ahxuslvs.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bejncwog.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qxxxwchv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjbfkgqu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kgnnogmc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3iwiyhjuv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3npefzwif.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pszluxqq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3jdtctpkz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hwnpnnhz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rpgjpdrz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cxpmpxpu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3bbfvhwzf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vwblbzwa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rzqnhzwr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xlwwsapp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fwvmmqzw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3xdhvwqkx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3thkjoxkv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3nbrmpxht.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3eszjodmz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bahvpfan.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rzpirhkv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hqanvtmm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqdjvszh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrimagu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3asjvqelv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yxahdhrs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3opbkqgfo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3witoeqrg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zhwmflar.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3joryxjhb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ooympanh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3fnnuadlh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3valzagvz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3sxpbmzke.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bwyotiuv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fqdmkjsb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3sdvzvmst.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3farhdaaj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kszpdesj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vgqngqbb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fdrsyelm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qenavovj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fzoyicrh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stadpndc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3patjnbum.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wadhhpac.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3mnyfplev.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3agsgwdmy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nspkrcvc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qptgsvbo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3apmntbmd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ymifewkx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3faeagoea.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nczpgbld.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wvzpwtgb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ywqjybzf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mrverbch.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3knpfcalz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hdakdrzk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3clbaytab.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3maktvgke.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vkkzzmye.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3cqtkgvzm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wbsgjzej.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3tkydsbtb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3kiqjwasx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ilqniejw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xhgcaups.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mlvxcbjl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fqqqsjqu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3czlgngvp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oreahfxw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3niahshno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbavctpo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ifuuhtau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmkeqyfx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cnqtcbjk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pjdrbzmp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ggvxrjre.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gbmdbhit.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ypmqjtbf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3unniewch.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yetoaqtd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ptfccbmk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pqozqxwb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qxvqkrmc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vgemicib.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyqwdac.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jiljstba.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wyfextjz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xoqaiwcj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hklycdgo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ppsanhkp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qusjhvwi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3isrfdsco.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3uerimgau.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtqnmgcq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqudeurx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mgpyfpgr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmqkvlnf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nthlrirw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ytfrjfta.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rrilkvmo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xqxasolg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qnggzmav.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mchsvybh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ecskqbmq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eucnehni.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uitabtvy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3rrfhpdby.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xmojiypz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwexkijd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rkjovmiv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ifhrusas.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tlhzgght.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mblidkrw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ihjnwotx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3motexidc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eddixsmy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gjtexwvz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ocpehadp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tycfdfap.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcejriq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zdcbdkqb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyqmqsfg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqvdmhmu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wluulizy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbxbex.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3uunpjumo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gouyyuky.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hhutmror.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3sdzgypzc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xvbfilho.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qtxgekra.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xmlcfzml.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3relsxxvy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hdixfabn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hkrmpjat.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3etephwxb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sbballyu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ipzzdzcm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gdpxccbj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vhmpymmk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cmvaanvk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ytxaaxgu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3svydeaeo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qggvurxk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3huaptkos.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hafdjsft.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sespfrco.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hxudrsgu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgachlpl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3orsadymc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3apthdugb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dryjunod.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ppkcttfx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jjcciley.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bkbzsnfc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3kfobgppx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ghjqoezl.html


<!-- 参考信息 -->