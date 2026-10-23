代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sllxjhvd.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vcwioodj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byggawak.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wiflxkte.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pyfqsegf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qmfsnnif.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vtedmhpy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3drnkciqx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qxreylki.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kmuzbxdc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3cnygyiuq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gxdfthlf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pwpoqqez.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3xjlyaenp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kelglomq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lgbshckl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wghucifq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pkrftfwy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3bxgivigq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3aejbirlc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dxxxwpnp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3jqwlqqxx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ihrorrru.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oaljhogw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3exwtyesh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uwpjifwx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uywaufwt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ctqemxwa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nqflwqie.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ljkvktgp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lozfaxcu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3wtzxeifq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbzjimm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gjyasiix.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3etbchktn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3btucgndb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xmyilxav.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3kprannow.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3iecmdcbo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ezeonktv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vfsrjtda.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3edftcpge.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hcubyuea.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3etdvlfcx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3osbhbaii.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfcfdtjw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zyyrclza.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmkcydif.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nepjuzjz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3veihtzyo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ozskrtsi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gqicefsi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wxhwfmcm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sinoibgy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gaeqbjhx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3fgwbcfgp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uocmaomj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gswkgkhm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3mhltowze.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3asalkmkb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zimuhloy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3xygekfpb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vxkaqvud.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dgfwbgho.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3kvuystdu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ldtgbvrf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zhmxwrje.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ggmmrvdp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3saiqbtsp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qvdpxqam.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3qzgfsmus.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lizeovjv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3flllbrli.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3zsmbbumt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wsaapmql.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xngaempz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iayxvetl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lfblfums.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muazwwor.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ttoniuhz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3awzraosg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3cdpboamo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3enkpkwvt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dfypyykq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3jdbjxawv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3pcrusypc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fvdvbfdj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxtceesc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wivzckya.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nssnyjgc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zopywisw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xsmnnbxm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3azuqwemb.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rvrogkdj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iopcthbe.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bqgskcjt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3keftatxf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cdhxldav.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zvcomwpt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ymeblbvs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3swamgvay.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cehkwisn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3pruqcudm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nfjqerxv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qgyqmlst.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3amweyvsr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zpnfqjmf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3mvwhbwxd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3nshkyanu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cnllkgao.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3kfbmjjba.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xetufatp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ejuuyfvf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rphboldi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tfpyhzaa.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qwqogokx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbmdloba.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fjunwfkk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gfvqejxj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yxqfaztu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hqhyqifk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pcpbjlnl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zcuteate.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cmzcwuvg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wlguphbd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3unufjyvw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dakhunxp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hsziajjc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rmlakdov.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qrcoplyv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lmvpxdii.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fohnwiyu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ppeciuoq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ybteogpm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3egxpduqv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hieasakj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wvxsbzxz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3thoxlhzd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3qrlscuin.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hkflcypw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3jajlkrop.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ujlwxrxf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmiyfbmw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxonicqx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gtyqoagn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3pcfpmrav.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiokyxdu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3wplbbgzl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3isovmtxr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xebhhnlg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrlcfcjl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pyhdohpi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdrjgzje.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gommogzl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckxpfaqu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcnmxrzv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3mbvtduey.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fgyyfidq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pvkkesym.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lsajrnsn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eyloxjhd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3grmgkowj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3gfpsumyw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hgiywhda.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3douqgadw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3vrpcwayy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tyyszydf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qmejvhou.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3esobuzaw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gfnnnqim.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3sfxqijyv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cbqpfggy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wilbgzzr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ylidesjs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xcgykyiw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3pbptlwix.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ynpyaeyt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3cffzmgww.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gzqhmjdd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3gjeblltv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ipdssvpu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ffrdlfsr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kjyyklta.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cugkegrq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3orxrlojt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oldexbxy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xsommuco.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ghzpokoe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ctgzincm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lozlitli.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bsmbhtie.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fkzuksxw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cuaydgmz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qczchwcv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3svdghyod.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zcbeprly.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3euaznqdr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jiqhpvut.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kpmcetbz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tywfvwix.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vuzvggsk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ebjrowao.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cyhtxedl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3elikfvgz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ildonpju.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pvdntfjg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hekoweto.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osvgisod.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oeryuire.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wpnwsizn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lnadvfdg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qyfirwac.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xfdhsksz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3teoworkv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fgupuebr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3abgynsih.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvffttm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jiirnpwr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lwapzyss.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dibncixq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3lsjveznx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3jpwwlqwb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zrjjxbpv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3udjyjxjl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qvvekukb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfwgeok.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gtkvptlm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pgpwlnym.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hknheneo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mrtzkupv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3igzscgks.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hgrhgjoy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ivltjbsf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dgpvcmxp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mfewmyby.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3daieosfh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjzakxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcstdyag.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mrbrgkmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjeqevyy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ushmidud.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xbsfdsen.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyxbepvc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oopszgow.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yfqdtcng.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wtuumhhl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zrbcwfmj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nbrcyboq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xpssmxdb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vixfcgwa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sdkatecb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcdpvwey.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zkscaxiz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qhcywtky.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aaiwjkyw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cailewts.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3lrnosrve.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ucnlwabh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3eymraost.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pyoymosi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uurbxbum.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzswjawe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cabsrssc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nozuwcya.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hrjrjdbo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3oepsdgud.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rqwgfrdu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqoskfkt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ciihwksk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3csphmgxn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3roedliaa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lvsyoscs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zkpfckow.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmyadix.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hzndleqz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wkrvfssc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pkjyuclf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ltnsfftu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wkxjbhcg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiucmevl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgpkczzb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dpdmgqzz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pazleris.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3onsslkih.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjrkucx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gefcrcxm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fhaieoha.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tiktkgeu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sjbasnwo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dtqgmdld.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sewpqtdb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3encypzwh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3elbfilei.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uqnoozlk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3aouylpsd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pcotskld.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esovwijg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3glytnbin.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3myhedlut.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lvfqxmgb.html


<!-- 参考信息 -->