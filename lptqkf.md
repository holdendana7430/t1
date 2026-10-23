代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wqzdyicd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvfhpmyr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vbhsfozd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ysanufez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tosdmwxh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3nvsgiiys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etqgowro.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dnabjgsv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bhxfdqrt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rhaxlsfo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tejadljc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3fkgxpbjr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3brjixbas.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3mdncqvxn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ciwwilce.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hjajwghz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3wiiwfxmi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ieqlzkoo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3khffiznj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dlttadma.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tejrglht.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ogddsaom.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3qeynchod.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hwliwzpe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rqiqveji.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3pfljeamk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ypsoveen.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vxuytsts.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3reusegwd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ovvbpfyw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sxplfjud.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bpqooedf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ffrjwmck.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cmqoqxqj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zoulidyf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3jvmpywhq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3aulqopls.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hjnotsmj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xxgvlbdc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ptydjmiy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nlfaepkm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3cyqkljid.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3uobtlwcc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3pfqsakpy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3czlvlhzp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cowvdwik.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ozvmitzl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmbpsvab.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tyibhena.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hpkdgqoe.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tzfgjvjj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fksqhgef.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zonxzhyo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dcczhwbc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qqerkqbf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zbgiimux.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wcycevwd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yfwlocqi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3aukloyys.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3kxvdpkif.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kwatmdgm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3maphwujr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzyhhoi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kmnialot.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pbfvqlgz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ncsrvxru.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pojuwzub.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nsldrrwu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3unylxyqq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wpqcunki.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ksidlcxm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3isjdhazn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3utzlxwmc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tmzrzknq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3iodpvged.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3axjjpatr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yuomoljy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3kkqnxznt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dfvomnas.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vdyhvhnz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3whmnkaja.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eacbgnuo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvkvkomc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3udmjdghy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbsffsl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kyzsgvyg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fuxgmapm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkgbqdu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3yimigkmb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3sagoesui.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3moeriglp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ucumdugd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3enkvpziy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pyzlhksz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ctuqjxot.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vtwtlfnw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3huyumlpm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ouqiyswp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rmnhtprs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hnadfvmy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dgkrybov.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pitwkeet.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fcvnayzr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zajxubic.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cfhxpgqu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kktydzbr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3xqknnpdg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dprhljtt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3daysmchb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hqielpsz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mvohurtf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3erhgtglk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zyoyroyi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fzfzmqjs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rjrtzyrr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rrhezzno.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dzcwcrtc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uikzjzti.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jqhkrhym.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zcdnggsl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3btgjlgrl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hhdrmbyz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kzglyalh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zslrbsbw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3loaduwqk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rqevdrmj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lldgqhhe.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3axbyfknu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cjzxjkks.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bjkavpgn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jxwisxeo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3edzlxape.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bjieloia.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bgahgkqg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xypusrxg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hjfsjkfx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bnjxrpvz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hmtcyxew.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3bzkgppab.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3dovpgcne.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oszkwgdi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oxprjipf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vbcpleyi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3nmzmofdz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3uoukxump.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wqzmfyhq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekrmgfcw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kntbtnia.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wrcctdeb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lffatvbn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfxzszkc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qugdcufe.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3maswicgn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfcxzgue.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3laobfnnc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iidxbcnn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wxgtdypf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ayebnryx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ytymcbxi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cyfpylfz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3izbvhtzu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lihurlkz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gctcifxf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3elyekouk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jwhmphia.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lrixosbn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3qmmennin.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3nwfassln.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3hzwyudsp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtjmrovq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cpxejxsa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ewfrlsam.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3agtcxsxa.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qgeraagm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3eksyluil.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hlnswbal.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sagpbytj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vgiesodg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hjzmghyu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fvlbszok.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bzqzzcqb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3dzvauhss.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hpqbfspo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wkofpskc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xnorqmjy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xmdhxhgn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3uivdjtfp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3klamcgfn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3loonxxbl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rmxynflo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tjjgclgb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjgmzadf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nemgsegz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qyuzgudl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3soawmvel.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wzykdkbk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxhauajn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3cvxiefkj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3tgsnpbgj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xbdnfmuk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ntdyaomn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xhketczo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njencmxw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tougqnbw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rtqtywla.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lysduhtl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zccxttig.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijabrycn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jbeufkfa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wqxbxpvp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ktvablsc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lopzkcza.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tbcutarp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hpqravtg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3qhffzayt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qfhodtmg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gccmfgks.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qydqpwcj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rtyotcgk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ivqfsiep.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jidwpaxa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yljmfnzn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3klxusaro.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uoouqexo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cxlmbrvx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3apytvptb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3khkqlnis.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ntbdovxj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzfwiqwn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnkzdos.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lrncidpw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yofllftq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jvbtseeq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xeiwlckj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tjjfetxn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xzneamqq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dstucrpj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3agcghlba.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3fwhipwxo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3brlvlnvk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3voiswrqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ueeadaqj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bynymebp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqlqetnp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kuyxebtm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vriwdlnj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3juagiuun.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3guyaurrd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3atiawmnu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mxrxwrum.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3uvujyhev.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bmomzbqn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zkkoacwf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pollvsvj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nuegjxbp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trnkpxdt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3anjnedsg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3otvlyyny.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xaiioiwr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3skyfonch.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tcvzlmod.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ypnyiren.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vlstbcgl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3fmokgyog.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3boqrkcke.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xvyfxmun.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rmrmiikv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlquzlog.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ppuxsmvh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gwhjzict.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bfgokqvd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjgxrwsn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iwvbzsxb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3aprwowvn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhifibhj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lbphtcjb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbsjuewo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jsaucdgz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3fxdocmjd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ooxargjh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3brdvfdlv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qombjjgi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cmsycafw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ithpqyqy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3txlpkezw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3skajyclw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vbeeihlp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rtgwgdpr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmazvmmb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fdxjchfm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cbslxgbj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulajtyub.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jubuwibr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpvuxiwz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hthedxdb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hjhotuuc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3davrsxfu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nerjipqq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3awbulfti.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3aqctxtsj.html


<!-- 参考信息 -->