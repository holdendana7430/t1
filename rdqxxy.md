代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pjmrnori.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jbbimjvs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wvuncpkz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pacfjrrd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cfdrktsz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2raflqlbt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qoksjdzm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2whxxzkoc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uurekzmw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2yoydxlyh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2kneasgea.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yfcfivpa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lczzvyzh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bayiqbxd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mapxydkv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gmghlrig.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lrdpbtro.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fsgjurfe.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2eqxgkjbb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2dcxugyhu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2mctotllk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zxescsxf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2regfppff.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2numtkyiu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2hdktwuzt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2spjcsgrd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2pkicravn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2thvxktim.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jgcuurbp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zshoaxol.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nuaduoiq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mcagetzo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ksqeskcv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dfmywbor.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwkhddtu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hzpqpvkr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qdjglmvz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2coxgwwfm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2oprsffrm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ccrmoqjr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fgkqtpyv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xnqrahvy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2moaikcot.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2mwcxcmzm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xhsqvbgt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2akkmqygi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ijmpyvpg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2rtwmsnmx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2harrkqun.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2nujbliuf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2npymmbxf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zvuuqzfu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jhdaludj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mvvgljkp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mmpjguun.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ohwabxvx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgyyso.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2twzmszqy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xrbsrgry.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eqnmozim.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zlljpvse.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2suovwxlz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmtjvpp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cpzzbkxn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jcndbryq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfqzfozt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckffxhop.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qujgdmjj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2laqajwmk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gjnjmwsh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cdszihmn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2klxducqd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2gspharss.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2kibnfzmt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2yqaatmky.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ubuvtepl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rlrsfsda.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nhvfgskl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xexqvghf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2pzrsgbvw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ffytufnd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2fkpzjagh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2erhfikqt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2phtdwxad.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2brpysjsb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rgxoftev.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zxlfrufp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2twwqllej.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iamtznfv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ptmjvpes.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vnkndggc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pyfgwobf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vejdxgzl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ypcqyjvm.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2esbwgris.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gocbwdjf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hvklgtwv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qxkjxoao.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2iwytxygt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2owmrpmey.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sviglvzr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oyuwqeoz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kaaobmxv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eneanmzq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rnbfshgm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2asyktrww.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hmfzmqpt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hcrprkeq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kggsevyx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qkpqilyb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tzdvgkin.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zmfqsgow.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rqwsbrvw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2gcwggnfs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sbgbphtd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ulzlsnpm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pcwjssnl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2codpigtq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ksuhhyej.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ifjrzdbm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vmkkfvuw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2axzcyfxo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2kvxkkzjb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dymkrrlu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tqelxiem.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ttmklovj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2liywxbeo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uawoopzf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kpvyfjgq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zzcynfpp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2fpovflzb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rargvggi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2cdcidutl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hrxqsomx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qeejhysf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ettuzghy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tshgpvvg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rvmocads.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2inysohve.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqdbxhxc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kpfoplef.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hdidfhwf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tknanoye.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbdvuypq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ewnwmyif.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2oooingwb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cdvnyqkr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2seqrcysx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kgokmrxh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gnpddouo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bbkfzltp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2skszupiz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2qvtzwslt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xfridvfy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2neuthsov.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2fmjbkkrk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sqigupae.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lwvmwmzv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dsfspcsk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bzkrkqoh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cbtpnajm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2shdymehl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ehkmazmm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2vxtmxwhb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2hqsrzhby.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zjljmaiy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2oxkdmzvp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ubgncaby.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zszbckhx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2hyfgmxda.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xxziihdz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2nzyqzwmk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2gxrsfcow.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fyrmrcnm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2byyzeqbl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntgrrtxk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2itsdybuz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zupjfmtx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kidjdgqt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2maxydzpy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2irrvyxbt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vstbrgyi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2oozquwml.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jzxvdpfk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2beiwunom.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ubbbgtrp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mcixzjtx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ychqkspr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2chcjfnlp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sqzeglnb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2exfxfnmq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdivhhq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aypreibv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mfxqlbnd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jcyhcvjv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2qjmfmxgn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sdubsetj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xaogralu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jaygzvys.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hfbkvoto.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2aulkaxts.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2viwnednn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yukzmmmy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2imutauqb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2heqsutbt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tozfibwe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cmuatllz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bozzlbgo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2skffcprk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2caayznfi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xebmjraf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ikvyopfg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2hwngqkzy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lutfzhki.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gnvngwph.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dcylqctp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2clkfgyao.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xmvwgkce.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kckzttky.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2blgnmijn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2oyowejkm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwehiby.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ypeyqege.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ogkhziug.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2thkpjgnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aecwsxqy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mzbfzhli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muzrjrfe.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bwqkmsej.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qbtcfemk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tsxfvkrc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bmlalvwm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jujdtucj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2esfxufms.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wuriddwb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tzhgqotm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tswchham.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2llfmbikq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2apucfkyc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lagcpqap.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2csdivhod.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oxpjeujt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qfybtmoy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2oizrqhvc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gpmzmmur.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lqeysewr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2gbjdkkrm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2dnpwsqwb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuluaheb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiwcswna.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gmteiger.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kkixxoii.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2skwpxqbm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2napqcodj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bvdxzylh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eaulqssp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uajuyxsf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2egvdgynv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yrmmrkqx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ertgmnok.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2uknehpfm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2retoxpdw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2omaxbalt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mfvuqpwk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ubxwjhfi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yrgfnkoz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkqwtele.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ceazobem.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mqujsdbm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ulgyhcpl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2svqmapfn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2nldqbecw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wfaehdfw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rtgweely.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vjthksse.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ndazilbj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aeaoknmq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gayucfec.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfjgjqlt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2egdorrvn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oxmbaroj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dcnpyjxx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bhtotyhz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2huwwcvma.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifsckaun.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbjzbkk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjghdpvp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qjefljjh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yzuplwjy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjxbywxw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytomwaye.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zzhreckk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xphcgwmt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jnenhsdw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gwrnbnto.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lvahhysl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ellfgarb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ydqwwjxs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cdphzllh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cvfnlzxm.html


<!-- 参考信息 -->