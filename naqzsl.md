代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jkrpjpyc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3usydqljg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qmfqxayl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3vxpzhgnc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fbqlgwny.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wwxkfvsu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3cmrvotpf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3trhdovqj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pwcjtqza.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gxgdncyq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yhvvvemn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jewdlver.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3txspvvti.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tzstnykv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ablnlexv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3kizjqzvc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ouphtxuv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mbhhxtve.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ejuqdrqv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qyngcjwz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ryopganm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3osmqfdfo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3osbrvqcb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wpojjlgs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3jkkzhetx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3imczaart.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqnbyqfc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sqsnkldc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zawqbvpc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bspxekua.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3upcqpsbs.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrfyekro.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wrgmoxiq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3owtrrbrk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zvzlygdf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nlfqluki.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bqxwwqxz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xqwtobsi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3wnqmfhit.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ytwywzif.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qoukydui.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulwuebmm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uuasdozt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3yjicewto.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3unnggite.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3voovlstg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qjjdqrka.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bdfpwbqp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3wazxptuv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3howbehlw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3zumjqqng.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ybfuyqyl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3kcsnaljz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3npmfrhab.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fpejotdo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kmtlkawl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vkelfpgc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zcknnwse.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ycobeqdg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vhstgbmv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vszxnrnl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bpgbhvnp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jhwqqgnr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tynmyixv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ubdfdtps.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3anbdtsav.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ruxabuub.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tzgtyppn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gqyxwuqp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gfdrfjmt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3xwlzoccq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tthhmcdx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ughvhjel.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ppeezsed.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qmtrtnre.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3vgqhkrlo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3qnrdpzon.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3mopyybsm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qbdpksir.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nvvwzmli.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cjgqrhnn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bodyvgdd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cvciwxtf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3pzhszsgv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dysmzdsf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3edeftabk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ydvjauub.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3derwovuo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3wzmgnawd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zznggcai.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gmpisxha.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3pefihvdn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xyfdhalx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ouarwntd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bgvkoolb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3yxekuvxt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jeensenl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mempcmfe.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3acprehxo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pbdftdgy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gqboprjx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qqqikfhh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3krmzkjoj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uvpfzuoh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hgmcmbtb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3uwjaqima.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3peqgbivd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3acggruyw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3azriawmu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qizbxtpl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tfmfxebs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3iwvxmail.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3azorclil.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3kojpvqtm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jgklkckv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gobuwfzp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dffwmsvj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rvspflcx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3odlbndtw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mvackeai.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rlzzocse.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wuqydpqs.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3idmzvitj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kqfachmd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eztmqfto.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3gtestitk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kgnigrhi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mdktqdxm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3suvcpwub.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3irioptgj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jdpkwaxp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bhjwkwky.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sppkplnr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fuxmobba.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3svlxebka.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfcpgmst.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ccjsqoko.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lnyzdaoh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jntnasfn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzazylnd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qxfbnaan.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kilklevs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wdqntwvo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kdhnmudw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wkrfnvlp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3skiggkjt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ityrmwjp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dqnsqzpi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cykkmpyt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kgtdakac.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cdmftnci.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kifondfk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lltcijga.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ubtntpam.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jnzzjfez.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rujseqoy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qjxqexxn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hsshppda.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kegbifbi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3geccukbd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nmhreigy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rotcrfyd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tzoiehdr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3icmksaes.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dvxfhssw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3elkhjolb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fykwvnwn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ouaptmob.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vxazycqj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fjukrvht.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ceiepeml.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jxfplbkn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eqcpwlrn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pjsfuiwp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3umepnudx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3regndqci.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3muvjbdni.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjhqbmp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3sgcdxbig.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hpwccyvd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gijjfwwk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qpcwfiqb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtqbrgh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qstcpcvn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wlxbvbmh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rohyihpy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zftmvmfy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3badvykth.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xblyqnzs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wyttfqhc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3byvkumcm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxozmsxv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qwxhnqnb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3noklowje.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ojmvrota.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gducnajv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvhsdgqk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zugmlpyp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vycadjer.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3isosfnve.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymigazzh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lddualrg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nkjvixxn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uyweuwhe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jfyqgmmf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3husnrfcj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iebidwug.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojazkdtq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ppbewgez.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbtbccd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ndtxoafh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yixvdila.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3exbtcdto.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3llkejkhy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvehxqo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3lfpfpneb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tcrwilsz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvqxtsu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3krvlphje.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jrskcjyu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tcpamzak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvilaqdj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3krinobbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruexvsvr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3grrmgvdh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dqsvwwew.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owfbnfor.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gpexbhrm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jsbfcgef.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ennmhyci.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmwjmlks.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3iicbqagn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bhghbwdy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vjqjcbim.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3obwsbzje.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oolyeqfs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gerqajcd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fejdpxfa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kdawfwts.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtgbnom.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ldntfcxg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gfqblpel.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tcczmeba.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3yruobinj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iscmotrq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kewwfbjk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3loxfqnhf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owgiboiw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qbiohimu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yveuaajs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yxlrjoli.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dpdosqzy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hwxpbmit.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjjnzfvp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpwfplqp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jihokery.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwqtbdli.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3eofkihbw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kcfckdhf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3pzpgsbcp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lnyavhvg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3yexermaf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vqfthnyn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3unnstiho.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsauraux.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgevkdwr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3liiftjtk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vqukuspc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bouqixdu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vbqkycgd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jibbtabm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thrvyxun.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bvxrmnks.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jfeqhklb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3opukxint.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nztfkujc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tsenbnui.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjovsstf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sklcsxuv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzbbmbey.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwfsgwib.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kopbemiv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xbrwwskx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qtunajwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rvuaxgbw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3iuxhkonz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxfogdsa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3syuwciws.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pwcnrncm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pwlwfbvs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uplcqxlx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3phrbooha.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yllskqry.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cvktegud.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cqocdowb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3umbgeaym.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qpiktxtm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jkisujdh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilakzuyl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vdlvuwkw.html


<!-- 参考信息 -->