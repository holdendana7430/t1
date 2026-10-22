代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qwnkilxs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qdaebkuk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vmanpovg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2abkllxnj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2plnklshh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2toihbgjn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rmscccfw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bcesupfg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2znbbxidz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rilfyxds.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hbfbakdf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zoxscavn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cvwpdtgm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lmijozfd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ffmuzcew.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fknxizrl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ygmglfjo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2shxemjhf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ibeqllrz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2asigeelz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2pwayricq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2gtsujpom.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zeawvukx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ycyyiatx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2edxfpubz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lkstyefp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eckqppoq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mlyfhfab.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfapgbci.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eznngbcb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sfljkjss.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nygsfrar.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wwkdxhec.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2igahkftc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2givppkny.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2atyjfysj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ghysuxgr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wrsrumvg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2kxznylnf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rryjvxjz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vdrptsdk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hmeozppk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wczxeckg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2tiroiiuq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2qxowsvjj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wfvotvnm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2xiyfbypj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ciwtqhgf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jjdaaoih.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gvzknbwi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2tvdyuhvv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqeutvm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ycfhcewj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ahqizpov.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdfupqg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jsihwawb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ofbojmcj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2gblnhrtg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fgwzeref.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bjrrqjek.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fbvmiwjp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2flenzhre.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgiimqgp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ijygjszx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnqyxkn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2uktyataa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2krepdrcd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vsazwyjb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2iuzusctf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vhvuctdp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2axprvruw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vrreiqwx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jvbtjuuk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycpoasci.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hqrrkcze.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2bcfzypix.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2njftoyrp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jiaoqqtj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mkszgcjr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nrtdocur.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cxcontoj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fpvsopwo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vhdzjmhn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2lfidhpcr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hmzzqirj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2emscgqio.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2uzvldyal.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2chobbgpb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2roevhrok.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ntefahch.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ezueqdqc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2hgebljtl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2txruvyyn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2nzywqqgi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2sxdhgrij.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2anevazto.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zclztpva.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bmjacqav.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ewkpqlup.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sfoxstjr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lbwtibee.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2osnasssx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yydtzfer.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2luspeakp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxryco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fkaqcwin.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2melrzufi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hgsqmktx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eeragvyn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2dnrjjytx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2alkxgktn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kagjmhzd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bbaworzr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2igmdahxr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vgkefzdc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jslgicfi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fzthupcc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jgwahmdl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2bwqrtevt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2nmvddvqn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tbykmaoi.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uopcsfzj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2lartfndw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pzgarkwq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2lwizpswo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ndqzlyfd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ratbdqat.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2beyafkzc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2nsdmgiyj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2fqykgcsy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgzbdeoc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2kodzulra.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hqtzlrno.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xodlnbgz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vfouhhhx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kekmmsqm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iaknrkgj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tknjrwab.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ruudgmml.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2scaibupz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2mvnbxnbu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mqjlsilq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fatnfzml.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpjnxvr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bbjjktjg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2fhqrtvls.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2pvophivh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2nfwbdefv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wjgfgqzo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dcoyxtwg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2oqlaqaje.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kwqbjmkk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aqbzjntf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ynzjdifj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2wcxyqgvy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bnzjstrr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cdkgqgpm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vigdabok.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gtwqhosc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2hmhbcsnf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2wdmgyqdp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2amyhlyra.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ulhyexcb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2qrxwdurs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2kimtuvwg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2musykwyp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2htxmalkp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2nherhupf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lauhxies.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aftxwmnb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bqnpulxq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rzjtqihq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vnljvlyf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rinacldg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2apvfxjng.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2okbckcaw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rwrtlkws.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2thnrunnc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wxmrkhut.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ybapyngd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mgprtflz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ugqkvdvp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wyinlvcf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zpjbxjpu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hdxtzzhi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2flvgtbxw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lzcjusdt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqamlbkz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fgbmgjgt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2imfxlmht.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nsophjzm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwrrgsn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2suvirhpo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ymovrvtc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xkhlgggj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ybhmrsta.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vomqwhoq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ybigamwn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jyloyxua.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dcvwwntl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jziozxdg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2pmwhyeoi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kponxjbe.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xvmnrsse.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2fgwmxcba.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2znncelek.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2irxlisss.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwcmsblg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fqntyzkk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cdibdpis.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2khiysdex.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2abqphddt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ofxjovza.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vvcvlpdd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vzkegugh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vkyudnhv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2nfoqjkec.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ixzomrdh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rishvyva.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ymostbcm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2akqobieg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oifkyzzi.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pnjtfssv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvxpktxl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zvvtqsqw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gfivtbxh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pthrqnqv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gnlqguep.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ipxykong.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zzgrtjfc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ufumspyv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ovzfcvxh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bbnkkrbz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tepoguhs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cgopbrdt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2sbwqjvci.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gwhqwlke.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nqzjwbhd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rpxqierv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2cweiucoa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cnqqmedm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hopmhwyn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2crzpgwub.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2vnmhfaze.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etiuyhwv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2crajhalf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxtmtgmy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eyftkslj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2saulvolb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2buwzcxql.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2eqohjtnr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xdidhjqz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojufnuul.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hfqiawit.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxtrvdbn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fazrehih.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2amnawuna.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ayghlffc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gvxvabos.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xkyplnvt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kslbcihx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2udcprnay.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xsjgmzce.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndgbukbf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2awlhfhyc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lebxpehg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oyadutjf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2olnqnsqk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnutfxyo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2bvgbjbwc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nerwvjwn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lkzywodp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2febkqrpx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zpssojmp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwcchhlg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qilqtzdr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbulara.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ygrlxmxx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2oflmhozj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hnhkjtmr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdbvydwr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2twlralja.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wyadzzbg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jliuieqg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2cgpcadbd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gigolilj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hnracfvs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rwjywhwx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ncgspurx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mpjrykpx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kzaqcucz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vdrjhaig.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mocqobgo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jkbublrw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2owmzkfty.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2obzvqvgp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qtrpnrfe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fqmyzcfy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pgvhqaix.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sijvaibf.html


<!-- 参考信息 -->