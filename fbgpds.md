代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3oanfkhmb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtnfwsu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3tubqevbl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wbdsoyxn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3typxwyjq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3wcvraayj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hknzhehg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vgpjjxcu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fsykfgyt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqyyqio.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3usxyaqqh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3huyfltss.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjogodm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wfqgwvdg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qfxzbsyw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lxlpekrx.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mxgemkys.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3uuyeohzo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3kbykqobp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yrslwrea.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3oekjlrdp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yisigain.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3rosqzlcm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rcnmxmfn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ntjnuiku.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3osiqpxwg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dyjydiil.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xpwlorgj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rlolkpjt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uqmbvyrs.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aqcuunfn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ioqyosis.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wniafrsa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mzekbwci.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3styhwwkl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3derlwwhu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rytlosmy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kyasgerb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zssafkwd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vztgxvkb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ijxkhklw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qpodgvtd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ovrgisrj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3zrugmojq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tqlxsmqi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cyqxelro.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qhnrmfuh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yexwqfkk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iovbpkfo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3idhrqxrh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ooxvecfr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hbhbzmvs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qaolazvh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ogcsfwrr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wlpsayws.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yqpojvxr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hpafhrtj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3luwksslq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mqhmhwti.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hkntposk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kwlajxzi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3augplcyl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lvislrut.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xtkxqdtg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3koyesgjb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tetpwbwt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3nmrpmtzd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3emylfhwy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gimdargn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3krkufyih.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3lrrldzds.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wambuxnn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3aaybmxzj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3tkytuwwz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rczgdzcg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ciibbobl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ealrtxiz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ytxwzvjf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fdegphcj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rrtuzrrx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfwqhfhe.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3saawhnvp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tcanxdqb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3txpzrhga.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ankkpsrz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nycvrrhu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gfyvurpv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gzlfyxsk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ifopftll.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bqmrwpnc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tburqesq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3htuqpsws.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dzazqukq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mbplbvvc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3liyuscvc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3aoeduchy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3inxdjofl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3fdojmrnx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ruazgnwj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mmeejafx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3igooovbp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3knrfthka.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wwqtgntf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xdpaxfzu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dzxassdm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3uopvpklv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3igmloilg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xvlntkte.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3vadimytg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ovanjyek.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3oxodzoqk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ijqxsskq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3dmertrna.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3zqrswwud.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3nrskfury.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3jkwrgvdv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3bcycqiqc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cshfdlsp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xpzuivsz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqfekpf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xwzlznjs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jeoapxfk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kggmcjlq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qtyhezjn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rhlpywfr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3mgjnxwfg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3whzqfgge.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3oifvfyqi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3cucwrfbf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3piuyqzkl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdpunkmg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3nfkfaenn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vejfukqi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3slrrwycd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yveyzhav.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3pndxhxqo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3madmlokh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3svouvgcw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3getzwwuk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fkfvpbyy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lkegpxuk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3uazhwryo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ixpzmrgz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3edbabunc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fqhwkgun.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uxulxhom.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3whqbqosv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vvxslijj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bedrkzjn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3wxoehvrr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ugsmibil.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nkmfnhrh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uvbggigv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3arvwkopa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xzlkebos.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gjzsrcsk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmidvif.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3anjkmgas.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3yeljofto.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3apjndnai.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kzzuaysl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3uflgdalz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3uwddwmiu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3awrzmzev.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fgfwuzab.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjtyrdz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bybtqgzz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3reelakff.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cbgtcuim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eliswhjk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pjfwocne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfmkopym.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3bksrgotz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iihwssla.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxctaffe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ryxnkqpg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xcwihanb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cgxclkrb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zobbstaz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xaqpzcsa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fubfocdq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3mezchfqx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3wjohdebp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnnvhjmk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rlemzght.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uhkfcend.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hnzgxnyg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bsegwdvh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xsiurbwy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3meljpuuo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vnscvzua.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bhbfrvuq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymgnrcux.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hvsctcva.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uiddyjyh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ksdzdxjh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hniblvvt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jvlcsxsm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pcmeqvgp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vajehrpv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hoaejzjt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ujnhnpzc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3omfyhyjd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3omejooyi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fioivpfs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3eokpczuv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nuosnlrj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypkwfxfm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mftsibgn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlirxze.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwzdsfek.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvpmacxo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuwvijqt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3neqyclip.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rbxplxji.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vcxydjgs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kxflnyvt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3woinjcvd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vswfbdil.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3buubvtpm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cmqiipgj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gxkhsiso.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfvrrqhx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ghibhqac.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xxniqntx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnqdobwm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jvqrrcac.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cwaezaoo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ylazykom.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3shnhkbpe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3capwrenr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ansiymnx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pacycwmb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pbxgtihe.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hghacxxk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ziraxyrz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3krijteul.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cylhxgps.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ztdzaymx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ucitxobl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hqkkqooy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qvuvgyeh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ajsakuys.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xxvuevpr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kjsjgfia.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3leqnjepq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jgfabiwh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzyhzpqo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dncsrsuh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xvfjpirs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bdtssrhj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqzpwsva.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvnonkfx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3caccbkol.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfolkds.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qgeqcfuy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tksqscxq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dtnjdyjc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nxikheun.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3yjpluqjz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oowbuzhj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3utxcpjbx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yhtanuoe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ffbitqel.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mpfnoaao.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jlkpknij.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gkqzweml.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3agwcbtnu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mtrynuvq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ufoxzmhl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oygpmubl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3sultmyil.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3usrbmesg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cgoeibdj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qdifrhnl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ngkmcwul.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dxxcnawp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhiwqwyp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jdaouxjc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xmixfapi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ybovmrfm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nbzshglf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgbehhkv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zqgriska.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3levxivyy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cggyyvph.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cbvzskoy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3byerzjua.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jxcekzji.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fgraaque.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dmlmervl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qnatvric.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aaxcihfn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqyfxxyo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayttzcuq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ejpctiwb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wffawife.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fghskcmf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gwjayinf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3shorufot.html


<!-- 参考信息 -->