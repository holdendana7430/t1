代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wguxbxgh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2oluhtfzq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qywhvjfk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rojkbkqt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wlwnoaxa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ycsikizi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2kucskxob.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2yurjzxpp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2muenumrv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2wphrbwfv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mwczfrwf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dwyrwubr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sotjlavl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kcbvvsej.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lkfhxqxz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2javmbcfv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dgfpytli.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jxphudsc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vsnkuhsu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2psxbassx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ufavpscr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ckkfguyj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zixjrupk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bzcoqeny.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2flyxaawr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xcovkbdh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ujdlidoo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2glegmxsx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2yhgosstr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hasdiktz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lkvpgspu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gvbqdxey.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2glkwjyco.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tknotcao.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jiqcdvje.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2melnfrka.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pfgmagzc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tcwkiijx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ksgjimpc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bxhglcth.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2scfilwwj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jmbljxuc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hkegegiq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2arjdrpuo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2omxcwedt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lewmxkxn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wzchplxy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iixaupva.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ncdtufbj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2fuydnlqb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bimjttzi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nvngkfmu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zgygctdu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2vrgnihgx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2efaobexf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yxselrtb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ftaydwfu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ezavpmsw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2bayyazmt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ntysvmwp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fyawtodr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2whpbevvk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ureauogk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rwiqynhe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fkpxsjfy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppawrhdm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqphxcdh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qkcvmllk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mqgxeqax.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xazcfroi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ivvuxhoq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tgoousar.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2faboqhwz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ymnscxvu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2fuxtobhd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ckftgtuq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hnhmlqta.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mmogcamf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2vtoonaei.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kquwuefb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2grtcctuq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kmgrznko.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hyksbesx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dmufseav.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qjwaudzn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ngzormxp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sshpjmru.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2clxbmdwa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tuuozhdl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zfojlcdq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2pqsnpblk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2szilkpib.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dwyhycpd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bkqbnvcb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pownwchv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rwfmjfeg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dclmkzvh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2nzlhlbxx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jclsiczi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kjevhiua.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yhifrxlo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bayhomzp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2blghidqp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uwshlhrb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qzmtpxhp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fydauakx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kbxwypky.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rjyqevpu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xucvnivt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wfnscfvv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oezjedyh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2koemskch.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tlnikpvh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lnvdmyoy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dmvmioxr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2jhlfyswr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2huhpbzmb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2myhmxqmc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2irmswofn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lrgqkzfp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pbziryob.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kyorbrne.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2plqwefyc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2jglkbzah.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wfvuavtu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fohiedpa.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2yzrbcbok.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ozulrgnq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2rsktonte.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2btzxnlld.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2njhiftpj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mndedzsj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2qznxccbo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2abkfqlks.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtfsqzwo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qihubapv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zygktuad.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2clofathq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tndnkomv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xeetrsgn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zrqyfiqp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2etjpsews.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udhhyolr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ccgnbhkx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2inshdipx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2odtmqzix.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ialyoaex.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mwlaoigj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2alpstasy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vvckjiek.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2wmorvwhg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dcmjwutm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2antzhdcd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qzykhcfz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uzatpeir.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2xwkbzwqw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tbfeigtr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xeyfbxbq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2lqsuvzrs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vlrtaoeg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ifbdfqph.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2wxxrxlrt.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2iritlkmw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lxudmjeh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2zmyapppg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xfamwkyh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wesinkea.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2lxuhfhvt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zmlufeth.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jnvrozqx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hxbefxmh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rjuipmzz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqfsnjmp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vwcacwfz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwazara.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xguvaftw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yttuleyo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rralgbnj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dtvtvmbo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2dgmlylvk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lnawjkky.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wlgplbkf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2prceyujf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ghkgtxpy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wujrchkl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2buezlecq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2enakgwbw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dulmdskt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zvclrtnx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rdgvefrv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2efxpkqvi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sftoxqxk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yaztdjto.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gkjtqtkx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qgoutbow.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blimquny.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2alasrqvo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hvzmhqvd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ndghnbzx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2dpglcvfu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzynzxtv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mowysumo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mxugnseg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wzaaktfj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fvgzusve.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xelzaizo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2frkdbscz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwiysekt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hpjmoiap.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ytbpnnho.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvlibsva.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dqbebygc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pakwdblz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ishjqmdb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ouqhxjyj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bgxcddif.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2niffnbar.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2etqlwbig.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ytbfkhkr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2uscaevek.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2pjgkuauy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wrwhdyjj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ldqsdyed.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mynqareg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wnrjyuwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgdrskxx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2loqtbvnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suexmyde.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uqggfnkr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ymctiwcm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2zlqkeyex.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aadjojlz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2crfbrzsp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dzwbktid.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yeivtjcb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2enrrazjk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ljqpsoyd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mottxgsl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lspqnstd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2oicyzede.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mgykuhuw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xrlnevrj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ehoxuxxj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lqwcxgcq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2enqkzvku.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sqqwtqgh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fygvzbnf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wsmissyy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qabbnaln.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubniftpb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sckwltju.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smlnkwyq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jmnyrypg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ttixrumz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2crnwwwlo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qehptnfp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qmdibyxp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hyoucsvr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2watknrth.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2beozfxzj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jibuwmoo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ydrgomkx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bfsxmzvc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcwueklb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2snlgxfvb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hkjwcsyf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fcgtvnjg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsrhxdkm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gvldmoan.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gwnypdbf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xbbdqvnx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kfhklfdf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdtbfjsb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2oifivrmd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dujotasu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuizlxbp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fljsvfgl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wldvrozr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2sldyqpsd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vcmjmmgg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pylrdmsh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vqabygvp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjafbyeq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2teqwmxhf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rugexyuq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvinnrsa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtsliypj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxrsgjo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qtxqxwce.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hcobayuw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bhvsiizy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yslzwfot.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xplcotho.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oanzuaop.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hsywfsky.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ldzsposd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vzttgsnk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qbwknpcv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gljlnhou.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ilxakftu.html


<!-- 参考信息 -->