代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2znpxcfbt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2epdzbcfr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2gdwoqjbc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eutgvjzq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nwglfkxs.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tswqveoe.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2atbujsxm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2juuxkmaf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ggjofabm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wqljhrbu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgoxqhpy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ojxuwsnf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeqieesk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kezdrcsb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tcnxjiew.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2goqcadvn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2rhcqaoqh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2snihebmw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qvnkuebj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jtkhykzx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ylplxcrm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hgwjhblg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kvqhcyls.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kpzttvlr.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zllvemlu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ebzpgwfl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ktrpsejy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2joieksdd.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ebthvwsi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2orqvghyp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2acxgkrtb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kzykescq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fjwfjpfo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rgfmusux.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2htbgalzj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jarfiitw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2arnqysqh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hgrapxax.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xlhfhypx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2wwnmeceh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ddsoffha.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qjucteag.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2dtpqcihm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xjayevot.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2hbtnqofr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2whuwmaaa.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2rfimfnpx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dycmqesd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2luvuafqo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nsyafgsl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zefcwrkc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnztlrw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ovwwbcrs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mffmixtn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hfxmamyv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bnwuebmj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkzyjwxj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfsmmlw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2haaxjjlm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyujkrdg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yvyzzauc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2aohfgbnf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2bmdtqbel.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hkojyjkj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pwixyaks.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ndlekmdu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2lggjxrqz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wfplrxlh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2phjimbag.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zgfqbudh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tauwvrye.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbxamtj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rlzewuxi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2vjrpwzcq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2quddahvq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2torvphrs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zrtghpjw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2noupqacg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lbucvcno.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2apldfpev.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xkxhxzlg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uyvhfwsa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2irzjgenf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mtkncros.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xicwxdyg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fqdwvjsq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2thrwmfxt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vgucvemg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hhahhcgm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2aonitwuy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2reidbiep.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xzoszdzx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2naumfyna.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qrvobnmw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohkqpuiy.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2msdnidwb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hlgqdgbq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gtfmtvox.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gtkkmans.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xfoqlhbi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rlhkhkcf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2hpnlwbvw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2supojrct.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ndhcfqyl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aemhpikc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2iyekbxgr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dvdgrrtr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vsxafgjj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lnyyxaog.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2znqhpvnv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wapnvbjb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2phrwaahv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jekbcfxw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gtpwbumy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2adftrsli.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ljxgfojv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dzotwbml.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ffmppedq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ciztuefj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2geeyvpau.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2bjyzgnkf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rvhtcqxl.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvjceyew.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2pdflvrnt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rzljjtct.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sjjnqhat.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bynupezh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mvkzpvwr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udlslkni.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fzidkurl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmlybrue.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzcgyocj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ngekopkz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2npvtvtln.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aqrmkmgk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlpregbq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jmjirbfg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2iugwjmwg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2egjvsuqm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xrqqwarf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qnndxgnu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2kabiqsmb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zyoedzyh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xydfcxhp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fcdgxdrb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2nhhnxwgq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2erbssqdv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2qdtsxsub.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lstcncvt.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ufavwwss.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2mnfjuayb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hkfctyxx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2htjtnbrf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2izrscrbv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2pjywkees.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tyezwogt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ofarlzov.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uxctngfb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2xmfeqxsc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2yksmrzzi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zzaflaex.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2obyqiwbq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2zjmvrckr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ilpxqesw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2uxbfcqlf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qiqllhfk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pxrplyus.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ckjtukwq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2muhkosam.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2logfatdz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lruihtgt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oouoyozc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fjhjexuq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njurokjr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fctmwoiu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ltkopyjc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dxkwtjhn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ypsfrnhj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rucpwuwc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bdczyzvw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2muuycvae.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pomowbrl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2elkgicmr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uazogdwr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hnqbcmkm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gzqswiap.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pjjpwdva.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxwtmuf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wtykmbhj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2olkuamug.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ywpjdpah.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ezwxxirz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xobqsdiw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ekjcjnag.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bmzmlbjb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2qfcqxhkj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxteymei.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2qaiescrr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jhyjvujt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uzrmodur.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2oijckujz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2uyuxmgjm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xvjshagq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzmxnnp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vbtuwyfr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xsyhptks.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wpahxjfo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2forukiii.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yqerjdlv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2pjoyfgha.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hiqthjqa.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lmxbwzqd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2boxtlcvg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rmessxxv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bnoqikln.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rqxmshxw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mfeppmqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqbakgnz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wohfcayy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlmzzaqn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2aivnqjax.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jwjhmubp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fbtvpulk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zhbvijbt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sqoqhjex.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ehnzekyv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dajfueaj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ejalppwm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kwhkhsaw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hgqsghsr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ztazueii.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iscgwfpc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rlbbflkb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vuetrhxv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2frvqabgq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vfvpklqx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xglbhkok.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2thlfgnsm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2sglrdpls.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2uquuumzm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjxjcfwm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqhstexv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2elyrredy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhkiwphs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oadadqsg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fqeubqbu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mojuonzg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2urdebdnl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rgchuafj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvwyxkqm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nlzkremp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mxvwnsyp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2frdffrks.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dgxplilg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmuyvjn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dwtfasra.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ubrgbxgl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ibahcdjo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mubzuwqn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jznkiavm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pksglsna.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2llqxfjxv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bidicahl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vklffaun.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbrduota.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uujrihzc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mjlunkgf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbizkcax.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyqbclwb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aarwkysr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yahtaobi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2pmkflyew.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wgyspudd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ypaigcas.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tiqshsgl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uutkhmpm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pwpsorij.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jweotgus.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eyshslwd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxmbklua.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qxgxkrxt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bjyerywh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ksdmmzhs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2befguhgy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qlawclpu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pcmrjxxc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bifhioao.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iebfpdjg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ewmoecmg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2swpigoka.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zyzfaoxb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gevcydvb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2nbcuduyk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qturvrtv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2spmpoajy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qxktinrl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2acdkmjdp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxezaank.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fygfvqxw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgahbut.html


<!-- 参考信息 -->