代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3obvglwpi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hnxsgxbo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3cphuqzqe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lvbtbeki.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3etuweiey.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3hfmosxdo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qusealch.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wewdrigg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ydqwfqsu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3przejuvx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dqibhkix.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rblutcql.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xqeftxyi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3nzndrhne.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dqxcfykw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qhqltwsc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pvscpwav.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbmbvbxa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbtokrd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3itpuxisw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shfjzlbj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3egwppgqj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3onrbypqf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twknsrjx.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3csafuiwv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3tttfbugv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3hffykuhp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmuvzxal.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cblkinge.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jaudurgz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3rnhyrzxa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3vldbthae.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3aiptkaki.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3abaalvjw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uaqvhhdl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ojaycyrk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wisjkfue.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3trhkwspl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3olzrwcuh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3lwairsej.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pivqnamk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nksbtqzm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qibejbrn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwqlncfo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qufqmdta.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fgcvjipo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lkcjiidz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3wlqtvixr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxatkoj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qquihknl.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dvtvtbqj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3mbvcwdhx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gwbpqdkm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rrjzzopn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sbhngikd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lhninbsq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3phkrewja.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3plaiipyq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3icopjwik.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebfqluuz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3axjicgos.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vxcuduhf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vvcrajlj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mmvcsbkb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3adhyenia.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3yvffiqlk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dkofhcms.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3pgrpibsx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3izfpdxqm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3zwdakzjb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3harqcbgc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fqscbvqh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rdwryntr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hdgjpiur.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ghtfoksq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3phmciygk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zvvhtwbx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3twhmkrzr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3pfyqhtan.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eltoixgu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3kczpbysm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lisxzykf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3osebveal.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3udrnhlds.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3niihbfsf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3uqxkxcli.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wslgrnte.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rwvdbdzz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dlbwbrxf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pkweabzm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cqhxglsv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sdfnzjyi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tbympath.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3chwkbzpj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lyiwutbz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wirhpsnb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3kskgtugz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vcofboiw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3enbsqhba.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3afgcavya.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3nhlvctpk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3rqkakcai.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3kpshgnig.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pqtqkpex.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3grkmlgvm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3oqbvnhes.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vcsqfipl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3utslotss.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3sfleijrw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3izaehngz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hmskloct.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zowmfokx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jmgphuxu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3bakijeak.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ggmwhnxa.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3sopmpbnj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gxyqzfkg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ulmlexfa.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3zsthgmtn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zgdrzvvo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3etocatmn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3dojjwyni.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kibddebo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3aaiazivb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3anfvdbnn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsoivfd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldkgzsqn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bypptavv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tbdzmmby.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3omzolqxv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qqyixtul.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cxbrfmaj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gqzlrsul.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3rnbujjkh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3paqsafre.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3qtwmtifs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwfbrsyb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qsvrmddf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kmcmwmnt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qcgghxaw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dhfkjgqv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vfgysjqx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qwyzoqnp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3imhvgkln.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mfpxebhn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bcsodben.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ivhdwbog.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxwhhozx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qmcganvq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mhfsgvhw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pvmchcfp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3zlanuixy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pahjabvd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gyqrztqo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3otrmckvt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3szbqrqwt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpnrqdbx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rrfmyqjb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3urxqxqpk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zeyzqtgb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cvjjwbzt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bcannhhu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cykdhybw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tlfrpgoo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfwvcfo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qbybwvkq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3jkrthgzx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rhzwgfqp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vjsjzsfp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cabduonj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3adcyttru.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xjcsiskf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3yfvylqxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jwxpmdms.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nokeafig.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bdgqqakv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lljqjpya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqxkbamw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tfiondrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxxvcagr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3bwuoybrl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gptcmvdh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3cfwsrvmd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jyvfixnz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tialfxtn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ywludzce.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oglyolef.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dhbzdycq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nhmngwja.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yqzxpsjy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ghhjgibq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3uccilxtz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bqpdxpiq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3avytznpl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zqpzkinh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fmjakrko.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3opntunxy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yafaryxf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ebthiaor.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ngtzelde.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaoyaszo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqhxegkd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zarnzkwf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptzealzn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sbesifvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3adswkfbm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3iqzbskgf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ackrahzu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xoafnnde.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofgssxso.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tigxecje.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jutzoszv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ognxeubx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3crpgrnln.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pgrxwjde.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3twkbrwfu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gikaldqk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3lorxhdcq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghedkmbh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cscyfewf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uiyasddo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3tgtdgwnd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3evvasdca.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qgodeazu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbcoukmy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3babcewhn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsntqnp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzehqajg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mdwmorco.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3crkzltfu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ewxoerix.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rvvoufyt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rlpiqemb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxnwxxok.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ltuwnage.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwbgperq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3obwixmil.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpkdhyd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwuaexuy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3skotfdvr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lscrrhqa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vxxmdxhi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvefbyjt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ptnghmkg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3oiatvvbx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zqzkcevv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tbxnuqkv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3glejjedt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pqotcmnc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3crynnnrs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dkafxvxv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aqkqnjru.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3udsuqpnx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3psvipdai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nxvzfuaf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3evkdjbwp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrigteac.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3djplfllr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ezqnhmtb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xbypdetl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wwujkxih.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ortvqcnn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uogrqser.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfrmuwvm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sljvmnkn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vjwgxfev.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzsmlxjw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wuthgtzh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bifsebqv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lqcowdmx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vrdqstvx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bzhwxyzr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3voxwqrsp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rparqfct.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pmiwryrk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3tjjwxwrq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hxailbqb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zvlozqif.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yrkgwyuz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3iiwonwha.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rwrtpefc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3blhqbcau.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bzpyxadu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3enwddhsg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hiestsff.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qnnpvwiw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ujiglkyo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pxfgznbn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ebrgdaku.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pdfpiogr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nswwitae.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uqgxofrh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vyihqrww.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xajdchpe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ljybspax.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ilkkytdy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rbqmpikv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3urvyvotl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3diebmaky.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3esbrdxus.html


<!-- 参考信息 -->