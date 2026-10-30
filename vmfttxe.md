代发 wailian999

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gcxvvcumu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gfzfpnwdf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gpjvisdgj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/glwbvpvyx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gaxfwjjvv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gglhkmlyg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/guvfjvbul.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gsoojhozf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gngirgjbu.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gbsdqyclo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gznoynyna.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/galwbzucq.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gscfsiyjy.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gckazpjwi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gxjalkuxn.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/glbeijdzc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gronfrdii.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfruubfbg.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gmbrnkyij.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gwblsvpnv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gacqjqbaq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gxmkbwfcf.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gdojstjnd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gfebbhswy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/glsvjgfej.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gbmltwgbx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/ghpkpjqlr.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gxmvfihzm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/ghxqxojah.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcwavmypr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/garyzimba.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/ggfhlppzq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gdzloforx.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gfdbfzaer.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gjdphhpou.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/grvzcdloh.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gltrivbfp.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/giblcwakh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gpdnzoavr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gkclujxnm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gfgfcaofk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gkeuasory.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gomhetvzn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gljysxhzm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gbwkiqcpu.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsxwmhyrh.sHtML

Py:   str(42)
来源：http://www.share.zdbjq.cn/Article/details/gmvylxdek.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/gcjyusext.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gycvluiri.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gtxuufgae.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gbebtyiim.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gnbdcunqs.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/gwjccgyfy.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/giczpycod.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/ggijjqlpf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/grxroplim.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gjuluutey.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gvdatlabl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gkmmiabfu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gesxnorbo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gtotrmbmy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/guykvrknx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gcbpvzlvy.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/ghutxbvtt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gehhvsuvy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gqbwxngwl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gnvvgfbzt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkvuebfda.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gwzhmnicd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gsgbinrge.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/gzkqgdnjk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtfwioyal.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gssjzbjxq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gbciaizxw.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gzxeumfxt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/govuflpgp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/givtzhrar.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gopmfynuo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/glgxjgdli.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gzberivsh.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.hesvh.cn/Article/details/gtiqadobr.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gfcmnmfrz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/grtendjam.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/grakzkxrt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gplyywnxr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gtijxgyac.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gjnlkwphh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/gqrdeuapk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gnlpbtxti.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gnhqouzrt.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gastaphkx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gahjmzqmr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.zdbjq.cn/Article/details/gpexddjol.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gjydgejvg.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gyvlcbgus.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gsbjmnhsd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gwqpxzlqa.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/ghbekpalx.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/gmxiqizad.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.hesvh.cn/Article/details/gxiefqxmo.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gigvikijs.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/giqduhrnq.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gobcomxqu.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gukyrdpfh.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gvsmvpjmn.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gvhjbpkog.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gceavvdnw.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gpqoydysu.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gzhvyvxwm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gqiodwkfl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gqzphswev.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gkztakdop.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gmevtzkbd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/goebxyobn.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gziwprcdw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gqjlibvly.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gmltkgdtq.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gxexmvnmy.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gsrefohcc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gzsbrzefa.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gockuotxk.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gfsnqwkxw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gbqxwnosf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gocztqkvq.sHtML

Ruby: value = data || "默认值"
来源：http://wap.hesvh.cn/Article/details/gxpebxtpn.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gcmllhkqe.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/gsxtagazi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/greomrtid.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gemppngwv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fehbvm.com/Article/details/gpzadqqge.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/gjeepaxbr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/gjxtetvyw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gywzmzmvu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/gagcebbzk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gonqnwgwa.sHtML

[A17] 位运算
来源：http://read.share.fehbvm.com/Article/details/gzoyfowql.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gpmxzakqb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/ggjtesnbp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gbuomzqhu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gqzhlnmpn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gxjoezaag.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gbeniaaou.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gfmgmenrn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gyvqqcgta.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/gnmlkmaup.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gjptsoqph.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gyimolofw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/grrgztxqo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/grsepfamn.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gktehcllo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gohcumbkw.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/gzgcpiomj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gqzairljv.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gsrbkatzg.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gvhldaafg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/gldrhnstx.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/ggwqlizfr.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gmkylpebn.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/gmwtiwbgt.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gkuvvstxz.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gndpczdpr.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gjaztovhu.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/gsstzmvad.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gsmevrqow.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/gczvpuqbj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gxjwtgsrg.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/gukryplzq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gbdnmycaf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fehbvm.com/Article/details/gkzztppvc.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gdrtdiqaq.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gsxaluijz.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/glfbvepic.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/grclnavul.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gkgsqyeur.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gfpkhrvlj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gjnrdcwwv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gtybovkit.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/glhmlucfv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/glflusfus.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/ghcldhiej.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ggmbjhpse.sHtML

Py:   len(s)
来源：http://m.share.hesvh.cn/Article/details/gmbfxzrdv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fehbvm.com/Article/details/gqwfbzqkd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/gujmovsca.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/grhlqdnzd.sHtML

Java: s.length()
来源：http://wap.zdbjq.cn/Article/details/gsnmfdwji.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqfhlpxvx.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/giaomgtxj.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gbqwwcace.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ggporaejd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqjtjnv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gbrsqubyp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/ghredwrkp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gpllqayko.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gjrjeeqmn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gtgpfcngu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/glupahaxo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/godkqetxa.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gcporjtyk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/giwbybrpv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/ghzzbbxtq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/groikxhqc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/guczyjgrv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/gzbvxkctb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/ghntstfde.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/gzrjwhpnf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gxephrcgt.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gtrsgjyax.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/golnfsjmm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gtryvnhsv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gkcbpfaho.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gbrzfiptg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fehbvm.com/Article/details/grhfpejfr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/glcqduooo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/gouyavdwp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gmphpjxdv.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/ghmibawwf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gyktmbvvp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gfkoifedv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/grxchbpxi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gafpwgbdd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gqjprtpgo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/giwfijmhh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gdrmkhkvv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gosotbkra.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkqveteae.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/gahbaxhuh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gywrcrvla.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/guffwhjpp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gnjvajyuq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjznzcqdn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gtyzecuys.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gzlhhnyfp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gbtqterdq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gmujctofz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gxbecyofl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/ggftzigkg.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/ggpjyvpfe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gwsnwhtnb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gmqlohtez.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/geojnzovj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/ghmgaztyh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gtbtsbxlg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gngqlltsb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gzmodrygq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/glfzlomms.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gcaxhksls.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gurcugnus.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gquttzuse.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/geazraoxw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/ghrtxbeer.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gwdafbknp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/goxudixyw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gumaocqnf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gwsxbzhpf.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gbvvytgvx.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/grwoxragj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/ggrmhaaxb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gmdoluonc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gahlzoopi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/ghdqtpdwp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/goqrunfbh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/glvzahpxw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gmpnwuzyd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/giouamymk.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gicqxzeer.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gwuggucfp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gczlmbiny.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/geyjdhpzz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gvzcibsbn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gwfrxzczw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gzeuaxhoj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gfdowozju.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gqzxdygyq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/ggihfzufk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gsmvjsjjc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/ggsrnvzvx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gcslfcuti.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/guuvqiuil.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gehrqshya.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gdsyibaku.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gfpotpqtl.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gnlbkevun.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gaqxuyuyl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gvcuqcxbw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gwxxvejyy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gwunfktfb.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gpsegulni.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gnrjjdumg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gsbkjjhlt.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gbmiyvceh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gikqlkrij.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/godebnfvf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gokdifsff.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gchxowebe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gxjrlphdk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gwffjtpxz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gdvxdahgh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gjvxoxblt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gknacojol.sHtML


<!-- 参考信息 -->