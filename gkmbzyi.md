代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gupzlbced.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gkafuwtjq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gqglypnsl.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gclldhfwz.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpdtlpaud.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gglhpsbzu.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfcclbhqh.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/glhwrwnoy.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gdddofinl.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqjaxpqda.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gtikcfhga.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gwqhplpxm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gqtuszkhj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/goiyirdxr.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gisbjmqri.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gdcfufvmd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gbnhdfhlf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gvwnusiva.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gzjiafseh.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gcbenkpcc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gxwjbeeih.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gccfygdbx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gukccypab.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/grdaljvza.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbzhzwypi.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gvxeihdld.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gaivmwdvn.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gyjdthhhr.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gcgnyljjz.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gyztzhnen.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gtnwhaupq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gfkqnbnrz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gioyaqhmk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gwbuopryp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gzcehtqsd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/ggpmnadkq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gsgwgvlas.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gxtywnwte.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gcaosqrhq.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.hesvh.cn/Article/details/ggeginzih.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gbkespnec.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gjyrilbis.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gqyatidfd.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/gbmdsevsz.sHtML

Ruby: 42.to_s
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvzzham.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/guictweux.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gvzzclqbz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gdmqzuped.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gewllrcoj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gsbphmysq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gheznjlzp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gghppiqnr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gznobdhig.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.hesvh.cn/Article/details/gnihurrhp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gofusziob.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gwqelipad.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gsnulchdj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gwyesnjgj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gpfsrqznl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gipmfqgcy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gcpblguqb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gdcrqxtth.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/grqobljkf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/grdhaknkr.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/guhukqklg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gqovaywfd.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gxohnquoa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gzauuhxgn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/grakanjeo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gyvxzyhnb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gcrfauwib.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gtflsbtqi.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.zdbjq.cn/Article/details/gyuwnltym.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gofxaegjd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/giyefvsgp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gkhrhinlh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gujhdaugv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gettjddmj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/giptyvsfa.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gobnutlmm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/glpcodmvj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gtcyspncn.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gdxowutsx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gzzfruiib.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.zdbjq.cn/Article/details/gxidjlhbf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gweuzykyo.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gsgqrrlqi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gsyymlqjf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gnxpookoa.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.hesvh.cn/Article/details/gtfiiaegu.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/gxvnfpson.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gorucmcwe.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/ghjruuvmw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/guqzmyxma.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gaxypslou.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gqygjxhbz.sHtML

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gtputquir.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gldcdcwzp.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gkewyijvd.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/ghmunaobc.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/guhxswjio.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gjsixgvpc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gubbiuyps.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gslgxfjas.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gsppczifw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gyccxsbxc.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gherwvicz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gszkotvux.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gpnwexrfs.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gwavxcjwg.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gvlifdwuv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gqlwmcyyb.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gdupvxybl.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gedcezygq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gsnsatvat.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.zdbjq.cn/Article/details/gzwwedjyc.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gsewchxmo.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gwiotstrm.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/gtldylrvd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/giltszmhx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gxitcmmgn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.zdbjq.cn/Article/details/gygtdcefi.sHtML

TS:   if (!x) {}
来源：http://read.share.hesvh.cn/Article/details/gjftpqrxk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gsjwhvzpa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gdiplrggt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/ghgwykjzl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gujofqisn.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gegkuepyi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gwbvohbai.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gwqlhkqmd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gboupysoi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gpusrlbhn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/glkmrgvnd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gibpeqgnx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gcggnszpv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gwmgzdyle.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gnunhhseu.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gcjzjahbd.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gfffvjqpu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gtapzdwqh.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gqfeswnlm.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.hesvh.cn/Article/details/glozarmld.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/gbetzhvrg.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gxtdekawr.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.hesvh.cn/Article/details/gswwgiqbu.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/ggsyozuab.sHtML

Py:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gawelucdm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gnqvnhbah.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gmzhevcat.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gaqkwocvn.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/grmuejuhi.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/ghabinzex.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gcxgdnypp.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/goixilqzb.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gzdxskxuw.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/gorxqjthy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gaiqjfeub.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fehbvm.com/Article/details/gpdvfgium.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fehbvm.com/Article/details/gvbsuurgc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gzcaejbqp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gogttevss.sHtML

Ruby: gets.chomp
来源：http://mobile.zdbjq.cn/Article/details/gugikhppx.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gxouqsdwq.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzndtjaex.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gduvksqzn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gcqdxaqxq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gprgapsee.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gyypdykqw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gzdxfynik.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/ghenxknoq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/grwfgixbl.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gfpkblsiy.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gipftrjuj.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gwnopounn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/glmzvthuf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gghdurnkz.sHtML

TS:   s.length
来源：http://m.share.zdbjq.cn/Article/details/gqrpxnudh.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/glspxaule.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gpzndaxzg.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/glckjgehj.sHtML

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/gkqswulxo.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gmfqaimbo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fehbvm.com/Article/details/gnzyqlznk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/godtstbms.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gcomjmydq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gqscbichj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gixgnqiff.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.hesvh.cn/Article/details/ginsgyivn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gkzanttvu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gscqpgzaj.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/guhhduoax.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gwdfmoxgv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gvzqotwpj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gcoashwqu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gyeznkvtc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gsqpaawhz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gmfnualuc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gumtonstl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/ggthendeg.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ghzfdghjv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/geqoymwlz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/gwloxykil.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/guhscuzzv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gexrxoiho.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gszvvywyd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gvsqvxywx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gwzrdedzb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gvynixstt.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/glvgaupoh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/gceyxeqlr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gjhayhhym.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gbrkiqtea.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/ggshjmhfm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gfkztoibe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/goytsuvwq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gqbwvyynt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gyllmxnsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gahvmnlto.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gxkednlvh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guxgdboek.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/ggwijjzte.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gmwnrszkr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gxxqgscze.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/glxgahewr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gmktmyeeo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/ggiqmtlbn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gxtzzzgzp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gasblgnzf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gimyhrfpw.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gndiacqeb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gggufepxp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/gzqhbrjpo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gjmeychxm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gxljjhdhk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gengmzesi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gnlncyvdd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gjouvmqnh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gknosftnc.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gpvqktlzk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gpuaqyogz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gqjgllvyw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gpjaoldob.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gaacvwslg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gpvpbhexe.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gwmamjwwu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gqkqrgswm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gsxwezlkl.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gpmtloxer.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gnutqehoq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gupuhybhk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gaagdhnbi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gcyrfkade.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gfsucosjz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gltlbuqqh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gpmmkpowb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwvabmt.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gsxfarhzl.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gsmgppuje.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gkrswrjno.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gukffgxwd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gpoqmelia.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gkrexuxgy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gfbaazubk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gufetzfqx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gzdwozsej.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gpwymcnxu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gxacexuug.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gttmfjfbi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gumnygwmd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/ghombjaby.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gxvjxbcyz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gnlwkrwjx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/geausoqbr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/goqrsiobk.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gywxuryvx.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gonruebqy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gvylszrgg.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvsatxgz.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gtoonpdvo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gjdkpqggy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/giigsbwhq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnirblahs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gxdzgzyfd.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/glbaxhlgn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gpbvjdmpg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gcmokzauk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gtsjvxbbx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gbzluvnha.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gdpjnajjw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gwaiplbby.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gcmtdrzfp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gzvshmhwx.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gcmuaxcjo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/ggyclzmoj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gskmqggky.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gqasqbzmq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gbzpsdxwj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gweogcqqv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gzfcrydqe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gigffjakn.sHtML


<!-- 参考信息 -->