代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qqwxaujx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2clrgcbed.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2emymcuzl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cugwkrmp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vxuiacvb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xfuprvul.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2jlnxhmlj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hhrition.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ltajzxhe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fxuqjbvh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wblrojqx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sawiolzq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2fnqnwdwb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cnnmhspu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2plaxwroi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ijwfrbvf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2axdvdbaz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2zbufyagg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qngqshpr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2izrezggd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkrytotf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gyeehvod.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kscfgaoa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2curixzjw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rgxuppax.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pchxdvmc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bonkbppu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mhiaxcid.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qmlvsvyj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yddrtwhu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kxsrsccc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2whuonarg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2scoeybcr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2clonvqjm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2nqmpvsda.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2wzemhnwi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vnhyxyfp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fijrsfck.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rijonpcy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsguemnl.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pwqngxve.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2likfaagk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kheqabhv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dsohhnqh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bexqozto.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rkzjyhca.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ouykelpo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rkhbzsem.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mwbkcoyj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zfbpnhiq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2zctonkyv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2wpkqhctq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2arfextvw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2lqbywkrg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2otwpojry.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2disxjbqe.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xcvexlpv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2tfbpybrk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lnusalzs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2cbrrkrpv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2nvnrdjmi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2htxwsuhp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2iokmiuyt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2omipujmy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbfjdyih.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fiirlgyh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2lvmkoveg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ukgcndgh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ccdionca.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2kopkzhsv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2linpvrby.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wfxwhrgd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bfnfsgko.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntfcdtge.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2imkrnyvn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwwexqv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xikelpwt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2wbzlgakh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2txvhxtjz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzshwjp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2behrzujt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2emddopnd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jdwmzjub.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hwvrrdpn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yosgkklk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ivjybuio.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nbbnjngg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2moaufjxf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2bpqjvnvz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wpltqknc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2hfgfegfh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jgklxhjs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jsvvilkb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2agtbpskd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hvtuscek.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xdhsvqab.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ccinwqhf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2swuifckp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wxeouwja.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2sjbrkpue.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2cwvktdmr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dcgkswoi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ymglfvbv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sdeiwkei.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2yubeztzf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2csgkguvc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2tsteiauz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ksulaixc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gcbzanwb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kblijzil.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cxtyykso.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ksmpyswh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mceqyblh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qiirekpp.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2opoplcbz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ckeldmpt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2unxgwpkr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rdgmlitp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vggwjcnl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ewlanjzn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bhuhhmkv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2gryrokfb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gdtqqubw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2smlzvyoh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tnnotlfh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2gqvlwdfq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xohpjmlt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2amdfisth.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wkwutgir.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kioyieix.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xviveplo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2vwhutmmt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bcilotjc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xngjbfax.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2peahocbi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hxesepig.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qqfstixt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vvtynxvt.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snrfdnxb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lkhqqokr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uvhcriam.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wteqgnlr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sogikngs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2gwqaawqu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lhcrjfxh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vaihqknn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nxqnjyty.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tavbflje.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bkowxfhs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2krfsrsnu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xkudwcdg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fdbhhnyr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2adcqtcep.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxxywtg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ripkcgna.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kwqieiyk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kutmtpds.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dpbigncq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2czaaczta.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qwioozeu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hnepwvxh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ucuedtfu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aebfzjim.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ftmjogzb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xizjnxea.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tousblcq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2tcklyhfj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2srlhuacz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ltmggcbe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rlbznvoc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2rhxdikry.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kphtokgm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2gizogyst.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yxcfaovg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xeqvseku.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bdgwbtzv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2mgxwbyta.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ybyifbie.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dsvvbyya.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2yxugkjnw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2quvohxpq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mtifivir.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mzphdofe.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dmsednop.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cmonqtgt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rgmdfhfx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2akqriacd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2asvuvdcm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ipovxtpv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqptirn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2eaiuubav.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mwummjty.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sntytxsh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zejmwnbm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2gjygulxy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aprbhivi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2otxpdoae.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ilpeyhkx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nbwreutc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wcinextz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cjxgczri.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bzhvqazl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vjcpmezq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2egxtkmcq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uugabgtd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jwcbphgl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hpchpaxm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jujznjkz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2avymhrpq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yckiukup.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lzougstq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lxiridgu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2dalvwwkk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tnqrqgdh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hwxevqak.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2awqjvfhj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zvatkgzj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ziwausjo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pdcaboyy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ujjpmizr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntnrmccs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyztuulk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ninenqhm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mumywfrj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ytgagdfz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2iflbevja.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rqtzqgmw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2czmxdniv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qefpiezb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pfprruho.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2edurpkhs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dfaihvgr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2usyitboj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxugenlh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2tjlwzdru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjdgvzhd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yelgchud.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2atsodexm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hwvstxrt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rcbphdzm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2auicimfo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2grpzyjhy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2yznlzgul.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wnimwwdw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ukdphehh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lpufxnte.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kcbckswt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdajnvu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pulfslwa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lvpwczql.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cwrbhgzi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ligbboxs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ajjjfkok.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2swkzqwwa.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2grawxegd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rdizivee.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzspsbac.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vvexgfde.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tucbdvqi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tdvamspj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtvspnru.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xwypjpot.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ulxxsdar.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2epbqzwab.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nrxzchnz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxqvoaas.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcnwiffu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2orkcqwmq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2szqjbyee.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2thzptkrx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jruxmxlv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxnhcmcl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rngvdqgy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jkaegnoo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ajzsixwq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxhmpnom.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgbgouqh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxktsil.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cmjzxlwk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jqaygnns.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2cddmlkgc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tyvxzjaz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jmiipxub.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfqcnlwl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2extjwqbd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2juhqujup.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wlzovqfg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ycyjmgxy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lhinekcf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rknelgpx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wwntugfj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbchtcyy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2guwjrbmq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dshopdvg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gvhllcjj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2znqkijko.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yqtrmewu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mlgtzxtk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjcxrdk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2itrxzzmi.html


<!-- 参考信息 -->