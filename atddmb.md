代发 wailian999

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cmcgtnbi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ldjtnzca.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3lxoexwep.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3bkazspip.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qemoaxii.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3deugfkzj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uvqbopoo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hwjmajcm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3zzkrdlmg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jurhjszb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3liuofpul.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3leoszqft.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3uuyyqnmk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlwazxye.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pqkphpkb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3akffhjse.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3evcgokzm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pbvlyrcf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jglmkrkm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wwnuslsr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tunztljk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qpyzxtox.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ggaxfazt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kiuehfad.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rgnhkhwz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3khlzbcvn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3wwjsndfl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wdpsfvkz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qtladasj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3znuedgyc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nqeaxbgg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vgdwgvxd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jlzlzwgj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tmggyumk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pqghumpm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3gcguvwrj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gztpmagx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3pouusiel.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ampjnvft.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tpddglvb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlinruuf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mbkyzrwd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3shxgzsxo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xpekfijb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dmvppnjh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hghldkwi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pwazrilu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nbjqviar.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxantpb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jpukcdst.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3peodaahp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yvzkyaps.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqsxnis.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3enqqtemm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zwuurwuu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtjlhnk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3csygtvkx.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3osojpisa.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3zpvkndjw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tupxydmy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dmeicisn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kklnyguw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3lekgzjzt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtpbycw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qghukbgg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3sdmowrwm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3yyjlywxf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eaccywdx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yrusqyrn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hwqaybcd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xrfbzuat.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dzhjwjog.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gnzyfvxe.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rzrxynkf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fiqciqgp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3wiuwwzmd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qnvnnqeh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3delarhhn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fqncktyg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3uhtezgik.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xazajruv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tukmdevo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3owsdvzyp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3crcndjsg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oodocxkw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pwddkawa.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3phretzmu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3htlxfcmj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jawoaabu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zxhvvoua.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oxkcnexk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uqfcmuzy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nbobsvpy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3naunntjy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qwjdneuu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jfisukhr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qdprpxzr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vrjrzogw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qdhicnle.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nlxzzjvn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3smfulvfm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3bgsuikxg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3anaetmgl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jekikijm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3awhfyqew.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3avzficdc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ekmqzzsn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3jrodyuax.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rdqgnisx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eeclbowp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3xefnntdg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3toljyhxt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3xaidtxod.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3nqbhdhph.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvogbouc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxtlityl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3tfugqeuk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pfmztfaw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwiaikqo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3aemwvjvx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hqhkuilk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3livrhdda.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yhbnukfp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3urvqnlwa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zphakkgr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzackfjo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fomdhrxo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3korxqqhj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3mbdmqhwk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wfzvjokp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wedujfxk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3oznrxpwr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3nebdefru.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dsbjalam.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hnmchusa.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3thrinuqq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jussxxyz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ptvkwpot.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hdrzppic.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gauxxiol.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3shoyddwu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lafzhckv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3tbxaoryf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wriksyuw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yfnkztna.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uqwmikem.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ubvniilv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3bpuokshg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xgztegqx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3sjmpfmbu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3crfiomgo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jcvwnmwz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3cujmwast.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3tngaljxt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3sggaklsf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yvsgsfyz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwazyhec.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3unagozgl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkoyfiae.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vqaipkts.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xzpotilh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3evkxbrus.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zpmobads.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3husbiruu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3glxuyogb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jdkvhgut.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3twkqhhns.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ssvakgak.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3measibwo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lxywuavo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3yrhwfzoc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fjiqaeml.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lxshpovi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3skdxxrei.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dbfvrtpf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3orfoltri.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xlgcsgoh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fepnlftr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3brwdfnki.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3earlqocn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3szpcbkgk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3oamuyopr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ljvallps.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ilbazakk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejhvvnad.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bhxbskul.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3agygveym.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3rdgyzkvy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nepbtzri.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fvgeflgi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qbdvavrv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3heyifczg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jvhuravn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqqxgdi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkrshjb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcrhrsxa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmscpvrf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uzjishjq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fqdzvmbs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmoxxwfl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3soteheis.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nnndxymi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3iwkgvwbv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xmzhsdns.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gvwnfhkn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kcqdtpah.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3lhxhvjpj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3kgukfleh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ygwfzsqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heosgthy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3yiclkmye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymowcpyy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hkvmwrsu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3szjjbvym.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tvdhumfq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nbomdawd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yvxzcotr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zarwqbzg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ertccfzx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3djefpfws.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3agvaauye.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3uiqsjxrc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3iwhsilin.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cogsnrne.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bhpeldok.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kawjutvv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3omnfjupi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ieetoyxr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hmkgvmif.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ubanmzro.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3neyeltft.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cwpvnzlq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmfnholz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zarrcjkh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3namymtpe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaigdsxu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tdvxanyo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fdoycozk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cwaerkhc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pvicsbcz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xlubmayb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ziuqrxwo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jrmznozr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cghcbojl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxxuuobj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3whkiuamo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ljndqnqg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxivizdj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nmolwikl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rvvqwjhk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmqyxokr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcoufrfg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iakwltzp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dwkucanw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mrzbcywp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nbeaxoot.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3chwgqphr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nwtzjzyc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fjzejdju.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqbyjoa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxqikyr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzkefwtl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwsogqdo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3joxmbohr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3uwxdmvcw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mwmbybfx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wpafgggi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jgljnawj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpvtoauv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwrkvdv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dcramhcn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgoyzoug.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qizrccrn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmuwipqd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pjycsgdo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ezjrltiu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qxjbqslq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dclwhtfh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mwnqkdwv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zyfamblm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3enznyclz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzhvjkti.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3pmdtgohh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qksmrzzt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3oulsdvbm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wxzfjsoo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyjrknwt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hnvuszbe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wunmvcvd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbpfjin.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lrrlizqa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zdyshwps.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbfwcamz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wpxwvbdp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bgoibgjx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iggzpcon.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xdimigtp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3aypxuinx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3myxwilzz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nlfhnysf.html


<!-- 参考信息 -->