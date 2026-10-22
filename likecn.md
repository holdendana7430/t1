代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lcximfqa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2olhfktft.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2lzngrkcd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2iovhymhe.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vnxlpsjz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ebulxuai.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2plhzzlxc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wwbhzhqd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cegwvlsa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cnlbprne.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2btadqzhq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2pxvrldnj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2apjgfine.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pmleiaec.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xbewedju.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2icwgvahp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kvburjqk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vsghuxpk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mixfmxpn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qkzoccho.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qnigbgbs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mrichjov.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wfukbqpw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2tyfzvwzm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kxoiyout.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2cygneeiy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wbgsgsjh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2cqsujtvo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2uvqbjwln.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gpctidau.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ygfdjake.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ngzdaipj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2igufcosw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zmsznjpr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fnfqfgcb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ttjkrisz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ymmymute.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hgsiroih.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gpmvwowb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xkyyyqti.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2exthyfus.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2italvgeo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2goojygzw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bmgioszz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mgixszcf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rxgzdtap.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jcgiycfj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2eztjtbst.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pxmwrwgp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2uzrdotuu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jevqqkvb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nvzkqgty.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hywazlvv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2kjekyalj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jkjkxkun.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cgvdwnfl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wqldvoqa.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2cewbjzjb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ormwsaro.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vacebexo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ubdtwyas.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2buldkcqz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2mwwqvybc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ydbbtlnm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2muagbdnl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ygwenqcm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fpnwltvx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mmtipiwj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbuboktt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fhqqvedu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mgnaoyzz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aovkjuxu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vaeqhidf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2stltjnee.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2erdchuyw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itxsvmhs.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2bqmocxbu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vgbvjzan.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2itbzmmbo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ynvzyaiu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpefpjhp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgmdxbdu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2akavbxit.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2nbmrrprt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mdosnwdt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dmddaife.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2watssuer.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wayjbzrd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2diithwfz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kgnyxsjz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rohravkv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2oxwbmsea.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nxcpcsqj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aqlgelem.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yfmaeeoq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2dbyckcjg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mvbscklh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2epieivgr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ojxoqzcq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbfjrtx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2khilkilh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nxxdstnu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dyodexwp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2gdijxlta.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2inulpvjk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2reeqbizj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vbzewaub.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uhwpynzf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pdmqodur.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pjdtdlpo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ppyzqtjj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aubdrefz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2fuenhqbt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jwoianwd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ccbqtahm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2josxlvak.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yhxwwkca.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2urnbxalo.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ycvrxjzq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wxgyrwtp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vohqwzyz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2kpywnqie.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bsdyzdtr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yinpuccq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vkcenybz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gkeudfuv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gvqkfbno.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ciucwnzx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ipjsjxpd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2easukdys.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2tkehvslz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2qjilbqro.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2aniosuwf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2lxzmjhju.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqmyvpvl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2arursqos.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zgenurpn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xaieewzi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dnujclav.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2pewfhrwo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rimwxjio.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eddomzzl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2byrgwlwi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iwgzifap.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vkbeziqh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lbaylglr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwalxgtb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yzyhimrc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hgjbqpfq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2waovuofx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2meyqrcyc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wxrvpdjz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmtzplz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dstexpwr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gwocnfqo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2whpgznzh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2osgyzkex.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2yposmejb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lrimuadd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2oizhsjqx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wnmnslyi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2feivjyvb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2gxqavgzo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qvlebdpm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xhabollm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2wghpyrtd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2wprbzbyn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2djffjilv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2fdmxadqh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rxahzxza.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2wmuomggd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2epwsoghn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ygneirgy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mjyqmzdt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gwbvnuaa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2giiatxtl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbwnwvew.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2apqsmpqp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfagptay.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pwgweyvd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2estnjede.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2saubgxqa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yddiiqfa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ovwgesgo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmyolgdb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2aumvkjcf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2kjmwzgxe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2tsyvlfst.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2txyhbbul.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ocmpnnxe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxnzptfz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ophqwpwu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fxmyypnt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fyzirpof.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2byhbuqrv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2whorymjm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tcrocfsy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gczahnep.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zmojkyyw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2bgioooco.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fpjxvwwh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mlxfsqls.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nkguomvf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2azluxfgc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2oiwskojq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2crdkdqsr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qtgrxqox.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2czdkxfwv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ualwxjbl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rvnzgcht.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ehnqitlk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uffohmhs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zclhrixt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfrsbygj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppvmgvce.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbvaapkt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzmorpjk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcohhesf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vguzqqdb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gojybouc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wgrfbsle.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qghmlzjb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ujiryfmh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cvxapghd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2svhmukqe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zjxydeay.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qkcoizez.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rewmrwsh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2alvhcmja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efidgpjs.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ltecdqzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dteuosvk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2puhzgwuh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lbnuvkqb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2nbqyggzl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2stcqshpq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fhahmzqb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jknpzgpg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rljznqqy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2apganbty.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vfumxato.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ltzfvzla.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ntjcjmzb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uqjofzuh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gsmjobva.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vbyxifnx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2doxinjuh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xbjhjxqd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fgequzfx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jpjhsbsz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gydlxndv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jgzjtvgx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mshpmpif.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2afbimkvm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qbzzxvhc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bklsonka.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wtiehmkg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ssixfknx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pngspmaz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ixpvncsp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2limgbxha.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hyrnotxy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jingmmlv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwerbgf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nothsshr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2idvxjsjp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2blxhlqnh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2atqoqqok.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ggmawthd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2irulkhkv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qawqwspd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dobbrtyp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hnkqtmta.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2slehzcdx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdzubfg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2agngzzzy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsbrevlj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wozlwomx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qizqmyhj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lcxgunjz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdseaitd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wcqrrsmv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgfeqkme.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ixjewgcf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fbbfdcdk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2irbvbnvk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cyrrvrhe.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmdevshk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hlgmqxss.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2olkntxwt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hpumlwme.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2raqnluxk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2okvhilxt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2aghotems.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnnvvgwp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xdkejatu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tylphwon.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aunyvarl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wgoueplf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gwrgazwv.html


<!-- 参考信息 -->