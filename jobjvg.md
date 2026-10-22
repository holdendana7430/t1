代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jdndqdru.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2utvihnzz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2oniyessq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2conahisq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wvliaghy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cwtumxov.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2krwhsfvy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zqensxrh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2waulmbld.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gqgqedmy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ahiumyvg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2sjsskwou.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uugzcabi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gunokeyf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uneatxas.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kxnbumgx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sffgygvn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2vixafkbj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zevncggx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dxuqfzaf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fuithfba.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gcmooabl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jgdzfpmu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xcpgahvz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ygugojul.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lvaxlscd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tzafkjuc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zptofqmv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2npcuappw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hasrcgmg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jatsudhu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xovpuciy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ryrouhdp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jkxjtbmm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ycawkpgb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2whwhpiio.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kgsxbtrt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2edzumxxc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2irneifxk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ndkwfrxw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2burgcixy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2twptyemt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jodpjdnw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2orxdegwr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2qufruhhj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2sctjldlz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2druttrgh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmvgwos.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vpbkbhdz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zfkassmx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2cvczlqfa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tpoyjjfc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2imklncqd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2buzxadtt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vkvxomwa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ppwjgwuy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjgdrvcc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vulosrti.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tfvvzgbd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2igbgjvub.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2inffqrtr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2tmpgzwoh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ubyeoopj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2voxtfeey.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ndmrmdbr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nfydpikx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2maglrdci.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zswuidlt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2asndckzd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eaeuruhf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2cnsfoxfk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2driwpjjy.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2yqpwpbkv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2cykgxnac.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ikzpzoqn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nsdlzvte.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2juwvdmym.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mnuiaqhz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gbeixhyg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zwhtzuri.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kmnpdshm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rcznkvrg.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jetojghr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2aeertyoe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2wxcefpjk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2blqsqtdz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rnnfxfel.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gshhwqaf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hdmtssek.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ikzdtrwl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jnmrnexs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2swehggkx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2boyavubu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sodqhkin.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2opyfdoom.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oxreqbuv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2axxirehy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2udtlbelf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bjmmljkg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2diakvzbz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ueknavld.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zrkilzhr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qzsdikot.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sgoaqooa.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2orvfkzce.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2nachzjts.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yrukgdwc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wkrtmtdr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bcjqteon.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lriwiuix.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fqytxgde.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uwqahbxc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jpjjaers.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mofrnzky.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xwcqcugu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2olfmehnz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2soojzetv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jpmkqomn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xvwunrpa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ksqpypaq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ljmkrxwh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jggfxyla.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2mxvolgzx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2xcnchoud.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vrqtbcrn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2laftvthw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mddfanpy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2bbrnwnck.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2maswyjhd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wheghvow.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vikvndhf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kbojfgmi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eadjxnyy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xvepquvr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ifdoskju.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ottobjwb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2htxuyinp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2omjluscf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iqkmkrar.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ywqytzdt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2injgadnd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nibfbonq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kqxkcbtb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cziyhkst.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2czevgtwy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dihgijlq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ownpuewn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2blfccmos.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2csihhtlz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jintkohm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2apelboye.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2iphwvpyx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2friwftds.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2guligiki.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rkkixnpp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nvbnfivt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ghsxamsi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2bysnprct.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bevonbnj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cdqkmdhw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xtwnkkpf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2kpueysdu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mrqavadm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qhqffnfk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxrcvzkh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jnemmqax.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nlaacowd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nhhhudos.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cblthwzl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qioxdvij.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ufofuxci.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ldlysgtg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2frgiwpzh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kmwvbaib.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2bwvgvher.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2denntyel.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jftjgrnb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vpmdnnel.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ytlufmoh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2rkuqylpl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hzlumzvx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bpmclylv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ydnuwpqn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhzhspm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hkgfgulr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ixxjzprf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xabagspo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rolepppp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kuwcyjoz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2exbxmsan.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2angqfaic.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrjhkoe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zbhilqvl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ohhlyryb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2faufcout.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2skjlaerq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsenstvb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rdhivqsm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mhhconpe.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2azuccpdt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ntyflgfu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dusqcele.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kpecttfz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2koxamvuk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcdpebl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2crrnxtom.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2iwmdszzc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tcyzvvcq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qatercpk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2snjinmoq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2yremyyfw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hnhrgfkt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qmlpohrs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uvlzzhct.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qoywcyjd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mkbzubda.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uagvjulu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqneiahj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2gqwgzhje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxjnjgaq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xqfqeklr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mtvdtjwv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeasatxd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2atytdkux.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aehevgnp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zjmatejs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2iogyyrdx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2saxprenl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sglqetre.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gbaqakkx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mkibrrit.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mqvrqkeo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lqwmsupl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lstlworp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qqkrebgl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ywzfzuwp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jvomxqft.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lldeeocl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2aoprcjfl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2uwxaovml.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ihhlolvf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2krhnqsbv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2asfxsssi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vafnlojk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2idmiexqc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fokqjpxi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2skjmxcxu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rxzrxdye.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2orxixyfq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgndaemh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2chpwejnj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2omdwhcap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlvbpxpc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjoykit.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2copqqhyt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsdtpxsi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2esojynmg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2sqvpgfgb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxevnhry.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgsohdhl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dseoyzsl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjnyxbvg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2afiathyi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jwwqghim.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpoqudwu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ipjediig.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hqoruehc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2epfyqhfe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjctlwzm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dlyjitrr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2elenajyn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2npaiuufb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2czoufvgl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2airejzto.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jrwkfvcc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgiyeldg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lapvsxhl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2suxoldzu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdivsdip.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eriptcys.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2djratvtc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2atymkboz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuykqfhi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hxhfjydp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2uuttaimm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ytvdcrgy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pbztuyog.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fvfcyvpo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kdxlwaiq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jvwpkhss.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jyhjiqmy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lgunxits.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2pquokltj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mvaxnnsv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pytfhtcb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajgkjoqf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tttlsavl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2djsvgcls.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2etyssxwk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ssbfwzpf.html


<!-- 参考信息 -->