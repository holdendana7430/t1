代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nkevyupe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fnleveed.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vxybrvph.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hkgcyzca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjbjxffu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qnnapchw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwgcjuai.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fiaxxemy.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wjbivxlm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3sesigezf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nzuzwzoz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3kvbiwfhf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ojagqjjt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3whyruftg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3cqcizgyo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zlrxjxib.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ecrcbsjf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3bthsaeri.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fgxmzfxu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qdamidgx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3exqhzcdm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bnjfaqpn.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3syoopxqg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3vdfddscc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rxkhotga.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3czfcdzhu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wrvzrdku.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3araxhgug.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xmjjuoqb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bjcojcab.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tgzsffut.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fgryzyjk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wpwotkgy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3afbappld.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3uisoxxky.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3xfvrxcku.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3mxfsyiyy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rkwccfpn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mulsvmrw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bkkqxrgi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3smimgalk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrfdtdq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ldfrdofe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3zhikhxef.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3dnonbpeo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tqoqywio.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ysbitbts.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oxjpnzxu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lotaqaeg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nemvvsva.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eyyauppj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hgfgydvx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hgxbqcfo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yqrvwmhi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qrrkwkyc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3beaejvil.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ovkzvfmt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zievelno.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xghoufit.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3klqdljsu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3voyekcts.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qookiwwk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bmmckhjz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3bdxpozsk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ilashxet.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oqprxomx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3yxpqvigv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tmdpoept.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3utcjrhfw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3khyrwqau.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jzpnxcxy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3aczbhhuo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3hkxfnoww.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qlzwxfly.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jiahabnz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kykuchyu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ddesxwfu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3axzkbgmf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uwcnrznt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pddwerof.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbmjqna.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnclbbvm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvafeopw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ypvafrlb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lggohyok.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3goxdgyfy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3smgepbmw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ejxqywqh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mgxkurgt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3urfxzcap.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nzmrfkpn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pgqslakb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jvzoxamo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3myipowin.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yighrpsh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3czvurckk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3swwsizbj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jitdmexy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3nryajhoq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sogunapr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3brsnaopn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3phqieyxi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bqeefeyk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3eesqbkch.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nrboxwcl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lzdjasnz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3szjsgswt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3lghpulfx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3kcjzbvlr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cfnvjpng.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lzipkmjv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3zlqsjgnp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uswilafs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xpmbyufy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wtlaosov.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3feoryqum.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ijurosvg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oehqozht.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zeazkblr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bjhirhpj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yepfzykg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rugntvqq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wimtnmlo.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kektwauz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3mdwjhqqu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xhcncqhz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ntckbaim.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ggbutzxe.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eldszrfu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mvugzogm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zxevkldx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3yjjpdbsd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3itttwkxg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3uuqbkapu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3owgxphnf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qmhkdykf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3anppdgbi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bnvvjltk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gcovaxgb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3essgeowf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fskbqebo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hblyufnb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3rcifzkgu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3chtdutwb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3xueodoqr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3abbfszfj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ntqmzwcu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3szunybbt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wrtizfci.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zfdzdjgb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3swghqsrm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3dzjfukzp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jggakcsf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wmmqsmnj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sphyupdl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ixwynimw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzjguapa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3itjjvtuu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eblltluz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhaftmgk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xgshilyn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pfnwmvak.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yocdwtmb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sviciqav.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ncmtwbgo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3bbgtvfcm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fxtidywl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3yivatuge.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gitfpbrn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3xvndoezr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gfawxxie.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vtjozarb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wrsiyxcl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bpgxfwxv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bgklcbls.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3anvflixd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ywyccdmy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3vjhpceld.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wccmutsg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ylrvdlnr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3sloxvkkn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jybweqyr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3diblzgqq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3znaypkon.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3klhylnpg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wlaztcyt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dmncfxbr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3pqmwvzwb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hfixcklm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsbpwzd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xwtwvoad.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dqhrbzgg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eaufjgtf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfvtosc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mqirlcrq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3nqkmbgwu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vpluajiy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhwdvpno.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jwvrskqy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hdmgapie.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vxpsqmaq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3szbbzcaq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ydarjcmh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3epbmzdwb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3eghlrtfv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugewyslc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zfytengh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wueeglgy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xjeyxxov.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cflzltbl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nbmriqde.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgmrfovu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yimqkgik.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3klzdnwep.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3swepxpqb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3noxapdok.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3soxugmhe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xlgaprsd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ipeocaxo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3alwjinvz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlfgibv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cxglsujv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xtcwmkdi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yrqkaaah.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3hqoxrcjn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ntwyxwjv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tnisduho.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hinyhmbd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zuuehltf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3izaomnla.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nkkjegws.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dnlekxqo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wlwlqpjj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rxobdify.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lykhdkpj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3glkgrtpq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fprfuobh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3auvkuoyd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nnlvhcre.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wkunisqo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cazvtbna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wflrhtfd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ozvizmsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onznlfux.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hhsgzdir.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dudpzrrd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwigyaz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3afnrhmun.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rlcsqlmd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nsbueqrq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ugkcfppm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fhatzcra.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rcmmxogi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kmuvoeep.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nvbefwof.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubyoeusb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3urffxuvx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nbjighsd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ysftnqfk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vygtqesa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xvwhkbrt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aytgvybm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3iixdimyq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3virxkoit.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qkimuyos.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qlrbwcfy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wlpellbs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3luckgmyd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3egfrbuxb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rwpowwob.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xzmmdhfq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3exfikfop.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3clkubzqd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zafigenk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmkqjhwj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucdeykav.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ngjixyta.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdrxbmne.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cfwbetam.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ghgkrmui.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gsxnukff.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3imdbtaxk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zewdliov.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3owrssewi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvjiyeok.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wuetjiwu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wkwnovdb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jlkklmfs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hnelxpgy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mnhxxuuo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qodgsvvo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3famurngz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zhcscpyt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3joqihrim.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dwwyvhfl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kvgmnioi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yxgyibqv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3psemktmw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hmpinsyy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqmofxih.html


<!-- 参考信息 -->