代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iuoqlffe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dxkhuuap.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bpsttkni.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3xbqoigqa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cpvebdrm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3srmoxiah.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3btkcbuis.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ldbkvatt.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ognksjln.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3djyhkmwu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vkzsycdw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3gacqhkzi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rhiaynxo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gzetdfqx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3clflbrrj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xnxqwsfn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3keypcjaw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3gerhevay.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvlfbalv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmtshzif.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ypazggvh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wseusqbw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aebekzkq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3jbrjtopm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ebkchsnl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gboemfcu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cmgrpttk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cjkylzmd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gnssojih.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ckzgseda.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ohcxijvk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jqgxxbch.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3sbajptpc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xbyaphoe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rktotbym.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nimtginr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cteoneyt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3lzarfxdb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3njyviouu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3uvlxpude.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3xydhjisg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jmlwfalx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kuowounu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3unkxtjeu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fblchcbd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tnkggdlm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dfgkoxrw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vvucqgvh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ewywjdnm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cotdrkhq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3cvirjxoz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3eoqjlpmi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3xaicssix.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xipbanut.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3cclxavez.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jwyiwazc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3arhbxkbg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3avepujsd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xmmzllsf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3oqkqisuz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dpmaemht.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gfzksjpk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwnyvki.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qctdzmco.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xrrvbfze.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wphpidbn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rerknqmj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3dvvtnigo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rilfsren.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vazzacop.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3fzoubgjd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mrgvsnnz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jvyjvxgl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lbwyrjlc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmyoxfcy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3eqcjvnvk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rlinvruk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3azzofget.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xrxmhcai.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3aacryhky.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cwgnqpcu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bimclluq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iplakebz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3vwdufwub.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xtntgqso.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lwiirlet.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xnfloacg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pvhndjrl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3scdgfuqc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3blpuzryq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3amzsctvy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3thwktlhu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3eshcnmke.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xjevyyih.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xhmxansz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zmgzqnrg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xfouovhj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3euphluln.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkcicgdq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sxqmvsll.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iksrkjxq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jdnmnwvz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3yafykfcv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3osulfyxc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hzdupufy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3lsexjvjs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3uawdgcpg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xogstwll.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3lihtlqrf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qbuthflk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hpsuwjmr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3muvwktdi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kfapszzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckkxadmb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3upkyfapu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmnifawy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3sowlbmrn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3byhfumph.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3oxkqnjyt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vvdaazpw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3paaeebyi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bnepyuwn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mrpljqhe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qruhvicj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pbfhhrwa.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ywdrdwft.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3awmbgbmf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3yjnxttsf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jyfkxymg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eynfxczm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yuqibxcj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3afbkdoyo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jymeffqx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zyhuglzy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ixmimtli.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3anhykseo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgnodefc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3povumcbs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vlqdhdnz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mrxstkqa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3edpolvfj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lstmdwrn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ygepxeiv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yiztvniv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3frcfwmtc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkzdwxtv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zbkwxumr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fmveeejw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeuuyede.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lepeysre.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pqujtvdk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bdaiepdq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rgocvagr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3edlecwlb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybfvjnng.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlvlkpgz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bfyajnwd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kousfsxi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dnadgxhh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hvmsyfbe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lejblfcf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zgonmlrx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzibgjt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xibaksnd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcljmpiq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fspqaqec.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyhgsxvd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jkcbidgz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ubuqwnqc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdtomsfo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3iyduhwtw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3egpiaaxu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gczwqkvm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fhmgzwlg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tkyxisfl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3libbgcce.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3eyrlpzqe.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcxojkzr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fxgcmpkz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3aiaxkqot.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vguboxhm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3grwnkqjz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ofxsiqmg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bqgvpzmz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rcwymyvi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lahgmhhp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rvlkuouw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpxcrogc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zfhhjslw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3unkcqrtu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fpnebzpg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ndkydvcz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3shtxtgxx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3buccrisy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fdtscywd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ixgukyvi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozoannwt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3kwnrwndq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hlukxcwq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3iqksjmzh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3akayrktx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ygephtja.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3prbbdnlm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qulzdree.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3evofcurx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3spdrhper.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qniokiwv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yklnziau.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pzjjbrde.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fdinpyrg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gmyqnofi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aydnhbow.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wzuiyypm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3fbkjbjss.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3syeguphi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hwvelajz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3kficwwfa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kkegctme.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xiicvmnz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3upnfufor.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aghqdvcr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yiaepltl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kescuhdk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zifosjyk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tenrlnmo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hprarlvj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tlwybfdz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mxfpmayq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lojcekwu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xiowwglw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vxsffucw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fjigucei.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ckungnvd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xjvjnbyr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xtomsxzd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ckjywstt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3thvpamyz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mrmtbshp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygdbceld.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hdxtrnkp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucsmneds.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nptywxrj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lvlslniw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3eslmtkxw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zapiigkk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qejhspdv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cmrxmeje.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jchxxouh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xheaglnl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hbizriiq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ydagccuf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zmxcttfm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tybzclcc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hkjcctwv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kxzaiwpt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gktadwbj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3grtivldo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qulcutnj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uxavztki.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rxarnmlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atxaqync.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3sfzqzgxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwojjieh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aemiwvpr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ftcxrtfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mknugpfw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbmvqcka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hitlotxg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvhtxptk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nessdiuh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yzdfvsiz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgstmrzo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xejkvlbp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ubdkudnz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tbavkxpd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lifquyut.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtzicqqx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bcrvtyfg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eudncnif.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pggiecwx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3urejoccq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jvcxyvre.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qrexltkz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hkyahjjc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmpdrvrj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojouwsuj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyxfuxsy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ofrvijlu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihtiwdaj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ggvcoeot.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfqsnydy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmkyuah.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3cyrkvxzn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hicfsuwg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3idvomzpm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pifsidvi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ombsxexa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3umhuhbxd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nkbohwpl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3bgczwwbb.html


<!-- 参考信息 -->