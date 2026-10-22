代发 wailian999

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ycehccnm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ncuzpbpz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2oswziief.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cbkoauap.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2isikxysa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dxesgipb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2cuequmcf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uajizmtb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fmwzumxj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2kamyrmpj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2olekhjar.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2snjomvnx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zazcincm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ocimipmr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dntikthi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vpkwogyw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xnzsdbnz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sxgxjvem.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2biczfovb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2avwqmwxy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2swlcaplo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2urhyqyfu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ufuecwdw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kjijtfsy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntrzqxpj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gipnyirl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2gbronrnk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2mkzytvny.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2uwfqfjfp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2byxkzepw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nfrfvicx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2svirilsx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qavddenx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hobmsbeg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cnnlmvbj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2deqqivck.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rbzopvxw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2skvxmbft.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2muwyumjo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2daaqaxkj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2zyxncexu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jazmhwer.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2edvyarep.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2usfkhcst.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qqzfprlf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2betruspb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2brwcmhtw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jcxtuiod.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bptzvbfg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bzeixkht.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2koxkdtjl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2anztzbxh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aygkwgkc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tipgzrqe.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2smkiosdh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lpaqiczl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ozvikysp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rlgtiali.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qpusesnv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nsmiqgnf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dyfwityd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2irkyitlt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hnpjykos.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fbrbqlkb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eijjpixr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rtklvnoa.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gtfjkqsy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ajohnigz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gnqigwdx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lpwegjyp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mxscisia.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rmngrrni.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2owolzrvf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tqyizsco.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kumajbhl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rqzjhpyc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hvawzeeg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jhdvweis.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gswtnghr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2frxvvwye.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kgxwwzht.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2spyzoxoa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwrzngcc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yulgnxyi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvdgbmfo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xxtugogy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tssjdgqx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2okgooyec.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pebktord.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tutqkavg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bnkyvrxh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vmnxuhaq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wmxsxfpm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kyufzlwh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qvcdepww.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2unamzmdj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rrsithns.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2imzigduu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vlnbhked.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2egsytzbx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2pugdejex.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jlzohtvr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2syhxgqta.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2msuicuff.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ldtntxnf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dgkdfqod.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2maunejpc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ofnjlrzd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ulwztsee.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ppamosyc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2msnppthg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2jacioprl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vuwrjqvj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ywtpibet.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2raopemud.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ejfjazwd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2expifdzf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2qxjggrqe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ylninclv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2sbgkfimy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2vnwpkjqu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2whnboczw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnoiligo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggcvsyhj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mngzolgo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrtzirz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bdbaylst.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2dbqfuxch.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2haanwyyj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gqlwjibn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hdeuldja.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2cdqlquei.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vmgdxizr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2edndkwjh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2muilcpwc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wjdqhdfk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pzoxzkps.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ivqnlxmy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xjhwroxk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fablqvej.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mzzphsby.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nypexlbc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xstyhqmo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2afnrlvgr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2enpiunec.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2sdgdeyqy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2cduxutga.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2blfhorwx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2laeswcnu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fabwkpbc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjezzeqs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bdsbrcqx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpdcwvcp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vznuxaag.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2aqahlwwl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xphvupqe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fmgualjs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bniwukjx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2eutdbuxk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cgqmvwpc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2etlbozpu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2euolcbab.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lexowsfw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrrgdqxc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2bytlrtul.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rrltbzmp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbnztnf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2undctjfa.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2armhvqpv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dyabqjmd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zyvgxqzl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rvbapavn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvqqhjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jujpqnpq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ucnmncrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpvwackb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2wvmuamir.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mnhpzeji.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ywtvuzvr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qjudfsxt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2goymxmlu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pvcklcra.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rxyyjtnr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2maaszuzx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kxzlkkys.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2olypvuxv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2emagievx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2pmcqnjfp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pjytdnbv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qgxvdmbs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ieaifnnj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jbzfivcj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2lvnnxvql.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vdncwmht.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lvqhxkpm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2aswlsuwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dsfedfnq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqyahueg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mntcgqgo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pbhxoldc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2olluwoqr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2lrbmemwr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hzzrnjpg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kvqtuxne.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ttoiqznp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqhabjzj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jzmzvfjp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sunsgjxa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxhrlhyc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fqqmudgy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mtswzecw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfktxpm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2patfkxxb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2uergxgga.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahvzpjhf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhtsdtav.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ognmranm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2axcxbrdg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gjzhnllg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gmoavhai.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwghxzer.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2oekimcmz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wcdjrhck.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2issyrcrn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2whaffika.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hnxjxukw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2axpfkrid.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvvbirhq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2chjyqxjx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vwavauoz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lpfmwcja.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohgrwdur.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tfmjrgrp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jxlogefh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ocyxzcqv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hohvamvf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2exlsexon.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oheuxmrk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2amrehaci.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qlcnnvqc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hpuroyiq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ukfqfhgx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tgakjwtu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vbxteael.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lrxuvkmi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dvqmsgkr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ooqoluhw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xkafmhtr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dhfoyakm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2plomcjlu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2geoxcrmn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2siymhvlj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dtgtidmt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2umdzwhpm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hljjgycj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2afjzkyig.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwxaqjzs.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2uyxndqxy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2cslsgmir.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjxcvyti.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qvrwfzeh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2snypzcmv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbnocbde.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xmaqmhop.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ehwwwdui.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hlwjtgne.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ehpjbezh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zkhlgjoh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mgxphwfk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dbqpbuzz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bughtazb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vzqaiiuz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xcwejdqt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2okjuezrk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ohzozydq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xrqdhxts.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xassnole.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nnkivhmf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pkbeyreo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qnjfflii.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fqhnfudp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqmxooam.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yqgvsmzr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rcvqlvxq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nwghhalc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mhmuwfkz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2miowtzkm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqtcpmt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2maqymhtl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wrzmxxty.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ctwfbpcz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qigaskeb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mqasbejt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uazwxoes.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zpckqmsa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ijvwodyw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zlnigonj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dfbhdytg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xkqfmhpe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2kvluiaal.html


<!-- 参考信息 -->