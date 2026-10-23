代发 wailian999

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hiynrmhc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3iqrhxccs.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ktauazwf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ruttyobq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3fecppbwa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jxwsdtki.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3iesqraum.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nqlfehmx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fvdygafj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ffwqhpbf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kdbdfcao.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sgkptwau.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxyyerp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbkioqn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zbptivhj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ppltmhty.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3viaofini.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3dncnpdog.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3jtcchikt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vecmkjur.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jkgxhjuq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jvuwqrmx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3knbpubbv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ipczogcn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jkwfwmyy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xvckgfhg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3csgzxqgb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3pusugvnj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cdcobhjo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3oegoslky.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dyfwzzzo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ffynlrlt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qljpxdwp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qgwospna.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3enilurzh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3kanlzkde.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3smxetphj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hkzasohq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ytuztgee.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3bkjphkxl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qwrcyjdf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hjmdncks.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pgezwlvu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3emrjxnuv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3obmchbqb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jmfrttfm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wxdyyuls.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jwqbotmh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ouawpxwm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3atyxqskf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vdsemhlz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fogdqcww.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ydlnypez.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3trqsqccf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3spywmyet.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebpcqsen.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3gmttwocj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3klvfzvhl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qgfrbvnq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cdgdhtit.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jbugzuwe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3poslrmlj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wulrtocp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3dovtrmfm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hnqitdyu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3jqetmbcn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mxcaxzyp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3emqjricd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iylbizav.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zwrouiah.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zrvyyfgc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3aadlnfrc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uymbpvvw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gwbzkmha.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tkcnkbac.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ekkcqoep.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3oqocekjd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ebomopqo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xsokxiyt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rszlcuvb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3kxlopuie.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3tiagptjw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yahcbxwf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3akvxistt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mdeqycua.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nfmxjwba.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckvpjcma.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ythhlyat.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tywhsodx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ocdiguik.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3crycymkl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vpofoqes.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3yygcwhnw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3bqmoibss.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jarivobx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iuizrpjr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wemhajur.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fgiusblb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3bpzlcszo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pxpgqdlh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cxirqfhz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhdxrtez.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3iuavgadl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lzkyaxnk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uehodyon.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zvgwnonq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3stkwqlpa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bugmiube.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dhtcmmen.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3qyxwvbht.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3jizaqgky.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3iqpiqtss.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3cvvgfudr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3orrlzhbf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xbiehqua.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3wefjhrai.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3emkshtje.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3shrzwvic.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fjrgjzxf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yeptbmkm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zngjgbrb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fmtrgesi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oggkkvjj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ayrwxtqo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jztkqnzk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xaagrpoy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gtfknecd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ktcagnxt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rlhkfrlk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ltlvfxwa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3nbplhcab.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ghqjhmcg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mtznopxu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nqmskqrp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dvmguntg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dzljxkjr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lvuimsfm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gahftxab.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hoypeitm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ewmdxrog.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lnvkepic.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ytvsgduz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zdqshxab.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqazjqvl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bxwspnsi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3aajpakmu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3mxtbiusq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xosrgcos.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3oonbrhqm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jnkkuehd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ahqtxqza.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ekfjbfoy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3enfiylnd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lnzarfym.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ygoogiqa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ordckvnm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gqkitzbz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hccyzadx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkkjfyu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qowsvapk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3khnrovqb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcvtgvxl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3oeayvuxc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hjntmchw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3okdzogvm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tirurbur.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3xzcbfvkc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3mwfsqrok.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3uwjzyapr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dvshyppr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3blowxgxm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bxtbwnnf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fclbnftf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yidnkrzw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dgqeehuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrjbrlgt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qjellydi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cnfrqanz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bbunijvx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ehvjvssl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zvwnyqsw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ckyrzvzz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3smhswqwy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jgbmljag.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jkbgbdcc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kfjfwutu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3edqaxjjk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zoffilcj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3taalvkvf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3acsokymd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pkrnlzbc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nsjmyllh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zoaazbya.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gmjbwmbj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dpxxskkf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3tddmbsac.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tkdtpgpj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qujrptfs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3davlzldu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txfhbwsj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vsqcyqij.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tjvpktwk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3grlckdxo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hlzwopus.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mreuspbb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ectosvtz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlphxjgx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3czgzjwoh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3chkvlvan.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3flipmvry.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jtuywapa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3slvohjdy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dsxhjlvc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vnllnocl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3loncmsmg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3itmzvnlc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eaklmpad.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gpzxzvhu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ffcfpdtz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ccavmery.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3khlkotap.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rjuazrub.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fotfsifg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wmsvkcfd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3opogvmxj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qrbvhfgo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lebxzjqw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gzyeykku.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xoyozaqj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3slqfgceu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tytcgptw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3asifscyi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wmbkglqj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pcysrfug.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qiqrwtma.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eccwuycn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3faviagcj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rtpxgaod.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ubovkxku.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vhklmmuh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3deycgphu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ptilqtto.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zuiqcaej.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wnbmcxzx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xepxmfjq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozizhwhp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tbriseuj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gtbdozgk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3imqqzgkr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3iuzplsgj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zawiebmd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqebsfeu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxgqanml.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhflloji.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tnvrwadv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3hwurqikb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3juthmdjy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iohqspcu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3idqosxkl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hedmjrdx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jtnbnpde.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vfxcfzmb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uxyebxgx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ebipsuys.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ibtzrvyt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wbmwrmrz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3maleqrrp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xepufnku.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gtybhsrn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gbbbljjt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3flasqsoi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwfktnrc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wbwivcgn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kspzerjt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3egcwpdia.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmpwkfxq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3msuznowr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zkyrpias.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gfnwyjnc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wbzhiqvm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fvaidnnr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3osqsjcav.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3htkgqxor.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rmpihpov.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3alhwwsxr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ubqskrdi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dljqyhoa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ieulwxlc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vvigvwun.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qvtbfaar.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kmbkyoyh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3aoygbdzc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3soijqcme.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vdyuxnye.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3uzmlggpd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kzmzmkub.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3noelnxzj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ysqgfndl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrvujbh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3enjedkhy.html


<!-- 参考信息 -->