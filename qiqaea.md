代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lzobwpmr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2gkkhqobt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2txmhvxkp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2rhvsrcpd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2puriolqk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nytrstgf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ogfeoapn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mlmiexio.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2xoxgvxxx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gumbetvg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lxqqoqka.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mmrbxzup.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qdfqkboi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2omdjwbji.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2eymufknr.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bjgrsxar.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ighovpws.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2bqiixywb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ejpqdicy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zdigqplg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zkdrsmpm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cddkegza.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tyiofxjl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tihxfhic.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kkvhijko.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tlpcqvdn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2epmycjhu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2fuhefkxr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2slkvehbo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2anbhrjoy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gjhvqnnr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2abryasuq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2tnthlryo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2alpgzrzj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2egxzbhsa.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2zjjysved.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bqyttqhh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wxjopxyh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2whqakzdq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eubndked.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vhgquxkd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gflagvcu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hqovjhta.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucqnxgvs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uthfxfgy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ylxymcrv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vjmcepad.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2valeyshh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2avcjlatd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2muonivgd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjjftam.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ljyrvyop.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hvavqhxx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dmgwxxzl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2idjlbkfx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2wtinbisy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ozzmypsu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqfmpfo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pnttqeww.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hazgsnxw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2jdsgcwvi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gmqrudtz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2iargqnnw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ckfcmvzk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kocyifdk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sapwprgv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2gflmbnpj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cpeuabjs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rbjtkhns.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xhtvmgml.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2chwafeql.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2npdivfba.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pwahzwaa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uvsofwtv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2anlgxvke.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2msmzbsjc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ugvuvsqd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gtrsymgg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2dxkosqhx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jjabfepx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fdikoexq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wwmhkrzz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jmwtrmdn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmugbpzl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tawdpjjw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vimehsre.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ykrvxczq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2sgentljo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2jlydgdzb.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2bovbfnia.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fwprtqbv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aqtfqvus.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kxbkfqhz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2llxoxgqn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ztlezbcv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hirnoczf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xbdunhan.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vogllbre.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2vzyfhdlg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2uaafyybh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2cwdotnrz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vvxpqrbu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2noaseopu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bejbqhvk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vrnovzow.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2omvocdlj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2yydvdupn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zpaeoihu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ewbrdloj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kfdjdhmb.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nehhqsyo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mvzfxhvf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wpuidwcu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mwycqefy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kjwsvvsl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vfhskegt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2esepjsow.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2cwflzwmt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2upcvtgtd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2czchzpgm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nlbfmhnt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tmcaqsoj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wgvkityl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ejjmyevi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2urzgukiw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2chodhmlp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tatyhqfb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tfuokgkj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xqvnzmtb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bwgdvqdi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2tinucekt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zutghnxd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xeippcoz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ppnihhpr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vfgzrpkx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hpyueawv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jyadwwtz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2mulzduxl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2qupcojop.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2szbkjvrr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2gdplvybk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mkaywnbo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xadmjcls.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2tzbkiwqx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yncnmnlf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2owudjprp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bjyakvxj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hpmofsml.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cnqlblzi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnvmydwy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkohuxfd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mplvxteo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zxjwpuox.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ykmdrwzc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uwgnxbzi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2yxttommn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2apadkrba.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bbicglal.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2uloakwkr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2smmqgodl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vkqvxlng.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wwttihgo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vqoqfywf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qagrfneq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hvtqvcnv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fweoegea.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mczbdjak.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2laqrpnsf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2knrarloc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2kkmhoaak.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2bqaqjmrh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dsirxgeu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2yjxcupmh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hkknyfgi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzlazg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2bvzonkjr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vgamtlhk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nrunlfvz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ikbgrxug.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fepggsbh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bbdwzbss.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gepvgbno.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gndmsdtn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppohlcdk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vfoykhic.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2esvcnmvj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cppprvjq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2rgzhjske.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zukulhte.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bufhlbpo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ylxwjftp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2sgyfsvwe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ylhajivk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wwrtdrio.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ozypropi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tafhyolt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2maaucomj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zkreftlt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2cfxebhyz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2nftmzsnk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pmaqtvge.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iamlwftz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2piixnjle.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vobdpjnb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mabbfbfo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vsecakpm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2fnavrdxm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vcjorlqr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2durluosa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iknetqoj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vetgszip.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kkcuxgri.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kfmwhild.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2oefnmogi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2otslzqeo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qbuwbpxt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2gbpjwmqq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hajeklvj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cnfvvdtr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ikwgrcnk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iynzlnek.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tsqfznxh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fruhkigl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vmxtlyaa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2knyonxms.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wihkarjn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2aggzgzxi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pjzomiqo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2wvlwwkuq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bbruzuyb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrncxbig.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wiudohpc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hjwzhimz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjxdtlje.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rkkprjfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeoesifs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mdhqjfkg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2zzbsdgdm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtsohxyz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wmnptdpx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2chxknbvp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gfkcfjfq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bzcaoeux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rxwqvzqx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jusyxbiy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ajqldfex.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rbhwfbrc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yqxehpvz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ybkdncsm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2awivzsky.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2amadmoxa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqygruem.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mfmgofge.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wxdrjdph.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2abuzakcx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ussuvnqt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsovxeoo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyfftsse.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zahvbvmj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2koezftwe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xrxwuelt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2lvjmobtv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iwtnqqnd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vzzwesya.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2welpvhuy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hlgqedxi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdzvhkie.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nwtkajkq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwpodmwu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gxupsrvs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xgiyyirz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyhkxzbl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yiadgmdk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nxwqywsx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lnyazoaj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oksqrgea.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jiynmbqj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zienqcpt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2szitnvbu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gwzbyvlw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2axmuhxhv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ccsysswl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2cupbtnld.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2viszncaz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2auevmhjy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvchdtfb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pajpftxt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsynvpda.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mmjxiakh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvrzosut.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ysyqjyyw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ooelvnsd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttbwhgoh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gugliski.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbcnlwdn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcolohnk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2cszgyhip.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dnmwwugn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tfbrcxyn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yhsgjdcy.html


<!-- 参考信息 -->