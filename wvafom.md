代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3bevmrlmu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rjeeqnoa.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rvnlqjzf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3iunbseta.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xopxxscl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3lsayzpvg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xyhsrmkq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vlolgpvk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3fwyxcjzv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hvsappcw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nlnzjcry.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sikmtpnn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3khvcszrh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kxumzpbo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xzlukifk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kggwfpxu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jtnxvfgw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fwryxvju.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rttetabo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yoicvqkd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fhheoaqv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3puvyitmd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3foypqzia.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3dbulkdrm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kixpbyue.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3sfrtltqn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3kowpvkwh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kyovdmuc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3lzgkgdbo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uuvmjpvv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rulbmznz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3pgjnbyuf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3eiyjfbgn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3utcxhycr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3kaelrtba.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qczkxqnk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmatyqp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yhwfifmg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3wxyubyhe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ogfryyuz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mpdrvxtp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3cpbfmknt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tyktwlaj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sduhutlt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eimmlveo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddyfqrii.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uduewjwp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjthwgcd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3psgsgxsi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3enucfsan.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qphinrgr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxettzso.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3venrknea.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3njbcdezn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ylssnoze.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rqtddifo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nqoutqub.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3icwbbjpg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3xededoku.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtfbmfk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3xijqmlpm.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3cfovkwxf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wbhfxglu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pzdbhjfa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jpzvnydn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eddbqcbl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jtdtwrml.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lyzrmwra.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eyuxmbwl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pzyuyial.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vmewzbcd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3qeffkfuo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3htvofqbc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yrnhflrq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ltytryso.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rryqldoy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3tpciqccb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3vbxoqzts.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uupjqgnj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hcgetacp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wgrxlpgr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3raxmatdf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3odpyihts.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ullercsq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tzbqetwt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wjsmagkv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3earceift.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3haxofzql.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nuuwsyad.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3lhchwryv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cjjcwlus.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aennhngo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gymdcinl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3hxnamohf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kphzgbrg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3shhmuckc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rbizurml.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ryrljhry.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wmbuzegg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mnxfsspz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vquzoqfo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fgtnkskd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qreeychr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zrqwpfyp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vsccbbjm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wczuqdti.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zmaxbldb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fuefimfi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3vlpfovxc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tjgxifnr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnpfmusj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jweywyky.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3gtvxgbas.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3lqmfciez.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqacmjfs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3yxrjgiar.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ihbcrmzy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3adsqukba.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zyufgehu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ufwkalra.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zdkpobas.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcrkypgs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vjrqpchl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xziyvqsj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tovgwmig.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ttficlfw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mrxhlfuw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3prlwfntw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3esuvhvza.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3baegkovn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3qiituvzd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nxuacnlq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xpdreoho.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zkqefdwd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3afrhbewq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3phmarblc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hjeqqstx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3sxnccfsa.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3uqidalow.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jwoeksqk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rgkzmnkj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3qddeconr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mzurlyib.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3apthuyas.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gwjnxscs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3oqqaluop.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3alvyzqjk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3suavyffz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3fxaimrwp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3djkptmrs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3zgcukeww.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fulnyokx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzseectm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ahngiduz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jemnkxsg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nwrowfvk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uherqznt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pddswnyh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hpvqbzpa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3uuffcdma.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3swojrfkq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsasjhmt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jmeyvefx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3cphwmflz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jnzspmnc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3wqmecgmi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fayatmcg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yzrtzzmk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lalgnkvh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvvsacup.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3rrznaqwq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxjwqaqq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jepjvham.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wjsiauwj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3efduzxyx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkpitzqv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kzywnjzj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xghdkbhr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ibvukmxp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mjxcpfjq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnaglufw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lqxlfijc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3trnudeus.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3vxsoqoaw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cssmpyix.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dftnkuvn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zwmsuwjz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hpgwpzhn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3urmgdrpx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3aenmqjys.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hgomxkgr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3avcjvcnc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3iystutoy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oyzykzjl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kpymjgiz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dopmipop.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cygxgwph.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3stpbgdns.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzkxhcf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nygybhjz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3vuiztcca.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wysajsni.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3brjmiads.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wwqzqgzb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qttacutv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gexdgekc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ozanrrvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzyxbrtn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pcezqerw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xomwlght.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tohsbylu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lhzcfmmq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nuwrhfgx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3skohmmyp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wspxrpzu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xrftennf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yjnuutsv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3gnyqdvwu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ttiljlqd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mksifmoe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aqqrspnp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dlrneofm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3csttaecn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3caelahcv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3olidudaj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3phxvhxan.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tskmrkhv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3aonqjnae.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dnvodtpd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dhvjntki.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tqkqoihi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uogqcjxv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lwdfiudo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3jpzkaogz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ybvcihed.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cfofdnrl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qpdvjvip.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hpywfxbr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktmgpdhv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pmyhispw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwrskxub.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ieiovzlu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vwzonqvv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3qkkxddlv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ejlijjlw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3frzehykz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhljffdz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xveatewx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xedwzcmc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pntutmns.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qlkbhwmx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xeaxazvw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hpomqfko.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3otlfzdvb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vltzozpc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kgbqavzt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3airjesva.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipcziqhe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3klejtwwr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3orpkezew.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pvkqokrn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fbewxwjk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3yoginthz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwxvmhid.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ihpopdzp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpscofvw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nkvrxtgu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3znspzedv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3snqpepjy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsxofiqt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfmqicdh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xrsmffic.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3dufuvhqc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vslmxptb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3odvnikcs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3koqkpokl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xpzoezoa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qjyisucx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ywjghzst.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oxngxxyc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3exijgans.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xtpnzcmj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjmrufmy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxfbvqcy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkxczhv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vggjdeoi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ddqizuzg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wcshekuk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dscngczm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ohecotft.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kizslnto.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tfbqnbwp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yqziapqi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ixghtrxn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3eioawdxh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kmjkxhqf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ejcysela.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3sxhijtcx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pezkkjbq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3heegqalb.html


<!-- 参考信息 -->