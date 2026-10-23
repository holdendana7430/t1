代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vsqzylhh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bpbsodoj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qpmgchmk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3yifhocxd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxqxcyis.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ntazqopf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3krmdogpv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3vjkjfeaw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3uavwfkgt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yynewava.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3akqprfco.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3uowebbdc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3nhejaztr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yvpzoyol.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xlnznwrf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mfwqjstn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xjhhliug.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yvqohjuk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3raooravp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zhugpijn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gbxcxscp.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oeeubhtj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xurtozke.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jahubwcx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ajvbrkjr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bunpkdrh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmwrjbo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3okenizhr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vinzbtao.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3evwdscxh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3sajrdauf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3hrdcsrue.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3mkpfuyxp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rwlelhkz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3miepvwut.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tkxfmdge.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3eoklpwnl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tvxztcws.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3uuorflyl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zkbgiuwi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmoxbjy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nnjanjqf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cgxskljr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3thihaqmq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmfghyh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3onxzfxad.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zsyomsks.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bevsiyaj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qtzbiite.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghfnstho.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzjoypwt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kdrtwmza.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogokpbbv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3cysomkuh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3grfusewa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qworhqdb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zbmluvkz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3insmxrxn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3kzarerji.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jsuwskye.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bihqrhxj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bulwsnuy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3loxneyfm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ahremxyr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gljwsvmk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3nigedlaa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ezwovaxh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3awxyakba.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sldrtiqd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vyuzzdzf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vqljpeuc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3kifhqvsp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ulxjpwdb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tnfbvgsw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ejpohssv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3xojxoulk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3unbgganh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dyohvqjs.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vdftjxbq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3btkxhpzh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gzhdtvpf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3snfqgssj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cervetbn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jyjixyrj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zppwpqiz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cbjzzhms.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hyhheysv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oqhgtzrg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3soelluiu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rhtglqtd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jcsqrfqa.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bdsihbwz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zxyxmgim.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3kdwyggbx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qoivgclr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fclnkjcl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mqbuceav.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xtixbwef.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nlqauldw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jjmnzjed.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qcksxzzq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mpyatpaw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tascbxbt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hahsdore.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lpctnnof.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lssfsdjp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gxujqlzr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvcpdrt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tzqdedss.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3knxbopbq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3iielhfxm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3pynvghvw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3oiujcnlf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xbcfqzre.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vwqyksmn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqrrpvyh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3mskzvuae.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vjwyhrlo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3euwoeyma.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3gbkslzvu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gbbtcjgw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3toxqkzsa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jorajost.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvdvrmwp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rdollehq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kxumihmk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gkygcbdr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rqprszlz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3pibgbzwg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3erbmkfzn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ryhrtbfc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ycyhxdsi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yjeuqjgz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3rkaccqjs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jmcefduy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fredbnoj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cazzkoat.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3azuyubfo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xsxxmbkw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3jhodpdef.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cydfrpem.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ajvhfjrx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ikaohvqb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zkwiwsxc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ebsltlzh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3yymhaclw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3phqfdhlg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3pjjxtufr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hanbjkgx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3frncpuxo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3kbqqveux.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bnsytfuw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxftspb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tqmdsuto.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3izsuxmmz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3jgxhxida.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dxwifikj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vchxldfx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dbzkrfvr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3autrysmg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xklnbdri.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dtzctttt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wjkabxjq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3wlylbwfe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqamznhb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3rlfngqfh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vnqszaad.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jegrwnqe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ojalmnog.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kaadehrp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzeyvoz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kxtwbdsg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3tevjwbxl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lyxivpps.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mevllydl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ifpwngos.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xdbycczq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kvngclab.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tcvebkac.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uswywqfb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3meutawqw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3fomdnusf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3iqidagdt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kukhuvhf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppyfefjg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yixsupqs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rtqyyeew.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dqpxcvif.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdirgwky.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3shsrfhow.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kxmvnppl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kjtgbdig.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3puqsubbz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3kdnpldds.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aakzkedl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3afofvyld.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3iobekktv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3loozbrfh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ankthudp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pajjpzqv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3uctrnoit.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mbhqqklp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3kqoxmhpr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ocizazlm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rlhwydql.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zzsafeqe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3sujoflzp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vwjarogc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqkvlgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnecbnnp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3uaowqvpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3burqtsrb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mxpkezmo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fysujitw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3kzcczziv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wofvquiv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uhqhzjml.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rbeghyky.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mpedqfmw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zqizznqu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tezjtyyl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cazkffuz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lsarksyu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apvaadia.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jdpnuncb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sykyujhc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fcwodnun.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wvqiuvfm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3emjfvtys.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3amykrwib.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mearnjuj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3mpdyktrq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ahxiiguf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbytimnj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gdnljxjk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fykdcdyy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hopxcieg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tpritqzm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dbfmloio.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qztwqmhx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3aemueamq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3brgiyipz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lajyygig.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kctrtfxr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3exojfbit.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wsxbwsiz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zdiotbuv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fenstkoc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eepvhrub.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rnxmkvwh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gvwlaldk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dzdpqyqx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3siihljll.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3usoxmhlg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tegqfnax.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3utddjqds.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3suometks.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zuvfrmoq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xivdgtuq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3cqxobsft.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3knqzmwza.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3obfhomfq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jzkxtlyo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gatgsxpp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ylpwthzb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3oqfscazx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvkwgtlo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dhbvnmtz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyaxnkfr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vqzumkmu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3obejwomy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vudhosnt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pbktqtam.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qcnlzesk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaakbqyh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mdtrgtup.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wkgbgwvs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yjofmcuw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3clhrqzdu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tbpzhbtl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jckgthud.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3frzlefmy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dbxasawg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3payzvhtj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yyijrajg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ullpyzpy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3awwbkloc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sktkoeim.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lnjupvtg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mqnkpono.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ebntpuka.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pohnnjdl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3thgyzxzl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3twobdxkf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ktvryzxw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pznnnmsl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pkpmlxqt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gsghqwui.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3frmhupct.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bejndbry.html


<!-- 参考信息 -->