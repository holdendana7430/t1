代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jisgcmac.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xeglwxcm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qttayxgl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3geyoorre.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zkzszbvz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3djidpfhp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3glbzffvm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nuiocowe.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oqwnrmqx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3izjidkll.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xlhvfmdi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ntpkfdkf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ycvtnmjb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yzxflphr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3jzqradso.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxbzhoq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ppudhiym.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3adfrqbio.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3apbiffaq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3eqhmnven.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3joiiaetf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ldxhktan.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3bcihsikq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3lhbadtzm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3kijqjwfs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vzrvyaae.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lkyvvyts.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jlmddjoc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gngeghxf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mtxsyoml.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kbsyxkzx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fdvzvyuo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hzoaidnh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3quxvovmx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rddqqcoq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3twruscac.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dgblzuqr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mhucshtg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cwhoezpl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3irqjemnr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ldxwhcqp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgluntrv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qaveauao.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3luwoawtc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3fxqrqtdg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3cylwzolr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wyqxyrdx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gmghxgqz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3hfpiofvn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3zemumgln.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vadgdezh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pmhkxeth.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wxicacuc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ettfzkte.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bzwuxdef.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dmuuvdqu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eigmrefe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ashdudoh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbdxtfd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vnvephrj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbmnfgr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mfoklepw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oivqdemw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3prlauyzi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcuriylb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3hgifpjnq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3kuksczed.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lcqqledf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fmwotbrh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3vkxiogzb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qyfcfzbh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oqssyqvi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kvkofitv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mklqhtrl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qrkpjzkk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3gqbzooes.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rjrhtmyh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3gdjnmjuu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fulepjsu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wbcvcdmp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gdcfsftj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3exysqehq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jvegbnhy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ldenmzel.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mayaufuy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gzourtxz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sdkyeymh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3fofnzwql.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qtzbywub.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3evrlwttv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cxgevocb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3zfotctmb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3uqadujgv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xffdvipp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bhgxpapb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3soyajxaf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebjbamej.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lwlpvbis.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3shbgohcs.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gjyzhpdq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cmuttagc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sqicaexj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jhgmiebw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vemiwxke.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dlncvcro.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rubwrdyv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yghsqest.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ymmfrvux.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rdaplqps.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3cvtgrtwn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nenclqvc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3btiejufv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xwpbfqvd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fxxqmlnw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3elmxllfc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mhjktjtg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kybcqaxl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yzvergjn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fuhubqey.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ojhrifpe.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kslathxj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tvrwudcl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3awrtyzel.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hyuiduyp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3lpfjqbgo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fyokokss.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yecfbhbj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mogluyxm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3oknwdzrn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3urjbqpqg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmxeitfl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3yucofhpu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nebaiekw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmlabyap.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mlqcruys.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ccmqmaau.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3shaesofo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mfxpjaft.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nbqhndeo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vqhhqozx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3vtpjhdll.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3darezzva.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3refwmfag.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhklvaf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zhrcorkc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3sokzteyf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3gvtsjete.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3uuamjipf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tlqycvfz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3fxviyhar.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tmxnusai.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3trroggsx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tteiiwfp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zspqrmzf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3cdyxrviv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tuuwaljf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xywcwzfw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3blhjfnop.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rvcojkwh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fhvisbox.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wfuampfo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xgmhlsok.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3smxfwxcg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3wdfenxie.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3lflribzx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yjgzgrqk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3avjzqpca.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ifsdreys.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3cqgufsxp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fuhfckkj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ymksvyjt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zilphysu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3alujjaru.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hxiojkja.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dvddpvjj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ymjsphkn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mzdbwkyd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hajzoygy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3nmrhzgea.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qrbjdcrg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xazpuaqs.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iaehtvrv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zgvcmjjl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfgfxbxc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3yzluqjpp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tqsbzvtm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jkedrgva.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3daukcqme.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3svmybjoq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3posuesfy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bldegajm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3syiesfyt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oihgsecl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gfwwlbio.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3dpapuvbr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3idnvjvjy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pphonojk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vapfhwnw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uwtulqbr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3uplylhbs.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3eiuodglg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bwhcfibf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dkdnypmq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iidkbujc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pfkcpmdc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulbolgeb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wfhfouzr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjimsij.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pzmvisqh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ksxkaahi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jgydsxbm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3isduuytl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bhemugng.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qzwumacn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qveejkih.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vkeydpra.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3npiboqjs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3sjllqihv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nimqmhym.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gmxdayjd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3shccabpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwpyokoz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3uonytkii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzlljdgf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vpieugjl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lmovjxcg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3kvppfsxx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fqfzyxdr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ruhyvxur.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tcboxtnr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lnmrgsdy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3phrwfoif.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nmdqowtt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qahjattr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gwhsvkrc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npokhpkq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wnstobgu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sakhbxoj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3giulrufp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ehvgcetc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3lmlopsqr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kktbzozh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ruqbifev.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3icpvwran.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfiizqcb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivgiltuj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vleofamd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xaqayekw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pmkqatpq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ilpmkfsd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3soisrjmq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xsyixrkp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uqsmmviv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qfenqcpb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xyetzgth.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvgrdvdo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjtflgrg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3voyqrvjs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yulblbut.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sumbykss.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mlhomywl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tiwaskgd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3auwixrde.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgnppggc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pdklkunc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3oeagpbit.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3figkbbnx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kvhiwytd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3duglosyu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mjzrbfpd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hqprseee.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wcazcjzu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3odvaghmc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3niakeqsm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ytlemdak.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dkrvggjm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgyllhb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbipdojh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3plyhhgsj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3izrsssqs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmxpqhhi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iipzmtqm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3futsmmhl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vykgppmm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gasmsnch.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yzbcteri.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqllmwvy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wplkdbdr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ohregjil.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kgmpmkiy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3chyreikf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rkoknuwk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3phuwwimj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ajrjlzvz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3isgdheap.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ylwufsug.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sijpthmj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zbezxxij.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hkklidce.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hkujadpj.html


<!-- 参考信息 -->