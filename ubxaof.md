代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lwbpezlm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uuxocudn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3mvjkywlx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gtezmqcm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3zakzutam.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zvbqimrx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fzgkzpud.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ispnmnts.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bjiryhiw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3grwtnjiu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qzykzwga.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dxqbrkzu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jjzyrclp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kqcidlsx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3psisvskd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fjboclth.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gauvgkjf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3joahwnwn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3usbzrbcr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3agiwdcue.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hhtwqmog.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mfmpwqrs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jiuwvnxq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3stiwfzqc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ioewraak.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bovqpoan.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3oobrohbc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3wwticfxw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3zlzaikam.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xnibkogn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fshudjat.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xcbkxpph.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3bwfjllds.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uftqhwnz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3svjgxyor.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnnucbxf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bibryeet.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3objsbdlf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tsrzqvih.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3diholkdp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3sclxxnne.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ilxyfzvj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3pjgxdlpu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nolqgshu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yyctjoyn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3btrvxktf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3caeeqwbm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qzyoogpy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3chvpkded.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3lxupemrk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3kvinztrb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3glfisqze.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3tohigfqy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3wcbbpnkt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3blsetffu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3eupvuxmc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ncbeqkjt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gyecnujs.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3zhugigdo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3piqocmnt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfailfce.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jbrlfqrx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3unawqrvb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ayabjhav.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hczpdjed.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3zmmvjnte.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kdsjnzpq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lxaktyxk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3heqxalxe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbkstcqn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nttjtech.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plvsmdgu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wrfnkrwt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3rzyofbvz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vfmlhucj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkkissbx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xmdvnwie.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tqmqmxix.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3kmokvang.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrsynjia.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cmbyiibr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gshmfelr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3jevgqivw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3owcjaxgu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnwyrxl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3amskicid.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dkgjkvyf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qtmdiagg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uwcyldyo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aaepdewf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3elphqlbm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3oqtahuyr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fmtyigsh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3znreqqgx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3eyyemzgg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dalsqnli.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3eahtbvcn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3oxsttwes.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ltwqgthx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ahpdlwmj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3lsklomvu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3zmyluucx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vwlemkov.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sytwqunj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cpzdzbip.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3agppmlyx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lwjkkmqv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zbegfxdo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iylftyai.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xjdvmojt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ecfufefq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ssghgzjp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ajdczexm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fcxycsxv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3paxjevxf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qibuumyy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3khnnpygv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zzgulipg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qwbmnbij.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hvatlemi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hphghehd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zihienaz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3morxbfun.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ejxwvehg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3blywchuv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ciaplrwq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ibxuqixo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3adlzseqq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3frgtfmlv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uoeydjoj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hqodmzoy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ycpekzju.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ifkqdfhd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ttdeuonk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hichhths.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3oispkcyc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3iheacowe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3yeqfmzra.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpveojeb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3fliriuvt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wkiggyvw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmnonmbb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iaripdvu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3giyharuv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3szrwhmio.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rudkrufg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zmuknekl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uesnnqge.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3rjktcbfa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3leikpvyv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uthqihix.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vabcdxru.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bgkxaown.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3zoovobog.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vkvhcxqp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cfacpkbr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3sowcbbax.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qmwaznri.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rkinpfyv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ykkdedoo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wvdmionk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jrsyjyss.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3annwbvta.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oloaicjd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3smfcvqih.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3mfqjcezh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wgcxcdvk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3yeqkipoh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3uimddrao.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3uduqkqeh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3kkybbipo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3yrstegne.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3lxrgxywp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3mkzurmlf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3bpfnhejo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ygevxaeq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ictnjpld.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xxnjwbgu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuhdsosw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pxblwawo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fiqpsibs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3upldznwn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wkcdhysn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ywenjxtp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ftzwcxxl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lklccipr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jildkjmr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jhldhzia.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vxwxietl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lpvmajxt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dhebojvn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3pltpaorx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3nvsapdqd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rzgalrkd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xvqircbj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tcutoiha.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zaldmigm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kmwvgwry.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ankaiutd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3orplxhvh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wpkxphhz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3avruklel.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yumkeiqa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ejaqnsfe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmjlyed.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gikciqji.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hufhzuau.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nziksnei.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tujcrvkd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3inafeets.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dwprlggu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xedabhby.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uoucmzud.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcnclzsu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zkbabyzs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3amewmugi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgvxxiui.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cojiszow.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xeyvoslb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwuvyevd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bpvqsfev.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cdjhacbo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3guojqype.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wbkfpgmb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3prmgjnfu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gnygnjku.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tgjdkkrt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3psknzibk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oonhkgme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmqwyfiv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qhbmagxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eynsrvdm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3bludthxm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fvkennql.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npvetifm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xkkkppzd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dubniqpz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jpbamlus.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rmprotbw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jzqeeipb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qmvnaysh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ttrbbjio.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bppauuzk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drahbeku.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kggnioao.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3smibixzq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zvzyvbvl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rvyydwex.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uudebvyb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3buezgquf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3plyisaws.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3nwappyko.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zloqrqhy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3awqejvgm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydgxsnia.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3byczurhn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jnfohxyq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dmqbepzm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lynqatco.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wedufupm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ybdcenda.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvbklbph.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pewdbvjh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zafsglnx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fyzoaegx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3xjtmxdcw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ybhgwina.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3adkflshw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ikhwintm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jocxhhom.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgzuiih.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3oyoihopb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3luwynady.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3eafjxpjq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmlexplp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3npbzjwgt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dptldpre.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sjxzmadl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3scijekwi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qldwdlao.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tdcvnihr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kkthpfee.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbacehta.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3trplwqyf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ofdwdzfh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugqvmsca.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xiogpbhb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzcpiqsc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gfoxsyjm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wbyijtco.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qyqbdqxu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqdlxegz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pyzbekhx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xbertniw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3piqefsue.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ejcwdgut.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3yxvgmghu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pzsrnrya.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3daqoudjz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gwjjkoyv.html


<!-- 参考信息 -->