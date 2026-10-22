代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gyvluize.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fwlhcrtz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bavwgswx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2agiqtifu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hcfstvbh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2hexvyvaj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pbvmtebx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uypejeeq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2sikompna.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2khfbcguv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2xstxovju.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jibbjpqg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gfsxtrwc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hyhvmtcy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2mbxvzkox.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xgvpsbla.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fpitpbmw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rlupokal.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fyoubttl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qwcupzqv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2iixwneug.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dtfbopgu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2oxzmezph.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2buouepcg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvmfmic.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uqxuiyyq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qszirgur.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2rdhdktiq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2mesxyhok.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2erbtupgq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wubskhtp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gvxrybmc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jhfukbvh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rvsonfnz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wkdchnhb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmupplqp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2otzoermr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2askxujyt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2akklgzos.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2odkssmfh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2taxnvpxa.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wnqnovhw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2lzsxlvyv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wehhyqcm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wsntuaga.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2krxzlhya.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2iyvsqisz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2cegfguul.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zeesgdqa.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mpbjedck.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbdqdgc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hsaibqex.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2imefautw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vfaqummy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ptujiqzh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2qeqogfqs.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ftoywmcg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxqdjpoi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2mwxtyiiw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aqamnwfb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2cetmxsxi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrgukit.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2gdxivbtr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oindpnkt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhusiez.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lvlbwdee.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tibevpmn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sciatoar.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqgmefyu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxauiaxk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nrzgxhfj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifxjflcd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hxvhskyp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jggzdile.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2carzjfhl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pjhnaxah.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wchysypa.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rdvryfqd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2djgxvwof.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rqjyoqwb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqvnoonm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ophjpkbs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2twgsijfy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2eimbfdcj.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2cztfgqjf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jpabjpqo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uvpgqokj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vkhjhwjs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2scqvlscx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2brhhjzuo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rhucxhsw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2nyvhedqw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zlvpceqk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zaraousv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2dvajpufb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2tchlhjst.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wdmfnoye.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2skyvuwej.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ndjtxkcv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ohcjhfbh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wxmnsxzg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hilymscn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xyzyfjli.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sbuupxup.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2haycwaly.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggyoqsll.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tqvfhlkg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2spohrvlb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2scfoqvoe.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rppftzjl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iymzizgy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fzuonmku.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ceqfqfke.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2mhpwgjks.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uhpkfrdz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2glmlgssx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mwwbvssq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lqysybzx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oytszovq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2goncvvai.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gkowmoff.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fdibpkur.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xuidelrh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mstpxkgr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qygvusdx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gvugzkcv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2lhrqmpfa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2olctwcfd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dqisbvku.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqxwudce.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ffzdphap.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sgndhyhl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2nrarmsiv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fqtwymsc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzkezobf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2fbyndpgu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wxgkrixg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2joyxtluj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unbgzswy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tfhjkhmt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lhzlvcgw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vmvjskxe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mhelevof.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2udgqfnov.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yuuvjuhu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udiqhlap.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2esswkwnr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lwczdwyr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2bzcqaloe.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2upfabfcp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2glexdjsy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xfejatdp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2evoojodp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2mnzqubbx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mlwcltcc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2kaytgqmt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hlvhdbib.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2eqpmoniu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fmuimjic.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jreyzbev.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xnxrfqxl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ipfsonal.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2tspdffza.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oaivzrsz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ffvrudok.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2cjjgyckd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ywrukfnv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2hwymfdqa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2fouksiog.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2jfclsytg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nzvezcvr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mdahspqa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tbmcaqzo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tahvkceg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2meqqqcxf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ovlwdgqn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2prgaduhb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gritvpzn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlbowmt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkbnkqaj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cefapxcd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bluufxuk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2opzfkyzk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ofcdwamu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vkpxvryz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hleylzgk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dgacmkst.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2hjpaitra.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2cslqmepo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ctcqqwag.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvgruos.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwyxawng.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tqheeold.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qysevkdq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rcfdqcpa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdwetgn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xqqciocv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nvydhnxy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lehsytlq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zmwxdkyu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vjscnwqk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2kaxooiqy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xwzlplbn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2sqjzekii.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnwkbmq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tlmwstzk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jqkzmvne.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cobsdvwb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwkfhftk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dqqzurre.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tfhlblra.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wqogrczb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kadkueri.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhmosgop.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2evzswkmj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynqkzzzt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jjxmrgdg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdjjgrq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2cchvwerr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wdxkfymv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zuqgoiim.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lrpbuubh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ipnietqe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2kezygnhf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kigqtobq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2abqofeje.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2aooullxt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hssskrji.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qadndshm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgzivgfx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nozneoxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veaixtyr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vlucdvby.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2tyloeoze.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2oyurxsyx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uyskhmsg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2klwsrqcz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2plyoioet.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fgwixyvo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wqmmxvrr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jcadxbsb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nrubruhk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2txvvyloy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pinqkkvd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oilzdlqj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gguizmnf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xeklayxw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kgctvscv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yihkoxnd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rkdvtqfp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2aypewwgj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2scafryhu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qzzytkgk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arrmzksh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztffkebk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dzwbytkg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zhsfpwio.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2isnxdste.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wunxqegp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2okywjflg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xihlhjdt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hepugzjt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctfcwccu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtdvvxar.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfytfvif.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cndvpgzk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hanpjjpx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2aikdzqzl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjkopkzg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kdpvntke.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zuojnlxa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wvsqdutu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2emslxkvo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2eizovysa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dafrzvsm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2esumzhot.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2htvslhev.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2spgzabua.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnyurra.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqwwugsw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2banzzwnp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcrsjwom.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iocvsnvi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzxfehzy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ukldsjtm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2znfjivpc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yqpwblxb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2prrgmepw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxihkixd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ihxecddd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2azcpbcvx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkqbdzfa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ihpwtjtq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2byrqzvrj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywozgmfp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mfmnfccv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wjbwwecf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fqutnfmf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sxruduns.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wrfdutjn.html


<!-- 参考信息 -->