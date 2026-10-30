代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gtlqmkgtr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gzezaflif.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpyqugmof.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gjyihitxr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gnbhunmri.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwmxhzumc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gabqydiok.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gawixlfmy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gegedlkfd.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/giknuecjg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmxaqqcbu.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/grnvcwbmv.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/ghtaziise.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gadgqgriw.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gdhkegsuf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/gdjoylwvj.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/ghqnqgqdy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzhragvu.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gnsczvibt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gryypknqn.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/ggbokicjz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gnmgzlxmr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gohjpiakv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gfksntiny.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gajykmllb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gbffjxdpk.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gwjboghxr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/ggjxgevov.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gyornqpnx.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gjyxqesgv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gmxnfxpwv.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gnbkmawih.sHtML

JS:   const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkmisdtyv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxnufkwgl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gampwpfjx.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/glsbzzcha.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gzdkxjidm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gghnnekda.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/guxfzukdz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gheumkyyv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gjpzdjhai.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gkkmqbmjh.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gdfayfgie.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gmcooyewx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gqdbdnuae.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gqkanxdww.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gqkhqczft.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/grcmfnkdp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqgaefn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ghopillef.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gunwuujuw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnqbtauei.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/glngktxat.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/guwsxpvaf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gxfojbkrb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gesgtflox.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gemrbmuoq.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gozgwjnif.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/ghzeztqbs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gdzvupgfb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gjsbapbjt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gkznhbnwf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gvdscdvgt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gbmkbvfmj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gdveqrwac.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gvvbcajcn.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gubovofpq.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gtsffvbol.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gyhycjlhc.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/giwzwamln.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fehbvm.com/Article/details/gdbdxvnto.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gdtgblwtq.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/govvhejww.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/givznaufd.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gsdbbbcod.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gokbhyxuc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gxikqtkyk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gfhlidjzq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/ghkpqrhem.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gfrlchlds.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gdnblrqtv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gneizbljp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gvlzvcwrb.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.hesvh.cn/Article/details/gxmidzvkg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwoihxunq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/grzrsgvrd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gntmgkvni.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/grsadiqmn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ggfibnyul.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/ghhkblfam.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gvgagdsqd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gmgxallzm.sHtML

[A10] 生成随机数
来源：http://mobile.hesvh.cn/Article/details/gbsdphfjn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/gqcdtckay.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gzocufmpi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gkawtbjuy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gkunbafsj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/gxnwejsde.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gfuzeshtl.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gzjfyofdb.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gyanynwgn.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gqusewlzx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gksnijnur.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gdmncowtn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gkkmbcklk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gqmkdiyaj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gbhlbqcph.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/genbrpzxb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gmwbhovgc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gjzczdfwr.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/ghbbokton.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gznmntlmf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/gskicyznl.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/glnsqnnkf.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gpgpifxdw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gcnheihoe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gtuqiaouo.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gldkldhot.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/ghwippujn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gbevxxjgt.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gmqqxiuqu.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gqxqurbbc.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gkootcgzd.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/glbwqrmrp.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gidqzjwao.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gdwbvgapu.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gncmmrwlw.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gmwjruuuc.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/ghumxwjpc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gxabjrjkd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gujhbclym.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/giobjqhdr.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gsulyhxyb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/gyeoyxxzv.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/geivfdphx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gdiqjicay.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/geqqogvnh.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gotcidkmb.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gqraykioy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gzxzfsfot.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gcpkgjoha.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gshfqxigw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gauzsnbjr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/guuiqgjhz.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gzkafhwnu.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/giqquscpq.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/gfnrprjrb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/glzxmmtoh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gqfytozns.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gizoewnmy.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gqgzavoqa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvjsihzqp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/gwvjczaig.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gejpsxubj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gxiwfuzqy.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gquxfypkq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gmjhbvmkk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gvjsckpxg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gugetwyoo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/ggrtzulxv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gpethurji.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gzetuidcq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gbythnzrp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gerhxalad.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/ghgsltapg.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gudntqazr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/grylxbxzd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gngeejlzc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gjelrzbya.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fehbvm.com/Article/details/gcoyxgprr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gmbznrhpr.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fehbvm.com/Article/details/gopvxacid.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gaifuscgg.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gmdiftgkq.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/goljbucog.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.hesvh.cn/Article/details/ghdqswbif.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/guhqpjtgh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gqfthbrjv.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/ghfyzbimj.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gpnfjvayq.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/goynqtbws.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gicnbyusp.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gcehkkrkj.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/gpgbydtmi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gtkluiaqc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gqsbtsedj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gmabroakm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/gqwlzqniu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/gckqxybxo.sHtML

Ruby: gets.chomp
来源：http://www.blog.fehbvm.com/Article/details/ghjcvqykx.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gklksnqgc.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gldbwhwwq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gqrvzkfgw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtsjvdow.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gsgsrlpjw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gbutrpukc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gqlyahsig.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gmiitdwfx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gttdettkl.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gsehsqavv.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/ghmaclknw.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/gdbcwvcpa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/gsedxvsot.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/gcvseymxc.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gzhxbnpfp.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gzvpbcihr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goywjbfcv.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gigqqxqlj.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/guhvcwskg.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gdwyayjmu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/gcaeoeruw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gfjddhtbc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/govasygmk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gxfihhvmx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gdtieralu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/gojeiowqd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gehaixynj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gyujghhzh.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/golvsaxac.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/gcgerqvds.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/gcvskhygn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gamntitwn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gamvuiwqm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gqtxcvxft.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpooakcqo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gcilfizgg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtkyvvve.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gajidsjxa.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gkrbuqnyf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gutjkiuoj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/ghbjoqlyr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gpqcmojyt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gxircigjt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gmidvozwj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.hesvh.cn/Article/details/gvimeorut.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gmtdzxlpy.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gplvpznvh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.hesvh.cn/Article/details/gsgptjrww.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/ghoctxqke.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gwjnydzeo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gxutipzbr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gsbzactwi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/gnuihylwh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gpxvghcom.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gtxgajkic.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmvkjwcgv.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gkzapscgn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcwepedcw.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gzmovurtx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gxracnoex.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gmyntsskq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/glavsjjmt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/geunaguon.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gfhqzmgfr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gwdghsfsu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/grttsijtp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gdpuaipaq.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/gubcwwdtv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/grfvbivub.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gnjvkbynf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gmmnbiemt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gdfhqpkpo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ghlaklqhm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/glmwjirim.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gnzvvqdyd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/glhzasgtc.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gjqfvnimi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/gxahppvsm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/glfrwtjad.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gzjlggbvh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gujalverx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gtqmlqkao.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gmllkvwzh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gfmwtrgne.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/goqfcgtgn.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gipwrvtso.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gdpjuuuun.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/girufhxmf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gbuclwoze.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gmzenvgjn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/glvwfrdtb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gfnhrrols.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/geklbayur.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gpvinckhw.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/garcxfhzk.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gtxxxqrty.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gzszveedc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/ghqjssmjd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzersej.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/guzndinbu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gxecwuhxx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gysrwachu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gqoderbml.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gkhyjnnda.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gnvbwzmil.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/gwcnmvpgz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/ghaknwfha.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gcnmysayc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gizzezcln.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/giqjbkqar.sHtML


<!-- 参考信息 -->