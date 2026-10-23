代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ufvohkai.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hnllvgnf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3onmkwsrt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3etgxblhq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fswgyjfg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jpnqappz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3kbxjrfkf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fppcjprp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3zzvpzkvc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tvswoxyl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sivnvwrn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tuldgcvw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3udtbzggr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mggcijct.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qjzkdjbk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rgtmixav.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3veaeikwp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mwwpkxfm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jrblhnal.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yoiyolnc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kwdgofbn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3avljxbsi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qwttnsue.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xncxyepo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kvinscyx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ukaopsua.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jljfmcsz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3pxcodfqp.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eotgesso.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kuxscmdh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vobaohem.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zqmmircz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3pvcujgtb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3spozreej.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3owhomekw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gyjbcwyg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lglqyjre.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3adhbraaw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3sfleipbs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hbzymvya.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dwflupzy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lritlexi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xoyypkwi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3braztmnp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iluvxgog.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wiucrqxz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlsrlced.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wojfeaau.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pwwrkihr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3snslayeh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3kbniuqep.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3azvvkayt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kxcbnvku.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcqvhyz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3xfngybuy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3skexpygv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3joibickn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3avreabgx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jpmapfxn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3scvrvwly.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ecjajduz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3qxpkummu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rrcwypys.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sbawgons.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ixvljakq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fvhbommp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cpplwycg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3hmtqiapv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3parhtskn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3poyxkmrf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ntuscbhv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ithadeka.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lsemdieh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wpaggavi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kkfxdrtk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ebushyhs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dqumiolh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wunueaht.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ruouaicp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3tpzbxneu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3euswpyti.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fkwycluo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gzbnntmi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ivqtolfb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qjawctnu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ecmhreie.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kmvhwitj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbathlmq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3aevwwsvb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3tsyvaeak.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zljarkxx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lmtzmvmw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xavtaswl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zxfdaogk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wktgpgrj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ifdmxylb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fhlzpunx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rxildljk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wqgyzihy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mhztjmtv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oktzeqhj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3krhpfvhx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3pfltbrfu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xpxpjtmq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rtbabocg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ohcgyqzh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dfhrjaso.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ggvkehql.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3apmsatfs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3hopszucy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rvldpdpr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvzldpvu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3fngljpxu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3veweblel.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lqaitean.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qmgbggwv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3onhpzpiu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixewxphb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nvegmiom.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yaykchaz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3imrifvga.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nxjkmyfm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oncbffkb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vuziqosl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tdeilbwd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nxhziavu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sqeazgdz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kvqrfenn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lcvmpjsq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3wprvhfah.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3nwkqitvc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3oszrkqij.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nkiggwhn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3stybashp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ryxsacqi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3gpasfqlc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qclbgkcw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3snqaulqx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kbgikqhk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3njllrmrt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3errzhjem.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rmkpleke.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qpdlxdqm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ioqkfitr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hsungwak.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mkcbxykc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tppkcgrx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qwguurhh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vfcximmq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qxqiabda.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pefyhfnc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3wnrfwkzh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3dmgohpjx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tmglojxp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ncorbtmp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jujcfoeu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qqijzacu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gqywkatd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3enybmdlx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jkahdyaf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tbeogbec.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrgxaoe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3pnitjtqk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rhwklxlx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jnufqzzs.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3emngsuho.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gkyiejjj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3nrvpyxyx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3eguqynew.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ftzwxugd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3idkejxzc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ilxvmhyf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3duheishd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tljqrjcy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lfmzusep.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3izmwzqys.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pmmxsucm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qdfhfelf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gqwladrk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3dowjybaf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3giybpohv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gebuutvf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mqgwtagg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dojyhmfo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkddnjvt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3otlwvtbl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pdlutwar.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zlbumfye.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fdfjncmv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fuoijjlu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tuqespiw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3opyoatlt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pjuwtymr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyeedvg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3uvatvaha.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zqxwvwzy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jcyhvlrm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3bkazfgoz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dtehgaum.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xaihwslm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wesyamxp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uhkyovjj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3gdowtszq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gvztbqho.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kdftvfsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epxpoeab.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3srhlcahd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lstctqyu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hahdfkgy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ylckdeyv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lruzarjd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bumokoii.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vjfrwbtc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aymdrngq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ifkraixb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3alfmimhg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3smbsvvoj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zzbjwvuj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ayguwqzc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otfnlkzd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hvsunewx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bhzwheaz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3etpdjooi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3goascplw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fsdkhhiv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kcqqgesx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3evwlmzcf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ewaubngo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjzvzlum.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjldwygd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fztjzhlw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wlebjrao.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3piythfyu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rhdckups.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3stssmeot.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mpzzupgo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hagltkcb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lddigxwl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3utuemgok.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpggxjtx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3bzfuevbs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zxhbkizx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qmxakopx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmxphhmd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3glpqqxnw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3clatrwgf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhbkgujr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3icmpziwi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtrlgkrf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gnnsphot.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3suyyedjz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qfhguggt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zwudvmxz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kwavqdpu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dmsbkaam.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbybihbn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3swhrtbiv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmpudgdj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuoztycy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jabiounb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3okkxvbow.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztaxvakk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pwrkpiet.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fpvbfnpv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlujewhb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rundkqyl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsrcxnau.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3isrouswm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gfgjgxhn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fpnyiicx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uasurcdh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jaqhlriw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3tmjrgvoa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dnxcmmzd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vrzenwpy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3weysddgb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yoarrhwx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bsikspyv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qccgxrle.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3syoaidzm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zrcrqbpe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nyswxwvg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxyrfhui.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rnzgbrka.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xdjbbqke.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mombzrov.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wvyvczob.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ezmrgfac.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yxrfsphv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hykdzhpr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3pfiqzfqo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gsurbrcx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xqnpycxt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3avbhngxd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrklnmfd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jprqngxd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezfcesqq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vvqfyycl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vodqibhv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wnufkxfz.html


<!-- 参考信息 -->