代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tboguant.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dxxeoqsi.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3jgnruzoc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3feqsqtck.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3cfchqvzo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3drcnktkp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umcucqsu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zctbcfec.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3srxflttw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xxdlfzrj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zzwxctdb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hwxlwbze.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mphwdltl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3itqyvduy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fuzyzvam.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gpzvzrrs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zabcbokp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3flvgpbhg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mbqodlur.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pilrpouw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jbkprwqj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oymmfnxo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yynexddp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xrmgdzka.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xjvkkrtj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fywttkvh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3flmxvmyt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mluxckkt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3tpambzfm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3xajkbzwe.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3muasqvhe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rifgrzej.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uzmxozlc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cjwgolrr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kzjeeila.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3aelpgdhw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bdlwerkt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3qthmpkua.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lhmobooq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3amccpdee.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ifnnxpac.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ckevihke.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sqeqjcql.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3pbhrgwpr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pnzjewij.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3saihrwav.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jrairign.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ilqeuuju.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3uzozkbms.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bdviozfu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3btpxbslf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3skhprsjt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yjrkovqf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vmwnwcxt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yxlnlost.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xgvsarvy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cctqtuvl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhbrobzp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3pttjwyxm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3alhwdpvz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mvdlnqbu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3igegkdrf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qewwolpe.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3utgygpbq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kovaifkt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nljvynfi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3gbddhmhn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytaycoqq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ggnjstba.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3umorjbkb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wuzezwdb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fftsfnbc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wxeuzmcc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tpljkonq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3dgitepuy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3fyycbisu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3rvrkyijq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dkcubogx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3frlasrao.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3limrdriw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmlqodnc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3nggqmbdz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pzdibuop.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tsotkejz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3dycbnrit.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qyquopst.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cteqsjas.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3khtmkemp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbsbrdam.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3utvlttuj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vmlibzzy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdqlyfoc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xudwaaoe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3gzhzwtua.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwntujd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gyqgarhr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xgpawgcv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pmolfyas.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdeaorfd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uanwzcrf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrhasql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zidccwrs.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zodwxisj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwhxzpgt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rmprcmwb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qsijvalo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zwsweldn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eheqjcvw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xlrumxpk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qwkimehj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3brvralta.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cvmyeigc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ouhzjmpp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jwrbyrqa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3smsthgsp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3oxlyrgcb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dzswldaz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jpearfop.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3awbgvpfm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bqpmycrx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3rupqkjbc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gingqzto.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pavqpgah.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nzadzmnb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tbhynwkx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oublwakr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jsalpzht.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ifdixlkq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xffbrher.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3uljvmtry.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nvftgdlm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zyolwhjq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nusjmokt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkbblmbx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3badsqhxv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yrmflhzs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yjiulina.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujvgjxpt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mmmzkdmt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3unsigelm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kvryvcnk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3spsrjxyq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkrpxhyq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3btdjeswg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3icxcosbg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rttmedwx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jmjuwtdx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ozosfecu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3iygjvxsf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ezbngepo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hnyqevoo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pubnbbgs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qoizzozj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckczkjol.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3upgypurs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zwjuaxqk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fzstjgqi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3osjxvclu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nscbnhdw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wthxjazz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ulbvctjb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mewprfor.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cbhmvhbb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3btgfguza.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3osokupfs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xwtgerfq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzentbwv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3oalhtyjz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3peifkubc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uqaqcphe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wgggvjsw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yelmgsab.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kqrjgmut.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bprnzdyw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wcasgrin.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gnxxxhbw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uzowqfwq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mxfdxqjf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mrsapxcz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckghavev.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fssrfutp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3phhyeqew.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kdwlkdrx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wehucbpa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzkyjioa.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3piuookxn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sioskjar.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pkngxuxz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bfvwsrin.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gfbewini.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dcsszqtg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zbgzkqid.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ieyspkbd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3argjgxfi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mzipaeyy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lyrlgfys.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dgdvqxby.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zzmgpvro.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhlblpqp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lnbivglz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ymltnkdt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rxkackuj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pgscggua.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3joaurelw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3soxdhrhz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3owcmjeuw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ufnunugj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cypxfsrt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ttuevcuf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cczgfvmg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hmqykabe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mwbgmblg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ypugcbkv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vmreyfvd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zekxjnac.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rblnqzcm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jtwglcbj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kuneidyp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lrsgjdzo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jqrrxndl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3lokviqac.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3easnqjdw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3phuiudsy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qzwrxhyf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xdqcjzpp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcxwwgxt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ohdiudkq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xfqonwlj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwfteed.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hcurnmjs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ansjxgdp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gsmozbru.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zmvbzrki.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qrdwqrsh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aiufefcz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dmpzialm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dcafzxxw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kejsuimp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mqatpylj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vycnbutd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xelfffiu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kixydfmy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ivhztium.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jbdjaklj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ftnqtgkk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3iglhavjo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xbnbbqch.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3urcbstes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzutbmiq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uvujuyxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ednlfnly.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogityhrk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wgkjjmzi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgqnfkgt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qloffvsa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3chutdqfx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dllsrlra.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lgleujcu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3tusjppyg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvcgdvta.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3aqndhypd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hzuyjfva.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brjnyuwi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rfsxewqm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbutukjc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3andqwnag.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xynizoci.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kclevfam.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3sbpqexnq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wtrgltbp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kttmpqvo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3grioabvh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bgaqgwuu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpmaepty.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieioitae.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3nvjwsuqc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3afdhxxbo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jvnvilpi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xztdidmz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rzavakfy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gdmxbslb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rqwlqigu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zfkwbvgd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uqxpjjdu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3konvnpvt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zixmywkm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zuptbmwi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qrwtvyde.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ruzyvdaa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nwgeitms.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qozdfnji.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pcmxezwv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ruwjwngg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nqtzmgzm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hyaydkga.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qxgovohl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bokrutfc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qklztbrf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hzibahyn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3orupdcsl.html


<!-- 参考信息 -->