代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qhdgvjhc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3isinarqn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3utieznpd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vanfzkbg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wqqwstqa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ssnsorbg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xhfiqlsv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbdddgw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kxxwfmuh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kguyqdki.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ymejylps.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3evzddknr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xqggvgtp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3avzzxucz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pkobcpze.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ilanyygr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jwzwiooo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lyoqmkae.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3scjqiacn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mdlkxttd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndeicnmj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkwbzbpp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aygwalte.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ctlsytcm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ciesdpnb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3qprmidbi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3wwwinmct.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3obxynfxz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xjfkcxwz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3skoiuqwt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3tizhycuz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tvcofhxy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3krfockxj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3btshnqka.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3gixwqmgw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mqzqiaok.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3iinjnbeo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3thutvnzg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tarkbrzn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kbcnibtc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3npknswgk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3grutsbyk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rrezzswb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ygzdiukn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tipzcufa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nqqyqwjw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hstrcrjd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3lplskvyn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lsxoleen.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dgevoman.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hkowavwv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ezyrpmqs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtfstog.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3koahpjat.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3drcmejdm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3tmjtlnji.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pkkcgfvp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eziclbjk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ikahgail.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uplvrakj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3udurzgyc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hfcytjla.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gubraskj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tzfljpkh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fdtyvqai.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3yaxdbpxm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jsdomvrc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wqasxcow.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nsqtucsh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vbhafqbi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vhrzbeza.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3eqagxhtl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ykzqspxy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3afzixzav.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mtynmcwq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3stcaprtt.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gpxmjhfs.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ishkfqwg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3xqaonqbr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3alnmdglj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gbiupnzi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lyjaflmr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xadfscub.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zqsupqjq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3flkjeihm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lltqrbgz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hkdcgpny.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whkyfrnb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ldyafzkf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3luswgigz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wdsljovn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ybmirhrh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mpvmgcyf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cesdwnjy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yfejkcmk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ijnpckcx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nxhmfarn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wmqyagrk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3axdgtuxb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qgnwajzs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3haeqrmgj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zllnvoin.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xlciqzmf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbfaftd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jkkwoumw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3jdvfrrac.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3nwoabkey.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3gahntxsr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jrcaabsq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tmrwmfpl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ddtvugwc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mlhsomqq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kqtbdjys.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3brfmwydc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3npwufalf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3obktnetu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3faedmapp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3sufdvpuo.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rfcflhni.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xmgialgi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3tvauunvy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hyezqspp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3klexrqvq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3zcgwibem.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vxujxdpn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3sqeuroki.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3psmlsahh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3cupxhtau.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3hwprasaz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nwwdbemy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3prygbnoz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tffyejyg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxwyeym.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvodhwq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3auuusond.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wcykjggc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3shiqxnqo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zekeeqjo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3etrpmpib.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xindwlrg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qgqyuylb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zhuadqpc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3irccesvc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wvdpittm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hziyrdcd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vjytzbel.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3henajjms.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjrpldq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bhxyhjvq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yyixgcog.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wloiwevo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yvgvlifs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gahijxmz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zztiqjhe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zvqyiitc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hmvdqgrm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdbhinmc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gjpydwev.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aaglmavm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3omltdsuk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bneditnp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nhvgrrub.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3imjaciav.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kvzbhpuh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3tjbechps.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuodkbnp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgzjuwe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3urmmidqv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vfxojtnq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hlyvfcnh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jsxscxjw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3orledvzu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vkmpjqvf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qeqbesyi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fcyjuhuv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3mlorvjlw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3oootufop.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rtoqkbok.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3pyksapin.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rawqzyli.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3opvuhvzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcgyvjfx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ksggebxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edmipnsj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3fxxuzubt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wczwafqf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3crponexn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zbkfnzyv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3axuyjgew.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sojiczwt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rgujscbm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gdccpgkx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3whqpemwe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3teartsnt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bxxiqtsx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdqujym.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3thxflaaj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wnfjdtpb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ijibodri.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ykeozmfu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3uszjkjdl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vbzlvwzd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zudrmait.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3sqhhfqrs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3swsfzipe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btrvsqdv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zqcivzuu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vclvwctm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dypwtbhw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3griwsjxy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xqfsfvli.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xjzvftgu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbnqhvk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qykozwip.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3egqfyrrb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cufvvhgm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jmghfend.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ssssrsdg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rizqlebz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hbucbkie.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nafeivih.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3omhgchmh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3awldcczm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zyczbold.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbetsrek.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lpntetht.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rdnhvfol.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3namdljac.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylffvsmq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ozurrsue.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjrkrzi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mpqbducc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fiygiaam.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3odigvbub.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3khnlossg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3spyynvwu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kqxqgpia.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sbdlrqcz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xdflhovm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bobuccbo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lowrqcqm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhqjgntk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzkurdwk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oagtjufm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3srukrmxd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yncmgaag.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rntxxauk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3idkutpeg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gkwgwopv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3moaytddt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qpuzkfto.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jqormttj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mmwoaihs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nzvwrgxv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dzxmygit.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pnngfhwo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3opbnizhf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vebukkip.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfalygm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rjsevikj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xezadhyd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwysobgx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rbfzduve.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mrqphgws.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cpgxutfs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hcsrodnh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ieobnczy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryqfuxpc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rwexkhtc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ocpnvrch.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3likhbtcq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ordjbdca.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vlobijtf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wqxxmuws.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3shtjvxic.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rblqfmis.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dcztlepn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uhacqxgj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wjkxfgty.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ajrjmxcl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jyghvzks.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kqmpoopk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lxwkiacr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3drnxrxah.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3exxujsle.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cmkwvnmh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3stfgrqer.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gqomzzls.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3balntbfm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kqospqvd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ntiurzrm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mrrggsmi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ujdzcatx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3quzlhqxj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3huavzmfc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjflhiby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lvbvrqul.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hxcabynp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fvqepnzi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3eptxhwgl.html


<!-- 参考信息 -->