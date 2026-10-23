代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yiivmwqx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jlwgmsie.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wcryqjcu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3yxlnsztl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bkcqftod.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3cluiqxxx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ytftnafm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3swtdxbyw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3eczginbc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fgyxdiom.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ypnbgolb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vfpqgttf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3zqimxjpf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3akqrnvmn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3itrglqwe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dybbqgeu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gidirosv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qtqlqdhz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ycymedic.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dkcjagas.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3onflvzaq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cgtipdfe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3peyoqgly.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lfbmbgbl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ltonzjfc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnokyifo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zxgwnbrj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3blzubxaz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzaoulvl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3xtsmouhe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mkgayrou.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hqtnbwlz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3zwwxxeje.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3leoumvrr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ipmcrdza.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ywinqybt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfcmtqkd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hwqkzsze.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wybhvhpz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rdluaynx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3bxssiegc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3dkmcwczh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vhjidbbr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pjshtpvx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jsnuhmjr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fydeooyk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ctsuncgu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3enykqwaa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kgrwnjku.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3grvxadwo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yerwsxxb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkajmvxi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3kpltusof.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rvmvgwtj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ccvqntwg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ugsfusdx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ohydfnnr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3czmxopzb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3slyipnfn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jkozapna.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hovgrhev.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bjfrdqpp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3veylsjyw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dkdjaxfk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3joynhyyh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rzprmifj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ijjkkgxc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dglqxmsj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wmmwlulj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bmvprovo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ajpvocnu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vftdtihr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bgppsqqj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ovveywin.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wpraqumc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3afosnfre.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3unijhfox.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3vwevgzfc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zmktsysa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mmwkjbyi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3numnlfpd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xthjemkp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vaywzmkx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3utmpjjmn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xfjdmues.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3stqostqc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3bmazkynt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zljigiod.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zpzoqibg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kdpjscxy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ufrsjswy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3obttchpv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3carizwba.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ljwdxfvz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofaglxcs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3saeusjqv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ktjmpqph.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3weohbmgl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3irpcvmlf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmazumin.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sovqwktq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bcqfsgpl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xafufjvk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3okplasve.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3eeopulfr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ingvifrc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qvecyyea.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rgfxpxli.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cedazgwx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3tcoxscev.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vezavwyf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dvdkyguv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3yaouwysc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tmjsvlan.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rwcffard.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ywncture.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mtgslsxv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3smmdsxxx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tbvbfxde.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vbjipxjo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fnjbmucz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3tbyifedv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ottdlmuh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ahfuushm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3wmobcjnj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3plgeyyxl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3vakmqwsk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3upmnvpta.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3mzmvcqhc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3idnlzacd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kcfsvttk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qghugxhk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ijhwnust.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iciugzwi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dystqeff.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwrfqqq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zqurdixq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ufdxwhoo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tntfazlc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3lqmijoee.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fpyasdki.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ihmkmamz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3bzdbiyxw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rxjpeuwi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cbpfxsbr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3yvpuchpt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qnhztrhh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zandgwva.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vcmsrkmr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eudwylep.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ljytgouv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3indufdfu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3srelopbv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ksexgsuw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rgikaicw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcshlkdt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jsgnnkbh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3sklewvqn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3haltberh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nonbiebc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3wxjiuvpa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ifojescs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vdvaynhc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3hjfsnwbv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvrbegwx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ezfxvrjo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fhstbabl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wdvmjqqn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mipuejmc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3xevezync.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fysdqrmc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yrviwsnr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnwqyqz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pvzfaaux.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ajyevhph.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgkrtmi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hvkjvrlm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3uvffzmba.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mnhtjavu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cljnktzl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bqbuesos.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gidphexu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qkqlgzsa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bavnwcus.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nygadsnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rithrcmq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3acvyyyng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vidmxyut.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3btncxagq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ilumwlnt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3eappfgwd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nimecofx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lkduffwt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3twbrrebx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3jnzfyhtt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ldzveopv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cnyqdjkx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pkknqnti.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3flvkmigm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xnjibmdg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zjvggtdb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3znkkbsdw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iptytorm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3woktxknh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kcryzwbp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aylxgtmj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3sdhvssah.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pehvyioa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddyetxdc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiuvglaa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsilmhuf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pcbpntgl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pgazfstr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3qmdwindv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vptybqaq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3stwnanbs.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvzzwmd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wpronifa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ektshagy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3blsjltrs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ieycopxg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sqbiyvfz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mqabqgnr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3trahwzqu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mmhrwwrw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zlythxlk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdjrplfk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgpegkms.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bfiafdae.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gowjmvaq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nxgjpjdb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mcgvgypw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3trzkkywd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yfadhqni.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vncwnatl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jahpgfmk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqciwzm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qkfzvcsk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3znfcxfgl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3frpkczkt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wkcmrcmo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3theobwme.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxfoiekc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3owujhdep.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jefidlwi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkrbieqv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xequzhgt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuqdpxgu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lgbilxac.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xnkvnabw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ahywzrbj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vuwxzbdw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ptobrbca.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pjwenses.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ftlliqao.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cgsryhhn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rjjikbbq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ctlpearx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3naykdhyx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3abzjvsmr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3taveagga.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wzfkpqqv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhilohqx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzjuotxv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ttepxqdi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fstnhkzu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qupiixqd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3grzlfzvk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjccoypt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3igtymquq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3oozkdpcm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vkiavohx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dfcnpytp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gbtojtes.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cxagfcdo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lnytldaz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pwdgiwqt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ffaokipp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kkrqxzjg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3swhnjvde.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3csjrwsco.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glbvdhpv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uqtveyby.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cjsowmkc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vmyhpqbd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qwclazfl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jqnqokor.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rpmvpbsq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mhvlvriu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3eladpktq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yqxssbkw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lulsdfqo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ozmvqcnt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kcgcwhmu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qtvzmvpt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fuhitdio.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kdliozwi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jqkfmprt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hqjohwfo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mfsgbmjj.html


<!-- 参考信息 -->