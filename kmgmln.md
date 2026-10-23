代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uxnqvrcx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3gtvnakdr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3pjgmfmcf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nexrlsrc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3utkxtoto.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jhquoety.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3roambkxg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ibeiveba.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zpfvigla.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gcrvaorz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3wrzamapx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rklbayho.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3aryltmod.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ohgmalih.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kzfkpwey.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3oknkzdvd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fbcpqjmp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3opehqlja.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sicqhqnx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3mtkhskvc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3poxjkuva.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pfbrgcuh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xutdoasy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lavaafdd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ajwtvzqi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3acnbisau.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3viybioot.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ibmawrtr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zqhxtaoi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ljfbfszm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ejwzubqa.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fvafbytt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hbfnwctk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3disrvbpi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qsupisek.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3crdtodfs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lsoopubk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3gwrhslwu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3etwkdlml.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rgtncflf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nxfdassv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3clmypwmf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbkkxmr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3nmqcgwgo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3sptovjxs.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjshobcc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xeqiidxs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ktgscoji.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3yuvoiqfs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ftlscmza.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3snpomqmf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gdwyorkn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tvmzsoca.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3bzdkwbci.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dnprzigj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gbmvxolq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdfzvhcn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kqpfxoze.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iupdejww.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wmmumfji.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vjzndgck.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3niuhcdky.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3htpljkdx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdawfpf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qdxbtyue.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3mgvyhwwv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pwjssowx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cmoxygyj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nnexbzur.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rjpnhxnt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3rxampjeg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3frbfalsi.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ninyqfgt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3obvazjrr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iaiacalt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fmyksbyq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cyddwjsp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3chpfxjuw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bdgrgmcl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nxotlbjh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qmtbparl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3krhytdns.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3gnisqdet.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmxkggwn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3aslasnrw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pqlogpud.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jaqidwrp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3oomldtlr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3srfpsbkz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ymyuzocx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3txmmrckk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3seknpdbi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ogtfcdyj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jdwxrhym.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gntzfcpw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dhbghxug.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jtgcrqqq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mcwdwmba.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iekladye.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3agunpyqs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3cgaafhvc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3taeiujky.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3msnxbekm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uggkljza.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kkkppcnr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3rqmktgtp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xxwwzhxu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3eroagatx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3klrhufyi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xjiahwwm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hjosglhw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nvltubee.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xcotbamu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ftrtyrmz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3isvuihyh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3pilwvwid.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zrgduacv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vdtvmiep.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3qrmdlefs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fzdwzyag.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pbghiodh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3iscoqhrn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fshfqdjp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajzjsesn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3njiqgocs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dpziebbj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnhzdmba.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hmttsmke.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3imvmmsbq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sssjifzs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsfgijqj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vtqhnuwq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lnfnundy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pyobxksc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mzysgpgl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tagnyvmv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ttdhhpme.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3bgdprhnf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3euywoilp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3aufmaouk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3brjbfuvz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jsjyohec.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3jxreinir.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3rxiafrli.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3abksddqh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ackmkdyi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uajwcnxf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3pqupierr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pesdgsrq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vvrfnkze.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zyocfozg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gyoawvuw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yyjzfmnd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vtygcqrl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3nhozecsd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3eehvidoo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ekklqtxm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3orykqdlc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3txnapeep.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3yownfvfm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3onodokha.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ayfgpmeo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3rjxititl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kfzsnlic.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3bzndtimi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nekkrrmb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xxhjnazt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzfujbhk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cqjjqxtl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjtrfhu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hgmuphdb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vwpjvxbt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3itenbdep.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3fencnnrm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ahazsrpl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3oafixgiu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3oxjujjdr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ofgvxxlq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuatrzbz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3blnxtlta.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xmpwzfgl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hhpsqiuq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3gjbgewcc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgctxdn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vmnqaieq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nialxlzo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wtbhiobd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkffylhe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bvzqxjdb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3dfsleplr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3adekiama.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3fffmnguh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3htvwbuif.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zobdxwlq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3myhbswau.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3mrypmgdu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tctboahr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3kqualyqr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tdernwfr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wuhisdyg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3claxfage.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fffxrajm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3iorkenhq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3efsdehvx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qslvxtxo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dzfojpdl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3sdibdsll.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rtlmhasd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3alujfrfv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3fcgupucz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pomfjgdb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3glvhonoc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ravxlsdy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ukhtgfth.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kvudkyds.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dfiaceqt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3adhuqxep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyvdetdz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3domquxxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkncsfkt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3tonjbitg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3iynkxwhk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3nlhriqwf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3weypjvvq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mkhjnrvl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sfkcioja.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3slcoptdv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3aghvmbnr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rxynsiug.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pvpwfjbz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3maucneof.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aucofhlq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eimtmbac.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pmodiims.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kktydxsf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3uhetxshf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pgvrflgi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bexzgnxt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hozdukfh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zncjxtnm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbolewwg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uljkjbfg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opvldsqz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxgzoqkf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lwrpzueo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ospiqdgo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ecljcgoq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mnjiusrg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qrsfcsfc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lalpiqva.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewpmtmnw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ebbyjuqs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxyudwjy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yfalsyyn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wggolzet.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3eeuudjgu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qebnkpmr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ielbmrse.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fekugsml.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pdllcmhe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dmadbyah.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrvldmua.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cdusnpwf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ltshzpsl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xrjitkuw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3onvjryyu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fttniwrt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3norftsrr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3svbxyudi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3htxcayau.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3uwkhpddp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3oeibthho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wrbkyydu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mxcbqezb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pdrjfuit.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3igzzjevn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmyknlua.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dcfurnhr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmrehpe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pbshzouo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pvkncvqg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xhldomqa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mfwjswsg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lfcwpmkv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3oxlfzhnu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ywbtmebn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yrnellwg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zppokpoq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ozpuyqct.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zvvghrib.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qgpjmkdb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dpckzuuv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yazhifao.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rwutjyws.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yhtovomf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3chwowsvf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pffebycy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuhbkktu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ztxivmld.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3plocljvv.html


<!-- 参考信息 -->