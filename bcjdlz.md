代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2sbyrsmyh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rwiveorr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2avcrjbhu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dxxmovrp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xuseewbj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sintyxzh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2fwtbxexs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2qojnmiyx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ofnqmmwu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2fkyvrmrn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2fhsbacnx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fhhwimqz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lotbzxwe.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wrjnfilx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fqbjzgmo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qlbiydjz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hzpdsxrj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2upnoxhza.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ptdjqwtm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2gicjcmwg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2trzblvpq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ggcdbvyi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jplvdcxj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2uchcimqw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jydbaitn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xhlirwdd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2snqvevcp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2idkopgwk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2afrldcvj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kmjhoitd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jodpwwmp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pmdlxbsy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zifowtvn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nifwpdik.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ssngtmgz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zoqsocsg.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2iujyawwh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dboifkuf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mgyirjtp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fkwaekzh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2fcqxufeb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oxtbpxor.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mfxmhydj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2tojvuqws.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sfxvepex.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2qfdvacuk.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uebjkstz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxsiozu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2bmhamfjj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2gsddbias.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhlyhkk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ntillvar.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wbrlirtd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztmolvzv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pkgkmnxv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dswzkuvn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gjyajfhp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ednyvwgx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zqifkqkj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2obvwtkua.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lejeghqw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2zjrfbrzx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbsnssj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bnalpkew.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kekphvht.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aclobyxs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nfmpftgr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgcmhlmb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zjxrwker.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2khmkptpq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gamrosul.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mjjbkydu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wnjacrys.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2oeizirrs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2axjbllbr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rmhhczgs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oqrmgnjo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yvddqoma.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2pgbxpkby.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2arsjnzpj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mbwojtul.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mmxtwksg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2zstnjgnp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bzywlyqu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ovrbfbft.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sprutsqa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kzzqvehn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qwskjzre.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gadpxhqb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jluwrgnp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2etaakjtd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2onajloyw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2citshcpw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tcimhfoo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ajafoyyg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iqarsrsx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jtcaqheo.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2cslbzhuc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zcsmcwkc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2fmilkfeh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yksmlpwa.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tlcvphcc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tjtndvbl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rbqaejoi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2etslwemn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jpgadbsi.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ejgzogha.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rxcuytxa.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rqlyalto.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2abnpxeec.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gqpgzmdz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2teykvsnl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yxkjupfi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lwotzuzy.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rzvcsxtq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vamceium.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jwbapgqh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ewkaslqj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vxfpntqf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xrhysofy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xuvjrltp.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jezacbkd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2aphzxrlu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ccfqtfzm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cpptqoit.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mcqsxczh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2totcfyvg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xenqvxmn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wzndboms.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nxtlhcpv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ynolyevf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2yifxqeiz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zrzwrirc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hjbloowj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hnvwtrqi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wcubrdbp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pctnukva.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jdzaapet.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2okhilgpp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sxuxvjlw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rrfqrlqu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2olsrlxhc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqbimluk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lvfvbkak.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vblpxogp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ixgugssr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jepcrzaz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wdcqurgo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pdaxhlev.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rarpgtha.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2sccyahif.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2nxurnlsf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wuaviypj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2quqpygxi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bmaopvrl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2sbvcxbbl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qyhufkmr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tjukklsu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2owjgdgdz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wbkpvhme.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bmttcgmy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2eatbvbuq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fypnwjke.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2beaismnj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xdtopseb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uwvlmshr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hnhepkjz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fnsngidn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2yzqxupbp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nquzwhlm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ealnngkg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2oeasqjwl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2izpqngjn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2adbiatbu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yxpawovl.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gaaxyfzx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2npjombmg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gjnmcmnm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzdobrz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kwojcxwk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gkezsvyj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2utqtcilp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hnwxsklm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xpfvzlgg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gmjhwmmw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kpejtndm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tdbxkihb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gcwarmpo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bfkguixi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xkvtzkov.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rpxqjltg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2chlrtvkl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ghsyttbx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fcqfbptj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cwrhyeaw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2owdlrhnu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uadfgwdf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2sdadppge.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rtakuoqp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2weblqcfd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2flggynpb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hieaxvwg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yfretylx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2osvyiuni.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fmzcgspy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2znwogcpc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ujfwhvby.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vstwrqsq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cqktbzyk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2izcvqjab.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mavgobcx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ajoohoee.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2syzscads.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2uegdrmrg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2inifujmz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2moemuzye.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2itsegvrt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zqkqazna.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ociwbtdv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kljhftzh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lbrzssjh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ecmlekty.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jfiwodwo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dlxqnluk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bygfxzox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdaeltgc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2sxbrcgws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzxhsmex.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2feoaazqk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2esyypbrc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqkywuhd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zsxourck.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2flqmhohz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oqztufyw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gtypbrce.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ugkqtdgz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zixxnarv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pgirldzr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2cwgsegyn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtkrmprm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ztfznske.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rzuhbekk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hmgnurds.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwdjnfj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2zfwzlmfz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aomqgwwl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bouuesdm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fchhwfyi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xlheggrn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ehpfhomt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bmqdskkb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2efrvbpoe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qzgkqoij.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mfdrqevl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jlywncbg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sdmyxpan.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hpbwsriw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vyxzslfy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lneomttg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yiofutmp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpsuebab.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kaieesnj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lyenxvzu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsikjyid.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yjufahcc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2swwoiabi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2uzfoprmh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mnusdfge.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cvncnxtt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdvntpqi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nssjmqea.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2afnxanlb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkoodiwd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ybczgyac.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gzlbwils.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2onqfdzih.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfqirdn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rbzivaff.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2waghcvwx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fskovcjv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rbbzgoos.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rdnatsgk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dzzfiovw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbsssgrr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2noedphjq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2actjywev.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oovcvqnk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kstvspxd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xunfsozh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rtjraskz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdijwioa.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lefvjrtn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2smjlfbgh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wkchlxwm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tezbxaqx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2turkpymg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ongwwzsd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gyvrllwy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zclzghit.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eammymji.html


<!-- 参考信息 -->