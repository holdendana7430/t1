代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3psdigcmn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cxxosnbk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3oosdvdss.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3eeruiuit.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hqxlugrf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nzlvhgen.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3cpgsdtfr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zgfidpbd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bgbmwmvt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nrzrpauv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cjeqhfvb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pjcvmxfa.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vbjkzlcn.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3acyvjpjn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3oiavnidj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rorpoykk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffmnhirc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3falsyxoe.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3alpjnpab.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nqnwixug.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3wsaxrslk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3plovatke.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3izyoyudb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3xkkrolcs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3npksefsj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zzsqxuuu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxiqzy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jujuaodx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vexmfvve.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kalbgyzs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rertcgwk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qhrmqlxj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hngjblcw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbcxnvw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fpdplshy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mnudsgux.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dwnnzdva.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mtrevxzt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3skurwiyz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3qzeyjrcv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pxaiiwzr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3eaqcrzia.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vfntposp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3szwfkavm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3hftfencq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3iimbpkxh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcbovuj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3gzhxpsdy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3prhrlxil.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3tvwnxjvs.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3twoglvvr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gqtmbgms.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbloeipi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkcyvde.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ydvdbcmy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ueuquoqv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fdhoynhy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hqpmjzqe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3azxngrul.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nswnypbc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uoylwvii.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3whxtbuls.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3krrdvlbb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lftxpjwn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pravxcbm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3qkcryhfy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vqtucvot.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3errlplqw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xdntibqa.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3dzxeutkw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bljtzyda.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tulabvix.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3snpregkx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3aazkwwvq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wfzsjsjw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ltcrjmrw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3fskjcylo.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3opavhwbs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ltxedujn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jmuqtooz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rlqwbaxr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3shbrctly.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qojaxtvm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nvdhygwh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vimrkjpb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3anzbxyza.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3maccoafl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3mkcvutvm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3zpuoabfi.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pgbardgz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wrjcpjsa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yomjzioo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kxigajsb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3dfoigcpl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3evihzkbc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ohvuidcx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yuiqtoqm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vkkuqxge.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ghjdlytv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rpwrptxf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xnzboyhn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jkoklqco.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3goejslsv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sqpwllos.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ahiipvey.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3poewosix.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3joqctfbk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3izsokmdw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lhmswwyq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3yfwskldk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vcawlwnw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jehxhhcw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kdaxrphf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qraukmht.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3inpugnpn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pchewurz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wnyhopbg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lhbckgne.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3pfxrkbku.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ohoqewxe.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gqstyebv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3glbibnbb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3htoeuovw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fbkicccy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3weovqkwb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3srakupkb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3igrabqhm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3gsakkmpo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3eqzwbtjw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3scwmnlne.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xfvabwwe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3avmahmyi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hmfspoma.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vnmxltzr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hzgjlfbq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3brhtrvwz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzrtlsci.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tvkzrxdq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vshetpql.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdmcjell.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3zkaewelh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wlserwbc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ycyfoyru.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnekxls.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lepxfijh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jktwesbt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3uksmoaba.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ntegxfmi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3smtbckne.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3nxrhqwvh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zprcdyrd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hntndyhs.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dxwbnnwf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fwycwlil.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3uphcviqm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hwmzkvua.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ypxgmcfq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xdfduldo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dlcvmvzl.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3gucmehdj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cxpbiubt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3itsmhlpm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3szegluwj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3erchblyz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gnmgmhmq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bxdystnr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3aqepjujm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ljexrkfr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vpljvrns.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iwbgdwfr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvmxlxsf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kulmppwp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gufiotyx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbtxzzj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ifdustqe.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3bxxvhmmv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dqwhyvdn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogydseuy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ppnzzbtk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3appwwzny.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qucjlnrw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3brdmulnp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3cvarvwdm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mdmjfnlp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3alduepix.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3aybctyrp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tkluvwbh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3wwuwzdwc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ihyyqzyu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wrtwuvol.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hlihooqo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gvofijwm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lrhlkbox.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3opyhtick.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hceojjij.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3stpekuzq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zzbwkjyw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mhhlbnms.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xbfuluws.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fuotkpwz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3xaunfobl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ifvwledz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ujhmbmui.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3somqdquz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zlrmrtlq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3xnocobkg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxqcowx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3occdtfez.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bulbiqmg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bmcevdkg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hrnzxmnc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbcphbfv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nkgmljuk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3debshsup.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3rpeoneqi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3awgvmzcb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ucomwdyq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hlnflwwr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3fbtuxurn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3dkorlviv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3odktnmvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avhyikhm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qarikbhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgqnrsdd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lugqmybx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lcmmnzdk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fofiltnu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pewngtex.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mmbxozvd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sutxqdfh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wevbyugl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jsixyryo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3haoxwdps.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3frrztyvs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3kztarwnn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vosmxlsw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sokvfxun.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dqtwbmic.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bjfkdtph.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3loithxnt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ohvagsel.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hnsbknvr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ifjamwal.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gjswikdp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vqaiyfvn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmywceeo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxuczdag.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vskkgdkv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yuzheeuq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3kpkwkbrc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kfxsevlc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3piftzrdh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gippouoa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yylenapt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xydmiamr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnwtitgt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3akpjfbyx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vysjeybk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ihfvxdkv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjffpgwj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zcrpepcf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3knqwrbmv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vvklpmub.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3swrqokar.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aadzoadq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfmtisca.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxndzwdw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3klhjwyqy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ubiutyjo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hdczlgnk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kldpqbgn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igeqjaoo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jiayfcfd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3boaxnggo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjntjmdn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hnzenuxc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jzxvzplg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhdyiyak.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fhtxmjjd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mklvgkzi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dicythlt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3atqxeiop.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iasglnrc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3louckuyz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wvosqygv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cyjwesjm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sccbhmnr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zzfylpwz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cflarvme.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hmzqxszw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aovtyjdm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dqiljoda.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kdnwywuq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jlfgvqmc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dyernxos.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mcojuqbt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3agiobdqz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3myxfpytw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xcozjpwc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3atorvuaf.html


<!-- 参考信息 -->