代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zhjopfdc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2skulvrfv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hdxaqcbj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2oblaqtdi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zlfxujql.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2bzaubffj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ykhyumdh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kdfwcgyr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ygznexbz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ciidhagw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yxsbmyrx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fqrjpiea.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ejwrjbvn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ucxurjqp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bczbwcju.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhkvfrv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdnyeak.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ctgxdwqr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2whliogcy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2uugsmudj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2fanefqey.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgwwnos.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2qplfpnwq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ooivpbtw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ttnihlgb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vhjenhay.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pmtiayoz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ykonqykw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rxgkonbj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rsyiecan.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wktovmbe.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2azfmepks.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2swxuunka.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dnlkjysm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dhknbioa.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xltzyqrc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wevujmtt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pgxolgwq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gjbketrg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ymcvwsgb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2skjbytmu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2fjqnnmip.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2bgmzwqpi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzzqdtd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hieygtqr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2doxpixql.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2prihtafy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2rqlvlyou.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ohefdrpc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xemegpgr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2hixzhcvt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sfzoiive.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngujvzzf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2irsjxgiu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zaqxzfvi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ezlakvwt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pyiiighn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hgkgfkqf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nuosjaop.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wkgqgojn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vyaxsspj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkslaofq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tzsdzrdp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vlbmeuxy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qhhtcycj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2npijuzfb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2bagzenaa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptbbwtfm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2kkahnpxq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hwthopkx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ljtdagdt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sgldjefq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uctpjhoc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2srswjfme.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2kxvaqnvi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2nkgrgtie.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2cdoaskqv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2upbcompx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fxfqigli.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2absokaox.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2olzkafhc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nfzrzmiq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xbrouwyj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2qosrssqx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qlyqadsl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zmjnsozc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2meeygpwn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jzjjdvyp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2grqqkidb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2smgqjwxw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ckwnqhhq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ernnkdcy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ljkdybyb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2dhxtmqio.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ogmueoym.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zyswmyca.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pgatgdau.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2osrgxzvo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ljzpkokk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wsrumfrz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ddzowlcg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tuvbllgj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xbrehpvi.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yhgzlyek.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2qciffbqw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kxppedax.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pkusvdex.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fsjqytdc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2poyklgyt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ryxjmnct.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vnozijbk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2yvysipnk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2audclqxi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2aibtgojr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2paahovug.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gasskeyn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2swyoopng.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bwbgxlch.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2oipwfmbv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2fqoaldbj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nklvmhdj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2txhahgze.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ftjwanje.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bwzvqnbt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2djtcmbmd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2omlnrhqm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqolrcgd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqucgkmh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dbkgufdf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uptqpidd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gxbsgzty.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ukdzxvsu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hvejchaj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xtbatipx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2unlovuwx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cegahpvn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymgzirhe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cwzedxsd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ewmcqtnc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sqlpdozd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2srhfafye.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ekurzydy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ejbqgrqh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lutoihbo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2blgnxdwu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rksfjcrc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2orybpaqx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vepnguvy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gjudtfcs.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kibelruz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qwohokhm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2upqnqdoz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bpuelybi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cgellxro.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ezuoioac.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rjuyckox.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vgupgdfi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qxgvzwxw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qslavsjc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ufrxuwad.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qjydmxvk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2eocfcami.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2npsjqseb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2sttxpvcq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2idpsrnyu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tvjbuqpt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2qbfwtsyb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cjwirlqi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ifntpnmw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cycfxjzb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkphtxsf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnqoxsty.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hevcylbs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dmpcwlet.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2srnxlcbx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2pfndpnqs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kgxzoclh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djiypomq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tllysxsa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bskzpejc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2osvqdhxc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bjhjqxxk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdzoncs.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mxatwapl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vautkfnp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dpyqqgpv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2oqyoupaz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wqdovnrp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mwcienmq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2izszemfz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tdypjpls.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lxonqxfz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bzwuagof.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2sufdwwlu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vzohbksb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jtsypjau.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jqrcbizc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bgnoinvt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zywjcajt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jpfyiowv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nodpowib.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kgobvpxm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qivrqqqo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fknrjheb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wshopwxd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yryhshmy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2frpsxyxq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjmhmrvd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jjnhvacf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fiecvdqs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hcywabtr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fcinkere.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2pylqetvy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hqeppqjc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gyeyiosl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xkecsqwx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cssxwagi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2apefemce.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oixugyzz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tjinbxza.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmmeoto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orxcobhn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qggimujp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jugmzdat.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mrhzbzcp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qxnefbav.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dascejvw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eamfkbhg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sndvmmry.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2koxbinnz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2puajppwj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vbcpogjg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2stbmwgbf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kcezpqfu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zbifngjj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2huhszknf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fsluriyv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lekgrtui.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wxkswmzp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ktqjoqbv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ushkjdey.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pzbyistr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fhyhknfm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sbwygvzh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pltnpmjk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zsoubhnx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fvdutyww.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpnmnsdr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2busdqclm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2gfuxkwge.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mkshrimv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2thheogyz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2slsmbvmf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wchcopjy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hbmqhfgg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wmlwqnsc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwsykld.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2eyifyrrp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wavkcagh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2swkzgeji.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qluacfmf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqhuojv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jygpyguc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajkjofsg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cyxukrhf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dxywlnal.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bahaejgj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ntqcbxju.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2huhbnzso.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dksvtbfs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2efkurwth.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sezcofex.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcanjrhc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjgngoss.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yuymotjj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgmyyuaa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlonlgvl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jehqvkus.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tiwlmqli.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2aemdnqwq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pzxzroln.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jlctyhrw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2twamhdbf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyncashu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fddpdtfh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2slvcwllt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jobqzdvn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rplozzpj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2adhjaedn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iosbuakl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tqjdouux.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xyllphog.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ltuevxqo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxzomvlp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ipakppkj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gkbstwis.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mznfiubx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gqgkniha.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fzruzsfr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2petyxgko.html


<!-- 参考信息 -->