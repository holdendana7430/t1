代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xxrdsueg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xhzgawzl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ugpvgcha.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3jgjqbzcn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3amzcdrmj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3betgqahx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3otbhnjds.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3bsaapgdg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kstbivuc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hfhvrmqo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zkccqizj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bdapebpv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vvxzamwf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lwbetysf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qbsotieg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3etyczoei.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zcypggjo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3yzsletlr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jsfkdcio.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ypnerajk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oewdhpaf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3cdwwjjic.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3egymnmhy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3uclnujef.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vdggoote.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mlyzefqs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3szbpukyw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mrlpehac.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3skplbehe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lsfdznsn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vmfwfviz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3kqicsszu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bzlmkvgj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dhbbbhbj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ogxdbxvq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ozvbietf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3tpsohqec.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3kmrmqytw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3nqehxkxj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ymootadt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ptwqbguk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rrtsnfej.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fjzhlaib.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3mtpdvexf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3drgdjsab.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jkrxooap.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibefvyge.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpdzblmr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymcncodh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3byudbfzx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gaerujnr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fdfsxuao.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pjqbqtvo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ijypeyyd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mazzzsub.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vnryllvy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdcgrcc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3sstajzwa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ptchskhf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fjdwimod.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnnorr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3stybmswi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kdbnvsat.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lvjptkzs.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gpikkokx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ebpvdetx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3sygikuyb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3msaeznus.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ygzpsqdt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3igajryez.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ybwuzgqx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3yznvjhag.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nugllhsq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qutsxiyw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yehzdndl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3vhkbnffv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yfxdhelz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hapjdewm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tsfouuaz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3lagtxvjd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wqqsccvk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtidnos.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3znlrbvhv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bzikhfhn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hzelhigs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rxryavoh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qswagsec.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3faobcdix.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jtcywafb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ufrfhqwe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3lrheknpo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xwjvcioo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfzmhuha.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cjfqymzp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ylmgbkyj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hhoripla.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3omkmebyv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wzflcmrt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3gfsphpif.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3fkvtoglj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hltlluyg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xhdgmsah.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iwmmnsqx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rgklhbrt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mpgvcbbb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xnlhwpds.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3buiisiwo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gghcnaih.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wavixurc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bydcfahr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lzzuvmxr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3phdqsvzb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcoafuwd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lhneboad.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3taopuokf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cdqikjka.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rlfpzbrr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuuklkas.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3iplwmzgw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zrysjwkn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqbvoxom.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vzsufsxs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yptoboob.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxuqmdwo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3eoimricg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tbxvlzdt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3schxdugu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3dnphyxmz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ddgmjrsh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hrtyxcdh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ylptmsls.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3puscuskq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ifihnthd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bahwlfvj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ymufkyui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frueaqne.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rumbzllc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3phsuiqzk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kizelfal.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3stsvekam.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hfahvsee.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sotytbgd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3tqzfvfif.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fkouuzrq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3azwxfuin.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hdghqtsr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uqjkefbh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pucnecbt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3evzmkaog.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cgbgiqwi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bcpuwvsd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dtnbdcml.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zszotyjx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mjecvsdk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3malmkjnm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3whkhohxp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yvziehbq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dcoujiok.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxmgarg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxrxllgs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nhwkxsub.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lddpoddx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yidxaaej.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cpaehuds.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lanzrcbg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3sabqgubd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnwqmgoq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqyqcann.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckyqnnou.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kptobrca.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lpixztum.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oneenudj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jkyahfjk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3cxyeiogi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdktvftm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3idimcnfv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wakxugoj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3geqinhaz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sjbrygaq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mzqsfysu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3myzjazuj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ndokqsod.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lxsnjphw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcdigylg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqddmzsb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmgamtgh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vimveiwi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vtpbpblr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nuzztadw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pnidcodu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fakqzdio.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xzusbmhv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfilyqjy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tftzwqdt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3djzfzajk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujpbkswz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ptsqsaxp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gtteewlg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhkkiogb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vvfrmddg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tkpphpzm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ccqabghs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ubvbqurh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3htuvjtwd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3skuxwntq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jdfexwxv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vxaiovcn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vkephvrs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rwqoxrra.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ceakaayp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jaapcwys.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebibzwwf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdaktotz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xydabngq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xosbapep.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gktxfgum.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jpgjtlae.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bjxxtdsl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3akmjqcbp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3masgklhe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3svobelml.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mywmwutb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hvpfgdmb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vmfceoat.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zmdtaeph.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbifnhde.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qajvdnbz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mbgtzkvf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ysvhacxe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gjoryffb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3euoyhbqw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hwgjpths.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nmxvjgqs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3cwdscjna.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gmtwzadb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hxvydzwl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jumcvceq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lymtueft.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3geljevpy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3murlviht.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vpxfzlyu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3taelsifj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3chhsgjjk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ukfprbdj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3legnkfvs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3oxxxbbvv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cpvleocn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sofelqpr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvwtajk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wcayeyoa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jfdzsdxn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwstikg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vynqomse.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ltrvvlou.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ubyansjy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ngcnpzlz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dszzxlkt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ibaplwxc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vjzfnyrk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wafjwwzk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ctunqmai.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3siorvujb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bfpzofyy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qcktbclu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hqbsxaeu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fuckmuka.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3blppsasm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bpqplptj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3atofvtlh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uvfqopxy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jorqxjjz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ikfqqzef.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kgonxzdw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxswdukg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kgojauty.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xoixrfwv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xmoziutn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tblbcaxd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cyqmfkpp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lrhzixeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwtqmgsz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dvpvzesv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpvprkav.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3exatdpmd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kclbnfrs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixcwjhmo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3unuadmoh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqucrfwb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qoenjvyv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zauyncrj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lxqtervl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rjeewkch.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rkqyfzkz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3boqargot.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzyzgrhc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahhastjd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uoucgkmm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xigkwovj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pzvgutkt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gipyzrdi.html


<!-- 参考信息 -->