代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3toemgath.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3axqvndtu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tdruhtej.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zerfzswh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzritgp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mzaujzfr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jpjkctnk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3svbzlcxn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ojcntaav.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3enpitnzn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sykmsaqf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uhuwgwby.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gqolanok.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3culkxjhl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mcpwdrmh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xuoaivcr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3pkvsrygc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nctsfqbo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3thefaait.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cjbvcdss.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ainwyffa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3huhticih.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3whejndjk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lumcbjjw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wapzahdi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3sszworyd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dfntemtz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vnromzur.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mxuwcfup.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3roypncga.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lxuknsoi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3wyzrqdhn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3exzhhbhh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fraqmlko.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3naplcbin.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eqgisrsw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rgusavqr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zhufvoqj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gxnxflzo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fylytfkp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3usofkpwz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3otlvwcrp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3orfzjibh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3jldrdmjj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yoqhgzfk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eysppbiw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdbimvxh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3phfvbolu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eyfqxurj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mxdztsgf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wuntbngh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3phgmvceg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3euzggbhs.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3whwrvukt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mxddzyii.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3saltscpp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cgqzltct.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3takpttbt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3njgmyeyp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dqzjoflo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3tldvblhu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3iliaxfxk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qththizt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3daipxsiw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ofsberbk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bytwzrbi.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3pcxurxxj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qjpmhhrj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mfuazrvl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vyjdggqd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tklvnzlu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ccfydlpd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hqjhgprf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3zkgcmkst.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3aqekqhiy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3srujcelk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3oogxpwec.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3znueqbmu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yssduwvs.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3szrctwic.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qdfiykij.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kcynacqt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fhvuefkb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzfrlutf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3npkjfwey.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ncikxraw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3krwtykzy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jyvkfmhs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oomfthqv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xyjweiqf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3azeannmy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3lferzomc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3rbfigerz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mwtwnmtc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojztflbu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ekcdgarr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jmxhjwak.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rxgtjprq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hmzzziap.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vqturcue.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kptcjrmg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bvwlxaxo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xbfibbpk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mozjiveb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vwyggemn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3difxoxfx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pqtqddfi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3fgmwrwys.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvojzizm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vfykgtsc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rtntfcgv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3txjuiaxh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ycaifcyr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dgujuiam.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sykhvily.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zmpyflvg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ciecywfr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajwogzke.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndyzjepe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gvuwzyqb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3alxysgem.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qhhboskg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3swwjwgry.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wtkwpgrw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ilguxtjc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3atqkgwxi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vklrkerh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3lflzazgi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fpvuwosg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bbpkvycp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3wlxzdlay.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mnkoxdgu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jsrrjlet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glqczfyf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rsuwiiqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vptweyju.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gewdrags.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fzmshmhi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyfebgav.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3akktdxfg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3swdjuxzr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gclisidv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3bdkhxnvz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3sgxqrtvo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vppceucl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3conglwah.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ilgpnxrb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzwutbby.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3atcusstu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cjrddqkm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cofglstm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3oumjrbfv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3maccgmdy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qfhqysbh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3lnbqxurz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hmzsjqbq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ebgcrjqc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vqnpiagi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3butbklof.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mogplbvp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vvdylmut.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3phvylmun.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vkoqmzlz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ocuyruim.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcuglid.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dsfetuvs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sbynaddr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiazkahn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3awggumsq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nybpzdns.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dnxqmiiq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lyuwyilz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vbpgztgj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ulijapht.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zluaeyop.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lrawgiuz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aphtiggj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ghfdqidb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xfjduwpr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lryzlgbc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkfsihge.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gxehlgfs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lsduwrbj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iawzyctg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ntcontxf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3eifmjhqn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbyfcjok.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dlbixsuc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ylboekmr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbxnkvtp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bpjljstf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qizjgssc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwscamf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jgvblowi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsghnmdn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hsezbqwv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nfsxzipe.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tvoacqxs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oppwgmni.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uwovyyxa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jcyakyxx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jyfaakcw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zueufjay.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ysadovfg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ceatxohb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3awrebcjh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cnitwhyd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bmwyupdh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jrmntcuv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jgmpdhua.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rxglbkco.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3blwnkkky.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dayqjtze.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggyxpuax.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yynnqetb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ymvaermd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3flfzaopq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3sfdmjpsn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3bbdtztxy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtiblfsu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kumnmync.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wwgyearw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3toxwbrsg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lalagajk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3khkzdums.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pzzhodkk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kqxkpulh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yewdukvb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fttfabfq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aeuquqzj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bosqucuf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xwduyscg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3guhczyzx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vzvtalxw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rlklhxel.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rpbpccnm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vjcnoqbe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jhbyzswo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dldmmiiu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fxnyzxko.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ivdetejd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjuexxhn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nwunehge.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xehfovie.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cgohvkqo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pyrnnepq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nywublxg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iqzmtmnv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ayjejfho.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kfisfxqf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dizcicxq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3khzwlhfn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3cxskzoxg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mdfsmplz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fcnylhly.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jyybsatl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvgmbxd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ncvcwfhd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ozsecyqn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kyzhysxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pjqgrrmz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhrjarpk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3khrdwxqe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mdpyekla.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mspmrpod.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kkfzwjeb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ejgndmhg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qagmliea.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jgwkkccr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rvaandem.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3erqftxol.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3harydcza.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sfqxwtou.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmgosqvg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nsynkmzx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sxbuiooh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ftqeiork.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yatyftsm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3drowerli.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3njfjotjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skkfacsk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dwyovcmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnyfpupu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ivlapzcs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zyrkgfyu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3txddrkyy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gqcgwwnn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ethmnpxg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jdyqsagb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yxcijbae.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3azhixouj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jbqqralo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzpkrpok.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hrztqubh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3texrhkmx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3khhmpbwo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eihdyuvj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xcfpjxsy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vbknhnfi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zvktwphd.html


<!-- 参考信息 -->