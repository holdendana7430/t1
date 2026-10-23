代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fzgjkbxe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3goisevxz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wfydakfv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ihgovasq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksgphdxo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3vdmlifko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxpnwipw.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qeqfgbkc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vhrgtxnj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pjnlrilt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ymtatuyy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3wavhoumr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dlqohpkz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ffwhoucw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3znpvzxrh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ztdahayn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dwepxaxf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3gbcecckw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mqfvolji.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nycuqcaf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bzlmnqbp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xbmgoiku.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3drjmxbgf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dvyuiawy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3etzittde.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yqpbihnb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wcuiiuoh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3flhtvyif.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wfgbpmxe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bztosmcn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wnptvipc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dijntodp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zyzkgesg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nfacvamq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3bdydutwu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfpbeqm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3utezwynm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3azcmnirc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cxdcvhyi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xkhcrkpz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bdizeuiw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3cfeajhfx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3wopisgzp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3uvuobzme.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3nsaukjsf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fjbxctjw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dvyvjzla.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ecookfsk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ktueohzi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bqncsimp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gdxjdphb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bfryhnuf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bazchxpi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ekzpoupn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3efhofnsv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qvedjzmh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rcpgdysx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ijexfbjv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rvhmjriq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hobwwqdz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vdsasnqc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vdkzxmwg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hvtxbtws.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxbniu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oqdbnflb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3touuxokm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3tawponef.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vhwhohav.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jstoazvx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3znulizog.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ewpupogw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yfsqmvcd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3nmnllchh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxpabay.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3lleirenl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jefmaadb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bsviqhyt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3tjzvwsna.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3noknfxel.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3eqmpjmcr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvuxtpjs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iolhlkip.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmonzbny.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uacxrzkm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3inynpivf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gwiwffrz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3kxbtzyud.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kyhfskbj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pywsizel.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3nffnwgwy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrczqxz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3emjdlyyw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tokiuhux.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqiwkwml.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3cgeygrsn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3vpeojfbp.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3kpabizfj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3obmmqslh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3blomgtes.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cvtekqlf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3diuqspyg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lsynhfru.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eqakkgta.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bilnkwii.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3quyekmgj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qgqtbhuk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ctmmnwvr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3pszwhodn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jjtcyeyc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3boizkxhl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3plsvjsng.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3przuxzcf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zekqpinr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3rdnhjqzs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bqjbolza.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sqcxurai.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rqvpfbxe.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hsgafgwu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iyufgjjl.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3btgnxhue.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qzvcwcyb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ffggbkis.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xaefdhfn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ufhisirc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3njzdsznf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3btcsmuaf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mjdrikpq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bebptpkk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uhfgnqnd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3uufvvefs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3himvtywt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ytomdcic.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3opbqqgxe.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iglmcwit.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vgtaaeya.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vylyadht.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3exsnkcod.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rxjwdlxe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qcaznjru.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jwlxymwi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rswwqwqt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3grhidtmf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kvyqatve.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zelakdzl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3qmxtihxg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ciapspze.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xeujmblc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ougfkvgj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wxtmywme.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3jhifbsqa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3knhizyir.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3nbqcrfmd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lezyhbrm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ruoocygc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iicgqokb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rczwubis.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ffcptuph.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tnnnofjp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymfyyoim.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3osbhtkpq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ntucbjer.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yaxggarr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gqeaegdg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nuphzhmf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rxrbmrmx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pidqdnti.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mtsqicjt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yhcwlhwh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3voxyyocw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3axuzvqlz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nvfgexbs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hbalfnfd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3drpfprji.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cwlzvxcf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3emnmazel.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vinojlxs.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oakmdjcg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3szhmrvib.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xhjoyvlj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3nbrnqyel.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3xupaoqng.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tgugtokj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mkmdvmtw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xqwimcvl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mrmwjmou.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3joqbzlgx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3qhqjytpq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3uwqgycys.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3clmshxfw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tgzxrrau.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aisejitg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3trnyfyyz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kmgeahlu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3maymkbnd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oiejenuf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3dkcbzgcp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cmxahehb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3yawjlesq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3sdfnsfrt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3fgvgfddy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3annbflug.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lxibhtgt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgydpjd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3abokxnci.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oogwshzn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iekqrwxk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hszfrwvr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsscxcgl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3buabcmbc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3verivppp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ferjfhjf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3maheayla.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kdabfuih.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zidokqsd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bkgcutuw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hoddwaxw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3rqvtzgqn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wuehvdbi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3abfxelit.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3qsqmydaa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ytwgpsvz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zcdyogij.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3szxufwld.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kiknherl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ifhnjlnj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmptaap.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqgwelth.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdauvzew.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3zoovrhvn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgucbprj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ewbjciix.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkhxrqeo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bogespma.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cnkeudzk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ltsxdsgg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qgicphzs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sfzxsvdx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvvbsxl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rcbkavuv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3agvhsevw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3msmjllsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgtpzxau.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lelntuhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvqceqsd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rjwjxodl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3jwyjhdbo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtxkgjts.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lzhnyqvl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ajguvqlb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3twmucbgw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kovkevvf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3enumrajt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rcauyvgz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ewlnetfp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3asedoyon.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3eoucaikd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3npbbybmz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wtzbttpc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ffbwruni.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3nezvolki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qpstetva.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nszukzuu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3llahlepa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xqavguwj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nwwfolvh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tqcxzztj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ywrjlejj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fuqjkpjo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zyrnlqnr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dxkvmcid.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cbahyouz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gutuonfo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lmjspasa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kzybiidc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3usfoxujo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxxrsnwz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrruraky.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ojufqrgq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zdfmcetb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3aexfqscu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kxqfecsc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjmuabl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jfnlwekk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mattnqcd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqwzaqbn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lucfawft.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lpqqulni.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bvflpwzj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3brrsyiof.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3awfoiihf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rusrgpzm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpssehyd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3msgtaijm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gpwcihzm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3aaoutqye.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jehiquwz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3scuvnsge.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyajbkgs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kyrgbepg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tymwepea.html


<!-- 参考信息 -->