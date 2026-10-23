代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ipozlgjo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mdaqqvcz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3zfajtdln.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qmixuncg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jengdpnb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hvvqwnrx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lginjczl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3govdfhxu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3cydvxdor.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qhlmgiwk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3yhhnnicg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gutvlppv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3zrbolxcu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gnvpwnqp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xfuyewup.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jitdxpgf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nbthpugi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3qmuffdpv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rzxfpztm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xhycttyh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zevwosla.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3srxkeyvc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3otcdkdco.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jvnyfbva.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qtdmhwpu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3dsaxjcoj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3svddgvki.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ugeplcfp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3agnbonhw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3cdhgmhiu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3trjdqgax.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnsshsoa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3myyhkbkc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pszfvsyq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3hyasqxmz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3hsvunlow.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wabdgjjc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qsytiasm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3smwhqyln.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jykorgcg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ojpirblc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bwkmolrr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jsmaqxja.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3aeokhmhg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3imcddlrx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bnkpowkv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hqdzgelg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qyrnipwt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3eebezndd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qfuhtfmb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pmhpfhuu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3sjutjxgo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3kixjozuy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3iwwssqzs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3daewbkme.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wysjqoyx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3elgevsxd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uftfbvxr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zcoxslqo.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ibudbjds.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gdkcriaz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vfzfeyqh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ewggmgbn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vbivosan.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vhkipwuz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3eudcgvks.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fwslpuqz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eioewvai.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hjwtakkf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pbduubyk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tekdonkb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hxezygah.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wtpdrtwf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dzqzclkw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nveqevrf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3npmasefj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mvvgpzil.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rckojkqw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vfxyecel.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3exuulbdg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qneecskr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jeeqtfgt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ivktrrii.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3powpfzsg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3sufzgsax.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3nnfejxym.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ofpgiwhm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vasyrzmh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hcdxpzxy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ipljauio.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lxshacsl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3kdeskfyi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3daojuwbv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kbazijvk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tihptuow.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3inoztusr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kskiolqm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3twagzubd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uybiuiim.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fgthonzz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cfegkrqb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3drspgmqa.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xaxvojoe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yvmzyndt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wsromoaw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3lvboezxw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uqxyjmdx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3kejzxnyr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mcffmmap.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3gfqpgjvd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tamvxpmo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3nhlxftvw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3azydqjvp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wmkeasop.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dygceyrw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hundgbzf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pizlkgwe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zsgqnqav.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kyqarbwn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3olkvdvsi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kwhwkejn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mjywxujd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ndotgdio.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vhxgqfiz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ziccsada.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3mjtxiezo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ngtekfrg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3dtgzsygu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3geeocrxu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpbmexa.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnjfodg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iisfoebj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsnmhdw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wibhepye.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nazlapcw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3zerhwnvi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pjkvqydu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjqwxyk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3yvlwztyf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jtjgugfq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mxyislfj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dntngptl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udubtsby.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xzuhrhya.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3buoztetv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nkgubryh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dacgaegu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3miijclzc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ehchvjal.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nydzbtpv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3epubnvqa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ebvazjgk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3newobelh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gzgvobii.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hmaiizlk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lphjwimv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xlgjnlrl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3thbznagr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lvcpfrfm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3zrhwyzpg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nsuxgvrh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3mjncitvv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kkdogxjh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtwzogbb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xgqinoba.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3atjuccoc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnpggxq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ffoxshhc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wszasgjm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hblnrjhb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nrzadxpo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3isbookgz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vpurgjlx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gusxxjor.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuqghri.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ordbqqzu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pjxbeyrh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hjjuksgu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lrsdbaat.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vtiwsrfs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3htveyxwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwynfqbu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3akildald.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztgfvhce.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3mzqifeic.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cljbkfni.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axxjzmno.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ppbandnk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3evjmlqgm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dcqygvgy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kpugrsjp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iobksrxs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ovbxtjgl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3mnxoodxx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dwmqdwzx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrmcxnkh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zdycosuv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pjxqxleo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cstbroqr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxvvhjp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tavwlksx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3peujhyrv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3xyqpsgie.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3etrgqbyf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qskvnzyh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzlojfc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yemioafh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zqrntuzk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fbshylqz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3oijlctez.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gkdbheco.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3utzxqkvr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ocapmcib.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cwjsuqlb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gnzyxexh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hchwbzbp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkbxriwr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3meqbnjtk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mtglnary.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyeiklux.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bcqdfgzl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hvqwboos.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fanunclb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfsejmjq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxsiykww.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3imufchrg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kacavqzo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3njtcrwkp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vbqfvayk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nuaziqdr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dyjlrtwq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvueqnif.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3eogdicuc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qbvmnotc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kbtumvcq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bqslzwcv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wmpsmans.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfebxclt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kupqqwux.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vemryzka.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzcbcgpv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aqwnrsue.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqjvtxlw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3spfseubh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cojpbdoc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3imkadiar.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgadpkdh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uefzhjgc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3agvetswi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fxxjzwor.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ngqejzhh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pmprktkw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hlaeowov.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3appypivq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fivuxxmq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sewnhjkw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3siiokyap.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kuaslgvd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xkrzdlqc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfbzfear.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eykyrrqb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqovdtsy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3loclsjmc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rtjmlcqu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhlxpxxt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nucskbrw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jjlgrtfl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3knbvuwbh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fdmsavhh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bqmszvqt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lccrkhef.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jkgtsqif.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iysgeprg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xxsmwpvb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wllrgvnc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ifuqddsy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nxyhehfb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zyymctuc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ncqufjzv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mamwqolt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eeykhdir.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wxfvqtyk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3buedlmni.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xsexqwti.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zdzyfjep.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dzjkgzcm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bwgehcma.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bxakwrre.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vhtmdlsc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wziuryrv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3sgqvrvxv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vxbilzjw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pvqoskqs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kyazoyhu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yktbynie.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wzjouyof.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xabpiytf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3yjnxrfob.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3letdsiay.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zxdribug.html


<!-- 参考信息 -->