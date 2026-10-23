代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ajludkoa.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eheyqkaa.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tljzaamp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lllipqnw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3grhpbyog.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3xxahedqx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3kofbwirk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jbmjugfy.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3csjouxlr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nrgukuye.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ewdlprgu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3boecboek.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rjdvhbfw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rwtskrag.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gjwionrn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnqpkq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jbjtkets.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mbryvxzg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mwiebnmy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lkjaselk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pfcrcnsb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3fimytuzm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xfwtavih.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lpfkocsu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jieaytac.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3weldcptn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xuomnvnd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xnsslafh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ojdsegfs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3iomotnrc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dtgcsepd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3bccvwdwd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wmjptway.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3muanmzej.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3rpxkxpct.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nesrtngq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wuytsqwg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lxrqkefs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrdacpol.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsiufbnb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rvusswxz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3kqbdjwbc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3exeoagep.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3vevoxnwn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqyqkkwg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3balhracp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dbveibgw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggkhpeyj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tvsyepgz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nhddegen.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rzjglnsw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tgqyszqj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xhslrtjd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3saqrmvfs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwjuraz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mddyssga.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3olzrkgin.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3syncrasu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jjlreolz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vmutnthk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vliswcaz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3dirwmgtf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zvegnump.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3dvtxlzfj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iixwgbvp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bqdnzayz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3gegccmpn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qwppvoeb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bvjepfgn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3okroecou.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qhecwjeu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3plhsvjxf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cdlqqmrj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3rugsqofl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lyteshzf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3yfsznvbr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yuuetrql.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3gyphuwwi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3csxbzeac.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nhlsaqnv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mmclstce.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pnclslzt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gngvutmq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsxburdl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gscfwilz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3opywdemu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gqbmeecm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zccijwrw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pqoqlqaz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xgterbyf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3oliuixtc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3sfifnvlw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zkdrfjar.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gdhkyomh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jnmydnoo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qfxmlort.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xneijjmn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3isxyikxs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xkplaxfb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3exbubbqv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xhdhcmtr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3moygkyni.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3evqyrqep.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkhwaly.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sqcyudyp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hniqfzgy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rmiyclpv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ltxkpxkr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3oeqaicsb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lhpvrqrt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ydwqhawg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3umzzwwnr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qwbbjclc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3thaqygji.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kgcyfjao.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3koimtbcv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3otxsuqvv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yvmigete.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oobsgjdo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jolnjkle.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3grzbaezv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ddnjvobf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wobpggka.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mjugbofo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nupgyctj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3oexqipjh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ykrzlhwn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ofztcxcp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ddgeqtsk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qvxzggvt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zvjictpa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3dejciysb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pupaybjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnbffszg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fjhosjta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyybktnk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3urwfuntd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3khtwjces.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3olwxusfm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3clwsppas.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3egqdijfj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qaewyswk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zdfhxofz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pfkdnlsh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cqahakjt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3uyrahhmo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uzzyztuv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfeaoovf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3shzocink.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yslerudm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lhxgvzqa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3eueunkrh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xrjhjtvm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kyvraosz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mwcyndjv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kryejqwl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3disvrkxd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mwmjmpwh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3acwzxwcw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vumrjitf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jlvqrdga.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yrmfahbr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3utfceqtm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3skrtkslp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nnegglck.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hfjzdwnm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntgwotnd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3alatcnxm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nfdocpqo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nxeppxis.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3bsfydpyt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iltlrafj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lzxmovys.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ggnznkjq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pemsvnim.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rstogmvm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmovjzqv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfxtdwtu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jxoybxot.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qqbjkukj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbwfvpvz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sbjjsxbs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vndvplng.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gspntszi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3osslpdyb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3saqpkbca.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3calpvpod.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pjrqeciv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qvxjebih.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdkjkpih.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3senzvqbi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dbnjhiky.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yhzpdmgp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zzgtroxr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hdzciqbb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyjdzirm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3fbvwhptd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsrvrovp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mmvcicae.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fmxtlncp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qhboumxg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hyjoieha.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fqvbryhi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tmurxwkd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sqewtpcs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wxdmuhmj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bxjaigpk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hkixbtan.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3apwscvyv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ojaibwer.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekfphdzb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqqmimwt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvxphhix.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uztgbpch.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qzhlccin.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3utevobje.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3glhnxhea.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mujhmoph.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wrevmaqe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afzkoyku.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pkrpdhvz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sceamrfe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3czoafkcw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdqdufxr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3inpmenkq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pvpywzok.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hpqdpqwr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tgevrmof.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3znakbjoa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tkwgapff.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ycvvudmr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wocsnudo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kmejtydp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mjshoccm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jlpsyhae.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3snhwwvtx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qifpiywk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aixlqcqb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uytlyxnd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwlpusxi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dzedshjw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rtpeonkh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3avdnwouk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nyhohgph.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ossourri.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wanotvcw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tmxcuams.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hrpibtoy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jawtoesc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tynqwvzk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hldwplgb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3junzhfqr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kpdrlijz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3uzhdmpix.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bouwmhpb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jlirajix.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3roeyqjnt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbqlsmp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mpqwaxlk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3glidsobc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfktgazh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3brqsfcks.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3powkuhdq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kflhrpmr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ipsxpcss.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3auavntnd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uoesflmb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ydabcrea.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3buwurssj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bryxdqlz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3islgesbe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gdhvtbwo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ncmqvkam.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3raozwodm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3obzcagxd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ootcsqrs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gqlabqxl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3offjcwcw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3athanfgc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zgfajhbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgrcjsuf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3msaxeain.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfkiwaos.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xzbbeswf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ytqegafj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiqjwrxq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fkznffky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhwxmddw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrrjiwqo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ybgddchw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dvbmmthl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzfgwenc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rvlkraae.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ydevvypq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ioxpxtjd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bprvtmhs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eadpekix.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yzoapssk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3iqgsrfzj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ugzicjxb.html


<!-- 参考信息 -->