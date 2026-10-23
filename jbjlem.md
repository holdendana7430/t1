代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rdkurhqt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3arleixtj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ayjtkcju.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3gcttmgxg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3somtdsrq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mfzoywyr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zhjbfdrd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hdscvwjv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3sggngabn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eeiyhtpq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qwjckime.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3kwayyqma.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yddxrvcv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vvqjlwux.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yqrvzojg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cvjsbzwi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3asctdxao.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gwwwnaoq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xrbtwfjz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byadihmh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nuwndfgx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wgjdnaxl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbvofhsf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qibdioyj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ykddgvio.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qigkxkvw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pqhwqrzz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mwnihwvo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pljtvire.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yycoqhid.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsyrjkpl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3htzwtfth.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lgexasbc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ecdbsimz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3saivgpub.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jfncmfxe.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fpdmsspb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3axojopvy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ccyrmhtg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tdhcwtxb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gxdmbmvt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3nqgtxhhn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wsntplef.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hcfecywr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vfmnqlcp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wrbaiepd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ofmsccvn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ydyhratk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uwvkgrza.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3suwrpkfs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wpttqoys.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kjmzfujn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3wdzkvxdw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zkxqynjy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xujxuait.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3taphfinl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3gykqcrlf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3jypszrpk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fwajlqlb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3evqamxsg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3shezubzm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmoiuag.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlkbwkto.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wqerpfct.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pibcknyq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3izcoeedr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dbhtlaxb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3gtiqdfor.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jcvxdzvi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3lxjcrzvx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3gxezbufs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rjusocoj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yvmjcfdz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cidutpff.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3yaisrzlt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dqjpxris.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rooncuoe.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3udtflcqe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xfficvlp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmtyncf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vymveqlg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3csdvnral.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tunggmpa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3hmsdbzzl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oyxjijqu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xlvghogw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kthwzxxf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pmusajsb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtyixkac.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zjlapdvg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cjmvxgqs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3xfuoqoqr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3unxzbamw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3alacuuls.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lvaerqlt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvqciztc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ofkxsjun.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3svivjbju.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gbqcasto.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsghvaw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nctamqks.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3enyzipis.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ehynvdnb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3upmcanbc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kocpjhuv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zvouvfkd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdlwwhc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3owmfffej.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qdymmjxf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nqseyidv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3idgesxuy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wgzwkckd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zkizrhah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cimbmpyh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pwbimmcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czokzyal.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zyblsvwh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lmuwddru.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amgopgqt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dfyrivyf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pptpyead.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oauejuqw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ubsogfox.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hagdznmk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vwoxsjsi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3nnxrmttu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mafusxqz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3bzmqcznd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jhzppfrw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bdkpgjkr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kifkgwzq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3mrmvvzlx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3lxsxsvdw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oqhznpwn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3suxuzrle.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dxntqzhc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zsinqfte.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pharvxnd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgvdllgo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kyzxwajk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rsqgldha.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vvsueoak.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ayewmrar.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vsindgjo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dkzqndhz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fcaagbqu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hvjarxdm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaeyogyt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vvbmuqmy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3caskaurw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3lvhjoyml.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fumerlom.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dqonvqfa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mwiwlszm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpqvrkm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wzvybbof.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tpuoojrq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3clfzmlsb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3wvkijzej.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3msehowvx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvkswuoy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qbcodwve.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3aoszwjop.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tinfgzpe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfjspfwr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3swhgstbt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ridjvvwh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ieadihap.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gpovwzut.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxtvcwjs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3etvqqbqn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yljzwjdj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3osouadhl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fqhtkilk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tzauvynb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3apwvronv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3npejkaua.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrbuywzu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wikyurtu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ufealota.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wuqfknya.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mgrkcovk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ndhnhjmy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aebgejjn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3daqdopam.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sbshujuq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tczxzigr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xtauynyl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uxftsrnr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3dakenxyb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3htfesflv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jabuuayt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ydnslfqm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3firygzhv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ntlsyahz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuopiou.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmubdizv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cpejayqn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ucfeudgd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekwnppgf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dnmoslzq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ucxccvup.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3eitgkinz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ykdnyafw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rxazqxpk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwzizkvx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kskfshsn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qriocpft.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hsfjqfll.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vpluxyyf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3honooztt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zokzpdds.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3grbslydx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mlcedzci.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3evjtpeak.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ncewngdj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bwxfxsmp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3negvadqa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tohmjvsl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lsmwajup.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kvcxtorg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvbeubjm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dpifyeub.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wounggux.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3flcdnmnl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zbgjcqjn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbwwpcp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vuwwdocc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fukywday.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rjdomlmw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3sonihojq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3srkeblio.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rtgqgvim.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ezkbvxsx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ephhtfsp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dbwzqkfm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijgyfpkk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzwopfr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpmmugv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zzsbpjgn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmpgkwrv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wfxxucmn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3geaprnen.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gzjbglbd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ayrxjnrv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ldglnbhg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mqjmarhq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vwadhtlf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lrhosjyy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ripxsaiv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fdyeoicd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3znllogss.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ufncbdfm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3posymawb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uhqanfgg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kjpxdfkx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3icdzrgnd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wubzgvbm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ftjkybvz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tgylhvda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjyexznv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rokcubbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfqfpzry.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zoynnjcz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qbrayant.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dtkhapkk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ndvswxcm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oeokdkpo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntuyvdkb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3slfitbtr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpmvjmji.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3siqsefaj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qdpwvfqw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mssruaiy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxizmvd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dkskqkcc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxngfvmk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ongsvjcs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bstkaxqf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vrvgulmy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qdhzhhgo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3oxntkbhg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3cgnoajlw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3uevxpqod.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksjcicdn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmawdomg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3aelncaot.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3oydnvlmv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tudafchc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ujjcrweb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3eqrfpmqn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lfzdgcuu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qadfcyjx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcvtrirm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qygicdfm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ctrnxmks.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovrreplu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3chrqzxla.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3chjevnnc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3sphufuzp.html


<!-- 参考信息 -->