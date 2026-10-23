代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3eewnsoot.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ymjfzjgu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kmrzlpux.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ssowjhlg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3srechrsr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mzlzlbol.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3liilctsj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hqdlrjip.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qgcghmnk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3orncdfvq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xtpvviia.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ootmkbpk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wmaeoges.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3pszqiiuu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ndbnhgny.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sbesvaam.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eeuzuvjq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xwnnmmwz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zjqcipae.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qftkxnmd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3llqpdfqz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3hvzdoxvh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mzqlxojd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnngpvks.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3vaydggar.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrfckke.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3phqehekn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ahfjafcy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxuffxsi.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3swaczfgo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ltuabhaq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3zndmzooq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ohsqudaw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3yojnmhmg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nlclgmbl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fzujctar.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wnyjrego.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3avazuxwj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tkihabda.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qogjlwyx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dnrwsrat.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xdnpqxmx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3duxekunt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3akquowyc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zkkytlqu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zkkhgrhi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gioxvhaw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3viokkmhy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3mxhwnkgs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3krgzmfhx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jefdbueh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ckncxzrz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pvexbmwd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hnzdguwt.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xeqvdwfu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xjivyiyk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3angbcuki.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tzchassh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3upupxwcz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uniolfna.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qpftqyld.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3dvupxjeu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bwifcawf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3thdgnjrl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zpjvhgtu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3iwadtfxi.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3badsezyy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3enfmnaun.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ynuvgics.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zlntsrkj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ndjllmbc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wyqikszy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lkcvgdwl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xdzzemza.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3iusdkcln.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ntkkvcov.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dnzkureu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3enoqvbwd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3pyplessy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rzumvtlr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3uliryrci.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3fizzbkzg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mivaeitr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zwycgcmj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3vlwlfdtn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qlugccsb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3liummbtq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ocmunxhe.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zwpmojdz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uoborzac.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3adaedfkf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dyncinup.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbotubbr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ipecbbuo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ehuzdvax.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aaisrxed.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3merrpbha.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrppdsw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wokxdhqs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dwjxnlmy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3glmvthup.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xcrgkant.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ynsvehqt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fltnotao.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vrwxjlmb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3nwtekxue.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3smxrphxo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3jqxnckow.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uemgqzex.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yqsfezsw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3arjlqejg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3peqrnwhk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bhslyumt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vayuoevu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xvdsgobz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3uiuoswjw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qpocamng.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3wquoygqt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wiyeoawc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3yzennltt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3djbnymko.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gvfqwqqi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pxrgutqp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3orhsjeif.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ajiwxkks.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kozwhmuv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3womumqgn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkflnkw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rwiexpzx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uuvpoivs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xenteaet.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tlucldri.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tddoonbg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzeegjr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hltjzscr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mcwpbjtr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ercixfgf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3aesmohxv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwtnflau.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fhaxcszo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3caffrcvr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tnuyopyw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xjdaluor.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3apdgttts.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ncnpeydc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3miqpzzyy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3yyvxxcmn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3meykazft.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ajuplvqr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ddzzjmob.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pkilxcjf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wsvqpvol.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3muxkkpax.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jmpjwuol.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bdhgokeb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qkmwzgpk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzofqqzy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vaboboes.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qagkmmoe.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jcluaftt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jgotbkkv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qoujxyab.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfomzezk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ixgvvmuv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ywlajqmh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nfxlrtxd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3tpyhdabl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmbuzbjr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3iovfsvsk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3potwleow.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pkoehixb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jfvnvnbv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3bpuedady.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzvnrha.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3pgtaopum.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3fenxnxhi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3umnvaxvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oftrvipf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3csevfxft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qptmrves.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kivoirga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3khbyhdrm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhxhwotq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3badrpslo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3myzmkjbz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3niptkdqa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3sawgbvnp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3aqfmcnvs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hslnjmtq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3opbxtfbq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3kbtbudyx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrvqhhto.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jnvziydr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xedojrav.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3evbubdfo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3decsawvq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3icmjqkgl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dcjzdvri.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jgfqytdk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3cvjgdppz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hnhbezar.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqvxuyra.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3owurlxda.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkezaed.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rkgcwbcg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3chhjulwz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vagfqine.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3absvdgml.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rioljuyy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3emyyromz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvlkqvcj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpnlebkc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vvtasgke.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qnwjwppf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3uduyxlmy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvipfdjl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sgmorokj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xmznneim.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hoxgpzfq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zltrqohj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3imcjzdwd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qbmbscxs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3nnckrdwi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3usiwtykx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzetammj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3afkpqnyh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3cejedhku.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dasqgcop.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mrqbewbe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ainqtyam.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ugirtccs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pogoluxw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mucpwghp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3amkakbmd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vtbxwyyn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfveiahh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpkpfmlk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xwdaqbsu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofjfodcy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vyymcyeg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rruqopeq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kmtwmvwf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ytugddqq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3brvjizak.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pfztpxmv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aelfuuqg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qdusjvrb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bgxhpdfn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zpithjxa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozshekka.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bdnuhyqv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hbogfudv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yizddese.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fbqoehwm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fprznnal.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fubwrkrz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vkqqtpzt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fliatrzo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xmjblycn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ssvyvcay.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkosuaxr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jhcbgers.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ycqxttsm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3kkupcwys.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wuojfulx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aymodaee.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqsgpecf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3fzaiintp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xgxdwhxx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ekkgzome.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fzgileeb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jfpbmstc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmuauosw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rllgdqoh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3todteqkl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdxmykhp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fvaisrhj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3levwucag.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lerapuqj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tsapqobm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bkyguocp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ppwrmmtn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kmssfjly.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nagbwmpg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rxuquqox.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgwxaukj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pmgdpubv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qsqzsxby.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gcnutpzt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ypqyqnxt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3neorxkwn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hebpxeao.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nyqibmfu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3paimajoi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3swtogvde.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vjpjqkxs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ypvhnwlu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rdowclyo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ltjgieyd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zjxmkxol.html


<!-- 参考信息 -->