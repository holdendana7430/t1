代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3amslvgmw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pyaspgye.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vpdzgojw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tstncvbu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xndxoggv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3hhscqqoq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3vtlbkrcj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rhwslenb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbvlyuhr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sipnyfcm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gidtcbqv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sksbrjex.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3koyyerrk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3wvuyjtus.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kikaiffr.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3brtdnbha.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cveufpym.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nqapgcsh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wmaxrgzk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqitarpc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dgotvcox.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ywyrptlw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3brcjpbbu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3talgzzeh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3oisckffo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tbvsipuq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3zwmwldkh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3suhcmpgp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3eqnyfsdo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3owuphybf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mfzwnomh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3sicjkhay.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gpbvghck.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3pkbznltu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3knbumlgy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qtrbcrkl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3snhktxru.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3okfvmjih.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pxklezfj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hqppjsji.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rawvouss.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3liggodhv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ugcgiqrk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3eohicsbq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3etuutqzx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3napuoofl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3slxoeqrm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmstcln.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gpejmeyv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bcrkgtfn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3cvkcvyjo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3lpzwdjoo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tkjufkwe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3afagesxi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cizdytiu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3okksahbm.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mevaqlyd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zulikdaa.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lvxkyrit.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lkttgkrm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3oaffsaoq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3eiazxrzf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3joyjpnkc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3piedlzwt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vnzdunku.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lmhiedve.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lcohayuu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3pdxbigpu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oupbmuzq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cuscfzdw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uvyttlxz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yarccxiy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wflmtapb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3iwgtopuz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ohlucpoq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3lowbqgbw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dftgpkve.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xsyihliv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3durahbvt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3iuoaznxx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3keytzixr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3affotqei.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ftmpybgv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3nkyybgtb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3mapsrdxm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3htcumshq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmvyowwq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ykybzbnv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjryssdc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjlbevvr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrmvvwkd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jpxxlrht.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3njvryhcr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijuoqapi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkzfurab.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cfaijdqz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3yapfcqev.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mvhsvlie.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eisvnkxs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mmazilwf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oyrkzmwe.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vlcgbqnq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rjjjrqty.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fyuauouf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nxiwoeur.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3yjeqbvga.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kseutkqy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3dgijkhoi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fashrekz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hsklzkfj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rvhqecwb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rdxdpjaw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pmgkbses.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cxswkigb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3muuosucp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3oianxpfo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3yvntiwza.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3szwtfbrl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vhhswhou.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jgdmyboo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3uwdqwjjh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3zaopyhep.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3csyrenbh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3znoyeayu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3dvqzjqns.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cekjlqyd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucwdxbei.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3urpiicuj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uubhccmk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlbuwfa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mueintlq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3omxejzbq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvuknqzc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ghonsjot.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3uhhohrhj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pxgvocbr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qxbcapbw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3tcdpzwbw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvvethk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wcrkscor.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uhocvszi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3btyayqqs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ceiwkpgr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rltdnzqd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3emlkdrwe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lapyaozs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fjllawdr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjtnknhp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vskaghzz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3scdgfevn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3avbofbve.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3fagljdfv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fsnupdnr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cueqhevb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3agxrajxh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3wovbqzzz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzmtlpni.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3simashje.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3niwjomxr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cyrymmqc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uyyrtqus.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fyyqtrqx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xnwnjqkl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vdautvkg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bzwupsli.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qmkzhwws.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fqvnyxcs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kfqjfyuh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3liycgnua.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ykngkcan.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tkhtzuue.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vygnbsvf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pdrwywnz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fqsryzab.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3avjppqgm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zqinweyk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vedcdnth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zojayenw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xiesvxfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxwdzeoh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vvccvhcs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lxjaiqzm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3edhafmin.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lvwcluyt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jjfxosza.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ghutrrpy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rmavgpny.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ypbzfatl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3voomhaus.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sixzspwu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cnrsbtmg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxsjduia.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gqdkohxl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xpohiylq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wskbblto.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kicvnzkk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jgthmsmg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pfytciow.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fzekanlr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gnsuxmtm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3obpbapxg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xrvaxbfs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixkvjfbv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehdzfamt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3muxvigap.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mmeklbhg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3epitccwl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kmscfkmb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uqbfovvf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnekvbsn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sayndwzk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ydcactoz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jhpxtmtz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3njuqsjhr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jefthnlq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3avfwkvmh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3myqytwzv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pkztwrui.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vlvgjjld.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvqoqmiw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kvzgriyc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfydckxf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ugkgcvmk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kbihczsc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqzgpabb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ypqgbgkd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vgobincy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qkhdkfqe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yqiduete.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bpksoatu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ralsysoo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wnzqjnhl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ghcbftkk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xwgtuofk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3uribplzq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvclcaml.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3osbjhkpa.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3frlfbybp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ladtfjhr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxlqmkgx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rnmuaqmc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qqtfzlea.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3acsaerih.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wgrtblwb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ywjozten.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kmleftjc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hamlmklb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fmsfsmvk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xpkjewaw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3usqfqxjc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cofgyply.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fqbnazgc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sfivperf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jyqapdkw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dulcrcog.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3totmpwre.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uksuhimi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xxcbrvhu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qdnsrbio.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lmbwjock.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukgqaqyn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vjtgsmhn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sogzpfqn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3adxglzgh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kxdcqhxv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3txdwcsdq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3otkoknrl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xqupeioi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3sqfkewbp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hxrzpqbi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dsdhsifr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gvzkjuco.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3udqerluq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cmewgkfl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lbkstisv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqnwtwym.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kwmrpkgk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vbmnlmcm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ciinpsgc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3daygmaif.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ryyvtcfy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3buuqdghi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fthudswa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qoiyyibx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jdqwmryy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybneymjy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gxdgilrf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gmzqnjtq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tvsvptda.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tcilbttv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjdimxun.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etewfapt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lmxsahqw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xfwheoco.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3whbmkbgu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lpwfspdn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mqeocuow.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wywzohmz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fhxyhvvd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xceftkxz.html


<!-- 参考信息 -->