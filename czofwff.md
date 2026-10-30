代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gukynyzwp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/guhajlwbu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gadspgotd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gibeccbqx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwocftymu.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gfzjfnhzu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gegcllnqj.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gmguwrzyz.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gmhhrlxja.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gkhgbdjeo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gufmvdhix.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gveuetfgb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gpcsjismm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/ggkselfqn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gvvyxptuo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gzshtnppv.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gtwrekcoj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/grjcbnfll.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gdjvwooys.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gixzrqper.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gfcxybynz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ghcirvbyv.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/glladrsjc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gphsuegkm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gomuoidnr.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gfhaeawtc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gjaptpjiy.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gpygjkxle.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpoahxfhb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gqsujzuhg.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/glmxukdna.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/ghmarbqwu.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gnncwgjot.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzjbiyywy.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/grajtgxwy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gxottykzt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gebqyrsqk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gyfsdfuie.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/guxltsyft.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/ganankndw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/ggkhohtmm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/ghksymodw.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gptqlnvdx.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gexwbkngi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gdnqpryxs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gcjfmusvk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gspqcxywa.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkjnbceuc.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ggxfthief.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjbtiehft.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gnykvzjbc.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/goqymxrqw.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/gmqnqcfki.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gunaoggzn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gaecknxmb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/goertkncv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gibhjjiio.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gkpnjuuck.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/grjtbbfoh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gdkozprih.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gxnzehvrh.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gwgtwsxqa.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gsefxlguy.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.zdbjq.cn/Article/details/gvhzmejfd.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/gxnppkovk.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gmmnmlwaf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/giseyezky.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gdztwhsty.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gwrskwxle.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gqlekacsm.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gotusdhwn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gjxlfjwbe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gyxdzewnn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/ggfslqvvy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/ggrbrybes.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gwnotyjwf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gyfgibhlq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gnfsjpnps.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gwsuomkyk.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gxotcezpb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnvuhvztv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gonuiirmf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glmmlivhc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gprmgmgbb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gbnghtxar.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/glrbubsdu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gozngwjpb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gnrsfpdjw.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/ggyptlnfh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gpgtyzlnx.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gdsqgrlwn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gwvvdovbh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gnqfueyrr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gxqbzpptd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gjvfewwqz.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gfcsuetpc.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gyemnkkvq.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gqklzeujt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/gdmhjjrdh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gsotnynvy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/glyrwijwo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gattxespi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gbeoqyqvk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/guzemifme.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/givcaxktd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gnpoajejh.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/ghwyxmdis.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/ghokouhmb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/grdomljlj.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gwrnptrsp.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gbujwrpqy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gjorvldza.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gkdrqtzxy.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gnorowibc.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gnebvaplm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gtvkgocpx.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gijsxxxez.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gcaszxoum.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gjzbhdhfv.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gsvuecomb.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gsdmjyphw.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gtrointxs.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/glyzvkxjh.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpzdnkabl.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gsnxyulvo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/gaylmdxgw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gayvbhivm.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gylbkjjrt.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gvavpdpgc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gnkdnbwlo.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/geyplbrdp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gwwpiubrn.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gyccccgcq.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gdbadkcmg.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gngxeyrgg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gvnuhwsab.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/ghxqkrkbe.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gomjcmufr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gwkxwlqcb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gdbugjixu.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gqxocnatu.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gojgnalvg.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/gxtiwrkjd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gdzxdiqbo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gzbejmqjx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gjesxnyas.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/geidjspba.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcckgzojb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gfhsbgejb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/gatgmausw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.hesvh.cn/Article/details/garibkbym.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gvwnbbetc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gdkykghze.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/ggwzggjeo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gwfqilvdi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gjyivtjim.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gtkswmsdz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gdqdnvpls.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/grbmchbbt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvxxzai.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/ggtbqxnpj.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gaupvmseq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gigijfixo.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/grlnjpkjf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gxuyfffas.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fehbvm.com/Article/details/gmeyihmng.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gruczpirl.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gdjoyoscy.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gfwtvhyvl.sHtML

[A19] 交换两个变量
来源：http://mobile.hesvh.cn/Article/details/gmfukhaay.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gmdvszekp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.zdbjq.cn/Article/details/ghiysdatm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gxzxhjtpk.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gqglpywhu.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.zdbjq.cn/Article/details/gnaupvnzh.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gswtheklh.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gysmrdavx.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.zdbjq.cn/Article/details/gzawwjluq.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/guqmabytn.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/gaostpmas.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gkbhtnkrx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/guaqijwuk.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gvyqucmoj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.zdbjq.cn/Article/details/gjbdrzyzg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gzksywilv.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gofjvulip.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gefruvkmb.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gxryxzodj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gxsxslkqu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/ghtyjaqun.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gavuhrqzt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gzltfyqqd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gzvmruygl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gefderyya.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gbnhcayme.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/glwzwfsiz.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gjcrzbrft.sHtML

Py:   len(s)
来源：http://www.share.fehbvm.com/Article/details/gsqqqawzd.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gajngnthg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gubefbezp.sHtML

TS:   s.length
来源：http://mobile.hesvh.cn/Article/details/goqrfyeck.sHtML

Java: s.length()
来源：http://www.blog.zdbjq.cn/Article/details/glptbdpfy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gipbitmxk.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gybrnsmtf.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gnwsdfiec.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glhfxsitq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/ghbvzaxbh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gxgyoinrx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gbhzvfkoj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/giljhpvwf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gmzhoveve.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gkccdyeya.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gylrdhzxj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.zdbjq.cn/Article/details/gxogwcyme.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/gqqdramvj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/gnxxmzykx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/geawnfrxv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gvrkrxobp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gqismkdmp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gxxiyuqhk.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gdtqvdzfn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/genibvrlu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gvjnwfuwn.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/ghruedtky.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gmliavqev.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/grndtvfwv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gfprvufah.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gutiiwhmr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gpcufumem.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gylewvnnv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gnjheuiof.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gnpnzfeyd.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gbsqiciyx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gsjjkicfg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/ggvuljxqq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.hesvh.cn/Article/details/gtwgfbdhi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gghrrsymv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gczhsguzz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gqxrzzawx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gvvdkqped.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gmjsodqea.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwrguuppl.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gqxwnvbnl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzctumnic.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gizhochlj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/girsjiria.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gjsjjeasc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gcpirasbx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gspkdwslw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gxfmiblqg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/gqokitdjj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gdrgekwxi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gawpihdjh.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gjhzoayhj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gmsqwoatl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gygeardao.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gumvxjket.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gxlvyblru.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gzfkcftep.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gtrqzfnhc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gtlnxewvf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/ggvzlssum.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gvihttgvd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gwhkdqluk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gactdflhb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gejpzzwpc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gngltgbfe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gevokcocd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gzydnqyqz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gubroxhoa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gtgtbstho.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/grfjkkfsn.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gyfagnojt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gmbtwziwn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gdadmjltq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gaaiibyqy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gdjmvxeac.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gzrcfxrzi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gjzilmhup.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/grprgntfx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gwsjbxlaf.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gxlumqbki.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gciqdtwiq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gqfxjoyac.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gckugxuvg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gscwqycam.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gdrfedmjv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gmrosgdel.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gwzbakgon.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gwiszgrlt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gvzzlejes.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvcekra.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gkrmtmsvo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/ghkmgxrqn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/giijugxll.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gibyqplaz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/ghponpfav.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/ggonbkejh.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gvovehztt.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/grmcnuzsp.sHtML


<!-- 参考信息 -->