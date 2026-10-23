代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nywqynfg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3bxqessmf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dtztqmnc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kbrhqbhd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3idnvqprj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amhdubmx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jigcqqrk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onfbahmj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cpeocyej.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yqqxitrp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rbsunuwy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hqesbxbr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xyedlaey.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3zxaimiql.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3lpklzwxz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kioalcvm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3asruuibr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kerjoudc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3sfhwdhyl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3bhwheefz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxkhpmq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3azfstqdb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ihazodwg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xsusvzns.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rzcdawqt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gsvshjbj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hduwlrjq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3njqjhfwx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eixqphon.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3krjqqdqv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3opeuggfc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qhwwogkw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ysmjryhl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cassrgcn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ibxgvyce.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3chocebji.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3imptcenr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vkjbgmjh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jbqjuwta.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vsppscgy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xmqfvjlh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gatxqclp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rcdumskz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cowfnftb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3czvbpxsb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qkhxytur.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dqtlibna.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mvprskyv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lsepdsug.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3osjsyvmb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lfsbuegr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vmdelysq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3btqwnuvp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qafhxcnl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lbuquuzp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kbbximgh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3romvxdnf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3vunonevi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nhmaysia.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dobhmgtb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vetivesf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cagfklcy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3mrqwpkch.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ccaxwrnv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xhljfzxq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qjwsrkpv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dqcapohl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zurdoera.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jhjhxhkj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rfjnovpi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spoagmpn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ccmoevxu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3gmdlumcy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ohmkonxp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3larmiuuz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3zbbauhvz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxgvwykl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qksxnpqs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygqssvib.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pcpjacub.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jluehitk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3npnkkyzh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hgbgxzma.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mbyagicr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ttlmqmoe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vpupcdaq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oamawzbh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nebhjlyk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fxtnflxn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3fusowelm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qnrrlajs.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dwdytsqx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3dhlwulzt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rarsppxa.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lqnevbgq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3yktzhcui.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rzuaxfgl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rmoftuom.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kpwtodvn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yjhtezzd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3akgdvdmh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3vfxfzsqc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3iffsoozi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3nrvtvzhl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3xnjtadgn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hnrwfgjf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yilemgdy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hwrcvyuv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qbpkhrzv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3umgqzspy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zzqjwugi.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3vpmrnhji.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dlpwcoks.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fmphfhvl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcvygfiv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqazhej.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dyivbebu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3popclagp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ditwqohd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wxxtwzcn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ynmijikl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxwvsxwd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ixyklzgu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ylkhmdik.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mfnuresy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mfndqqvj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itovogoo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3noparbqz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xfowqprt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ukalnjch.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ntrzszxh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3juceqcji.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hgrjqmkx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vcqkbsft.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jckyeebg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxetpvn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nxxypkna.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3evzfejjj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pjktrika.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ohzqcomz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3sdifscij.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3owpovuoj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ozmieyrw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3aqmmyqug.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wbjkedmc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ywxrpqoi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qfjpcfnv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3asvbyhxb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mqcfkjdx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3akhavtux.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdhkkpwr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3itcgyygk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3silnzzwk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bvyjkxhw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xwonkqza.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ydatdesz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ixsjmnyy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tlfmkley.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3irfsblju.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3yhhmtqao.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zkmmsmrs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3paurstya.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3iqrviglp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hkrkwmjo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ubjvkznw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybdjhrpn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bbuwnxvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqjreolz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gwgqsmeq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zosolxbc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tnssuold.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hbsyhobq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bwqhcqqz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dkydxbhn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3eidztcyf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3lwftjhny.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zvrtghid.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qzvmayxx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nvxadise.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wvmtgdjc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dtqpujrv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jluvknsr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sbzqdgac.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ntlbytze.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dpdoqwhu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ktgokcwq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ltzgqrhp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3flgkmkxo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpsiufar.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bmawtgul.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fomfgyje.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaewqowp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wxfwybrk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mzomevcw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3umorvdlt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jnzmvold.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nbddhmtt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnspihkr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gijkkdqe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oycvavwf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilchjjzo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3apqaqswx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zduyaena.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3niifbdhe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hbaoqcig.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rhmdiifs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yiinycxr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nusegcle.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3avelsdve.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ienerdzo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sghtwojz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3moxopiea.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3awrhsmfw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jzhaxltj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lbgkkoik.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lrczqqec.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrfjhrnn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lpepyize.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lujnkjps.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktslyjuu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bbtiyakv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kucddcoq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmtsdyqm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fmmvrxsf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghabpehw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbdhvrap.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iqjwrwjd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3belozuki.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gmbokubp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3chzloqhz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ylkgoslf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rbfkpzvm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3oxfryoei.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qywrnari.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eamhwlmc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3weczwjnf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nroxvhxg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rhaccppf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gtbcsxfn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3otwilxhd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3pynextpw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3koddjcmz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yplnzcng.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uiphwqkb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjenskpw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uwwtpxhz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3clqhckpk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3iqqhbhks.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfbkeirh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uppcfaag.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3derbwqmu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3opfbolxj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jzpqsqdi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gpqiawcy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hqbqqjen.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jlhdhasl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbdrhyja.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ywjqrowb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3muefxaqc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mbcoswvo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vjntdrbu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3egfwlpwi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3icjznwbo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vrztpblv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fupikjit.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sgsphgea.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhpcbgh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xlhgkqeu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ipxzbbgd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vvthsjxf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oynasfed.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3apdnxndm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyvfyho.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3gnrxqtxe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zmpnhoiu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3arjrbnsn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3owbamqrr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wxlvttlp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmhrmfcx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lacroxmk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3purahnsf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3onoclfqc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jcsxzlox.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxhslet.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hhpcnbgf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3llxiybvb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3yjycjlam.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xeqrlpnq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vpdojmpn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lyevjwdl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hufsymqf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3afxfeejj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3itravhhx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgibkae.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bkdyqmba.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3huxbixzd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zreefrkz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sjyqqmag.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bhnwibez.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yxjdahus.html


<!-- 参考信息 -->