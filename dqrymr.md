代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ptoaolqs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vtoirvpc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2rkkakovq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dbjrffek.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bfwnskqq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2tacwbwno.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2bzledtyd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hgaacvkc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vwcvqddd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2owzprazs.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hedseoxz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xpagayzs.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fjmmsorj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kdjkvcda.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lihsfqnp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2gopxezyj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oatoppwj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rhmrdhhy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bjijypqv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kedthida.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2gcgshujk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ifxnasxq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2omdgxvgp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2iqijmrpd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2dmtpfewe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mlfzurnx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wxhplcow.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xfvnpzuz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yzrqeywy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gfsbqkcd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mwojxwhs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lstgqepm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vuyerkot.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xiyvmeef.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fpmqobvk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pasexbmc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2shlekucq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yqwghfqx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dysxsmzs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jocxobgy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jwigkvmz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2bhjvvapi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qlezigkn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ehvamyfu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2diqvbigt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2robexmqn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2lcbtswxo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nknjvkjv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2odtfkonl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cjcnykds.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zqqnvdyk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2krtuyqzh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2xwyzjunl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2olfbviur.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xfadbqxw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2msjzstkz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hamwiexv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ckrgjwho.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dpnxqoil.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wmbtjdzm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fxujmgfc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cdrqzlbh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2svlbuxyt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sddantay.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2njiudchv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ramzrmah.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2nhkjksif.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2grwqyvab.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2pzkvnncg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hgqraftm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2spzzfalx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ngqhjcbf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2govgyfvc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fkrcfycx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2zyilwivc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2rnsullqk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2cttjlosw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zsfxrtai.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kjfuzajm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kqyifyih.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oebrsnpm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2njtrxftx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bmhycgue.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2uhyvcopw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kktdrdhf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bkjqggvq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2roksjrhq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2whteqhlo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kvxipilc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fjlbwnfs.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vnloqgkt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2luiwiugu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tyvhhqia.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vekfbnrj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2tvasvhob.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zcjtmjan.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tscrqzff.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ogoipett.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ijzcxrxw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fsoocwaz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dfuoemco.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tzxkumri.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gqehzpkv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mplsveoy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2wwswvgzc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qgandfju.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nuodwnkx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nnhoirul.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gkxgrvjv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2akggsmco.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mcopwygk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2quyktqdn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kulvmuzg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pbpuszhm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mbgyvuvj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2haydneus.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2iaeobpnj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ouovrzex.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2hpnyliji.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2quuviwzm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wwaelvzz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sxhsvtsf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2yelvqfat.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zurvcqgw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kefwbsii.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dshkhwwe.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2zoemznkg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dpinubro.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nbazxost.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2moodzbbl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubfdqvtl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2tcsjmjkc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lxakueby.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sxhjncdy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hewmjxnb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2doqoefzr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yedrikht.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ealscgyv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tqlpvefa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fbbamxbk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2eviphjxi.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uwvndwnp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wjeiljwx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rmurfqmp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fjntloft.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hvdklnxb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2bncdkzgr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2rnjemeoq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2jymdgvrm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bxvvtpza.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2enctkxiq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2seratffc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dlplplvx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yqmmpmrk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2mycgrquo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hrnlkllm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vqhmgkvg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2cdratest.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vudmyimr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ooeniglw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kzkuxcwn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ukhmqcvl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hvovgqlr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2uuibdpar.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2gupruoqx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bwqsvucj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2aspcbcet.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2bbmydwmv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxchyeee.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cavfrdqx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zywsckxm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hxsvjceu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjwlcaf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qidhothw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cyahoqmv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2imcowxen.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2frkddivb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzolzeuv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2znrpaqbd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2canvupwl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zasavpff.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cjlkzqrc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnggnybp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zsvybjhl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rqhfdymf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fzhrwsej.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dqymfhuu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ckuoedxp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zwivnqfh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aayywwel.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2djqzxlgx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xylwaztz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jwhvchsj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fqecvahs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nziebtqo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fppqdkvb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wogpsnvf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2daawuiaf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cmxbtrga.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2yofhpxon.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2usuhgbks.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2qdajduod.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2txldvthl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hdrthoyg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ciyufhhr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2wfojnthc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qniylnbk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ozftexyj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vpbebmkd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ohunxzio.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pqmsmdvx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ufiqpuud.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2rwsbzvmu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mgizsmov.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rolootqe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2zuezohti.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ykaiccmc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hmmbbrhj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2whezdhlu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dlugrein.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2diahfoaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eovhnyor.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lygqaokw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqltzsyl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bqdgwysw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mjphwnal.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yncgirga.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2egadhnmy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jpuohbri.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dehdgqfr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2irgjaxtq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qibtyehs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lfljwtpb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2giapnten.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2juvtuhve.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zktgahwj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hknocfsr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ihcsojno.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pnybttro.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2tuotvdpe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bltxrjii.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wwbifpcm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jpoltjch.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bauxewme.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hqgvgxic.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hripabrd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zckdsguu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bcchrixd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2linhpsta.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yemhsdzw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kouyjcah.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2whcbbvnn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmtsrdj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyyuxfst.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sdedtqtt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozfenxss.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyyxqafm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xbttrdeq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2iivncsdc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfllkkjk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lzbnleii.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2czhnpwdf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nemtzhjr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjoetojo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fenqtssn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cswpbxau.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2svrcihle.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jxlnndza.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jhzcapjm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2arqwlmes.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ybjihcti.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvjlbwwm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vnatvwgw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xchyyulr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uvsleflx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ytajpjnq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2frmuhjux.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfkwhrq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2kumppzzc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jznajwrw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lfsflxdk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uokzwzre.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vtorepsh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2myuzniqd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2nyjqyocu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bmttmold.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lexduhyh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wltaouvl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lqyffwki.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zfhwozcz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rxyfzbqa.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sesypaap.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xpyccnkx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gixhoays.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fxhagemq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dkqowfso.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ynpcgmcj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pfhbamxp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mpboczxg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xcyzrssc.html


<!-- 参考信息 -->