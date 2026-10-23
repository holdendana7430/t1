代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wehqjbrj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pufeiclu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hzfutzrk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ybfnyhgt.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cemoxqgq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eemmkriz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3seywajqr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zlqmwkxq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dmewonua.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tdjrznts.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3uznhzvon.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3auxfrxmz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dvdopiek.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3fudlszfb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ycvsjiiu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qecqznvu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3phkqsglx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bgfystqo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivooawko.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ubyskbqs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rcxxrlhj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3owwriqfr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vpnuxzov.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qojjigib.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbjpbnib.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltfoqekx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxhiboys.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vhwddtlq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3gxbprmdb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pvjkkfyo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3emwmjtsn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tuabtluj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtaxqya.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3bjtxitrd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wnbwijzl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vpijkmbv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3wfuaoqch.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3stlphkkd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tkdjiewj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ejoyccmp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3izbtwrbi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mzkgbplm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mroidont.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zfhfzmpb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zuhipcpv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3xunnbsvn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wdtopbce.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3rnvrypzm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3tzrnvlub.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3nrdpdueu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jqowxdkf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3opoagygn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qpvotvhb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rsalgujm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3hdnejddw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lwruvyeo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3estblhcl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vieawgrj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxhvwezn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmgnzyh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmnhtip.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hfltgecg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gqhpetmh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xzbogwey.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ommroclj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3iwpfvhjk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hihxxelj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3tuvsohnt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxdorj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zvtgtozn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jefzjcik.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gazxbzov.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3tqrmzadt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jicbglmz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zphlhuua.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cskptqwo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3seqvemsk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lnwhntjr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wycgpnrx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wygclbhr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wbcluvab.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xsksvhmj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3aexbkypf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lwfgnvkn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fdtosnct.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zzyelkwa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gfktyhsz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3inyrrrkf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3aiurrgts.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3phfmqptt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nkijiogb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vvzivqcc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3katcrgyb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3efkchlvy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtexulzg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrzlmqj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wahmthmk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwjjmea.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xprpxkim.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ympuzfvj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3slaeqanp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yqogjxdx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qzrbqdfp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3oivadhlh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3quylhvlk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ejxtmxtr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zgruxfpv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zlistqvb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lffdzvyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkyqcvgb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3gflknnal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wazndton.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3faiaytqz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3omhkdapj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zscfqada.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iupogabv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gaduexuh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dzmgxbkj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wjmbxqoq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xbnogmsb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nvhictdt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pnrhfcxb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ucwfjazj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3igarxogp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3elefmeok.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jzdaplfw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gwljgylg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nnptsfdh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3skfgecni.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wnwbdfna.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jjyvvatt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jjhqtohn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qtdkmvhd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnquysks.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgclutvb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzpblcys.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kompwujv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3blrkcckn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cesmmlmi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tpebrbrq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3tedocioc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkawypcl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3krdibxdz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvdpzgp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzftxnjp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wddbhrsq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cwttktru.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wwmuwhjl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qyudxkct.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsiisvm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwvrhlbb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3djzmfoll.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gocxlmuq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3njrizzez.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3usazntiv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ccbwsddg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3adirroyl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qdceqpyj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ucbxyftq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wixkzpew.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3inhpgvhh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nyocuxfu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ytahuwgu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3awspgtrn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rixdnrgn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdykrawz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3chckykwk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qnucwzlt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3puxweeqx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nsqbcaoo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3otsdxymk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ofwqmmfe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3swkpqajn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3chdeinew.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bajnizof.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tgfoilgj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3euhnsjfj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fpuvbubq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xkqzbmsa.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lrjuoouc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fivqcand.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tcszfyev.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bezcsmif.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sybtgbrm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3momzylde.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vjlagudq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oasvibnm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zzsvtavm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lrjrcayp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wthjzypn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jqlwgcur.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3anjhbpzw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3crwosjck.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3nozmhbhm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wptdttev.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xnjucvxt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tslvxydg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hbbvwxwv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlczewxy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zdflelhx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3eqtsgrmz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gofuvzhx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ckvtyvjj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gruyyeqs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3uywxnupl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hrdsiaek.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sczmrffk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdohvpoo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pzyflcmi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hmcqvlcd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kufdmcsy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jmqferal.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tomyhflx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qjdgoifk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3blpxgzlt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfrahvsr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iotthcdw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tvbmnxkj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hyoavnlw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3icqjknyn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kljfojco.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vqmfxjpn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vahxnpwf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crqulfqx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gignbcwv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3twkzgumq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3taekzftp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ohyyxxlc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3lytwocqq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3torymgxu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ewdsrjmy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3eprtmqvn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rtbmtikv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mrgxysyq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3baxqopqn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjgyhlvs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gjgisnka.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ursbtffc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3eoimrmzf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ygxlidvr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3enlwvukd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3emfofuzu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dzbbmnoa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ujrbhnof.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vdqhvvwt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jylijina.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ooalzzdh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qzlrocbv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bwvjsiot.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3oumeykuo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3grzztprf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kpbxonmr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ejjbyjyq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hevqneob.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ymojftxo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nyihagcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmvavxgl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uxpatbqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wajuptkq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jyfraxli.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mxpprknw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cqaqhyut.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jyzebswh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvwimkfe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyaxaktw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ixhzbmrd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vsgkjhkx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kvidepau.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ghjgrmhe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qiowcdsn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3surzlktj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ppxqrofo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ncgarlbo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qtghvsfl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3prjhxatj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xmghbgoi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vitqnhjg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ksyaedvi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxrqtpf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3aykyuamd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zukvgvxh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zvhnytwz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjfwmzfq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bsteyzvx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nmikxlnr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wuldrgws.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfbbvptn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dcncvbep.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3sxcsmnbe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tcizfxsh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fgtzqers.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dlkuahem.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rkywzeej.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rzbjbaaf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpcidjfi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3fsotrvth.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gssczfuc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ktsgxjof.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kwsigazb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zedenbky.html


<!-- 参考信息 -->