代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwsmqatc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mcyeqkhi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zklrnhss.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bokhxrsi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yuaelmgf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ibkphxoy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gtjokezv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fswtkbmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgdyrdis.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3inzethgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhcgibul.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dinbsmzs.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nagawfdo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3cjhgrzzl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3afuzczek.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3iujwjdcg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xvadddyi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xiztnpug.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xtyfemcc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ygrqtwsi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ydqieald.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3xaswfavr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tugxzmvt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ctjxpldy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3fliriuuo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3niokkeoy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3twkdpjnw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3cqvmxajd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dwtsdyqs.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3fntxftqh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hssemijd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fzdwwmif.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cilltfdt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ryeyjxkh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eqphcfyc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3yvmcfmyq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xycjxujd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hdzmlsxr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gownkdqe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3pbrkjarh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3btscixsu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ywjkdasi.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rhsrfsqm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3doxpgxyq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3zmvxpbgr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3yhliiuvp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3uyyjbbrn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ifcyzdux.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3tdxahvkq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3prfiegyd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmtclxgm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3skmwmvji.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ogelcgoc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mmnccitx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jxnauyfu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bhljmcun.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jbgaukrl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xwxnzgli.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqofkr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rcxvndan.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3prsospby.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dhnzxpze.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zvwpstpx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3tdmtrjyc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hhvixzos.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vhpanqao.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yromxheg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qogicfja.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpjmhurj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3exymahwq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aqshjtzu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3kiacrzjh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ibzcfljf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pyrpoyno.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vzzzoejb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zgjebxyp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wxlprkup.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mpvayrue.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjtrxgx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3samvwwkb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pssmkpbl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zwqvgwpt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wettrkkl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fllfmxxn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ruggpcpf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ocpahxec.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqxhhgs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3juldubev.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbishcui.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ichtwwrf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ootlzwru.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohktmltr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rcqaisgm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3zlklzxyw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3musjznxq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3axprnzzp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kavaoxtk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3njlmibkc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3lfhwpicv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rswwiwua.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qouyvxwa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3lnywdnxr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3gwuyfgin.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ebhcjuou.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rxjoqzfj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tfmgguag.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zlgjjrfx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dnioltow.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yaqfmxqa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3topkdzfz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3buscbuwa.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkarizeh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3usloxpvv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vjruycax.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jsrejhhw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pvbzgwql.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ujpoezpz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3rtsnucjk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jylyglsu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mnoqfrtm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tkeeeylw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3drtvomap.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gmurojbp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bcacweeg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3djfxdhzc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3flpdwesq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xevkpimv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bvrynsyy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ygwkmhpp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3wfknjhlv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3otwkkdwg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3upixhzon.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kvpjbsbo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3iwzvpmdm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yvclrelh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3owndwtyf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kihmovsi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lccjgbrm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ziubjcli.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3inyoupus.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wovifeok.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jdcbcujd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cecmrwlu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3sqvxezjn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mstbbmrd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3erqzmpfi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wqeavejk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3szvfuofn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3tixsuwkt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3zkkjkesk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzkjrrgy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjtvhbvi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3txzuanla.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3egeglrfu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shmjddnv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3wvflexje.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqmfonvy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qwkogyop.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rlokmtsv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3judnzqct.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3shzzpqwg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sambymjc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3prxzkmeu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mgvhnniu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3lgaegops.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3iozkluuk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nbgtbbou.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rcssfesc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rbjfcrdl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3iwqfezrt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3furyfdpa.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mltdloqu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3boovuwsp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lrcqdllm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zkpngmib.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bzdpbrew.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rofhelyr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xuzfprah.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vzymydhr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kgdnwlgq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3scowmrhm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3wpcehhnj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rwbqizzs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3foqkcfsm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fylzakxo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kkhhkdsl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nfuhacxu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3oajomqoe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3dbcinpeg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3jzchaaab.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nmexvxpc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3oiivkheq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vtvqtfpc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hkvcsujg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cxvrhvqq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3trqyfzrn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3njocpcjc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fdwctejl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kibwfbou.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xvttxqfi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yiyvqgwo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jduvxlra.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3pjmbdkqp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3qgkixjul.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nokabqhl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hbnxcasq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zxlzwfno.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3uwxfcmub.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3trpucxgh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xjylwbwy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sswgtfan.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wktkhwuo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tonigqsk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vflhyxlv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aojqrtxu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yurvtjtr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eqtdfkay.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3nthxqxeq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ryzpaffr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zxguhjys.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yolsunox.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gjdynhnv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ukhywghc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ntlerpsx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tnsridkx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3uqjtrcfx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qxlddgiv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3owdlvwjj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3szxxrkci.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjeyazr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohllmaxv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dczqhfnu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gaycfppu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzpkedtl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3owfdyezx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3masrivyg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3uaomrbhr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3kpvyqhet.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3sstmijuh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3mqftbomv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xhviwmuk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3drrsffqo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dsvxdjdh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hnmbtzgq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvdgpus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thvsebgy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vquzpgug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aixdjxeb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xqvpfqrj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3waawqpyg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tpfkvnmr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cndulzqk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ibpwemku.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3plofimcs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3cgwgoqxk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3praddbux.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xhlhfuak.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jtjhuqnz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3bcvybggt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cffvzbei.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xcemgozd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ctvmdfre.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ojuyxgnj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rujlayne.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fzameirm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3agjlfclc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3olflzcpv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lvrotwik.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubtenfyu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhnizvym.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3llmahlud.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrryvfh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yhemvvvt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3qzmtvetr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wtsdpivh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmcmlmio.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gazxljfs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdjciqdj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ncfupwuz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpilvcd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3plvvhyve.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3oeulijdt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hdyfjgbc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmrrfvo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jlhgulsk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hbftgcho.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3muspocmo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pfvljqka.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cnuomveq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3letxjrdj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sxidmdro.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hwpelycr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gfmilnsq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bowhpnar.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ltfmindo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bducpmfe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsobagmz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jztgijev.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufhdaljg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ccpgdlfk.html


<!-- 参考信息 -->