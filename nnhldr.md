代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fibbleay.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zsundblf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3blefyldg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tqgbkvkv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vlbcdxvw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3daisrtou.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ulydhnso.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ydfxlnid.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3axlittyq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eeohrzrz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3sjjgbwjj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hjwfgvfj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aeoheomu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3unckdwgv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3gfwmptiq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jjopsscb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sosfisak.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imdrqfwv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vysmdpif.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3utmjvvje.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3yxubrjst.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tzmryovr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fuvbamid.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3sbzgjxiv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3acpkgwbh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qilojoxt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nqtwvbax.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3picssxrr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fdrztzzq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3peltbmwf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3gwuazuef.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3dmjtmkyr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3pwxvibfi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tsjmdtjv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwfttdnl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gjqleuxs.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gqjpzrjq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mdvzhygj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tzauopqw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bkugktqr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zmtowbfz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rvdsmbfc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3aauirdfr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uwwodlcp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jbzhlgkn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hbmsxqro.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3vfzgvimm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3tvmjjqvs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gcyrynwi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dkkftnrm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3uzagkpwe.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3yjinlded.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sxmclwwu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3wpuqwcqa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3afqxwuus.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hklfqztm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dvdqrnop.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3lfghdvto.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wdsfmxpp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vgcczlqu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3emhrwrjx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ykftbfzm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3waeyjcrf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3blabinld.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vhkzvwgu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jtpmedjo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3guyphart.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hmdlbyli.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3obmzxlgd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3onhmixpr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hdvrywup.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcskktj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mxmzxfve.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3vafbipfw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mgnhsykt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uktdpaut.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uyjmovjn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrqdnkm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3aamcelwo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pidpfblf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dmrzrvkp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mowfwnqz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3eadoympa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3roypdaqc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqowalo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tigbvuyk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3izbmpieo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3drrdbypf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3parajamh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ytozgbic.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rmvmohyt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dflgdymu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dsshgqhp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3beyegxpb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rfkxwcgr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3pbrlmbin.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3krrbobfb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kfibkcms.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lbsaypya.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3hzdtinnl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lshhorhk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jgqlqcdd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hudcfjvg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bovjbskz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kksdjbbz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zhxkgqlm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ukhcpkwj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gjscayxx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uqvmbpyh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hfmonbwq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3etwjxgpn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kkpmejhu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3rmjkphil.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3sumopmrd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gufurjmi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tnphzikf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3afwddjul.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3mgzjbzjt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hnzwyndn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kzzsumhz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zovyrxfo.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zpbzqrhm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qkyehwam.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mbcvcmgm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eiyvntmm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3avqtkxqd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fmorhxkk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cueotghk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mubglbma.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3leunarzh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3pkwwwyfq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3gkuqdael.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hhaqbeui.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xkwcglgy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txvyhoaj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3telucfgb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3fsjjunkd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zmzdozuq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cenkqhvi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3incleiho.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlimwbnr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qqdvpihd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mrxtusqa.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vpmsndms.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vgqnrjse.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ckybdicj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qlinqacz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3blstghtk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3galbglqt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xgimqwui.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ivpsknye.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3adluzmxi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3eqsfzdvc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3kwpwxdob.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3pqpnveex.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3erhfxwfp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3zzylsoda.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zgqulkmo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3keyrumik.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3nttkruhw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gcpunvcd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gybovmvi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fwukpvax.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rzejhaey.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3idqtfwla.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xewguilk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3aabzpzpu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3wdrtkiep.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3pubgfomr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3oqdeatmo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3muqfmhxz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3biueatkb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3oypovlai.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hajafcoq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ofjtotps.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3psmsqrtw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rumuetwy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mzquigdp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uyuheflf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bddkqtqc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gouyyibh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxyfbzf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mjoozake.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3gimvbibe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jiyfcnpm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngdpjvnl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hmesipbj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3nxlnqfge.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kvyfbvxb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vnhzmifa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3njgppbjg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yfrpmikj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fnwbrwqr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ofkjpkbn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xcilzjld.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3fyqgotdd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3twbqwdfy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3asclwobo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xvyvppuc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zupyruro.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vgojinvr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hwnzdovo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bppzgrdo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3yrvkzqdt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vehobyej.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3onvspfhy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pdyxpeph.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ewbijhkn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huedrscm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3wmlulklw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jbiipxmy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ighorhbm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zgbelehj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3putcsjts.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3saqkwmul.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mqqiyxyh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3yvpnqrxj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tidjfpmp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3pxgyhasr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3trgagarg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ybflrgvm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tjvontdx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ajfbpfrr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tfuzupgy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zbdsdmrb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nhsdrgmp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3argvxiiy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3qewbqpok.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ivokwbvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vblmrvqf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3geneqiij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dajgkawh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xaskfxdk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wuoxmlce.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tzcnhdrk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ojtjskqu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xahtxiuw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zdmksfla.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvjwqpbk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kwabtmzn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fpdbxfsk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zlkerpfh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qcalxrkj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpbruprq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3alaosdma.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3swegaonj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dbpjzavj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cbtldmxq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3upkswrgn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gvqrlder.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nscghmfi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rugbezqm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etxogpct.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxfitsqi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gkihooje.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ozklmfwv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rztkztgj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kvxjspik.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kkuezehl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zyjduigj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3yhfnkfpo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pslyureu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nyabjvvh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxyakmlt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3piswsmdl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3efamyqln.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3uxqwoeoh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mbdhzyes.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xgmkijiv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3yozhgyxa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3beirhnvs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3swbombjs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kircyrcs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vwbtnquq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvdmlmrp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgcafkw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xlmbtjat.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gqhsrung.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ltoifbne.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovxbopyd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbpnmlus.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fzywfatw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqvuxtqn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3afawqnkz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3azatdfpx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhugzali.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gfyfnhvs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vczjcxto.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3thlnumpc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3recrhtal.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyadivff.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xdzmxeul.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ymvhgezb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pdvwcwgb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecetzeny.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yxhaifrg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3eufpvdzc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qrvcpsjx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qxmtdtdn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wujhdzte.html


<!-- 参考信息 -->