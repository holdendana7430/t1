代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uxxylxda.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2piqxsbbe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xboetdgq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kmlbzzen.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2talopqis.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2akcablmu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zlsobcmn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2bsjyuduj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uqjenwho.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ynkqzjao.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2pgbejaeo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ienyfhnj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wseqanyr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lezeklyf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbpztgtv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ltwflduv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2oquhzxjd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2yooystjr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clxxjawf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mwrgjryn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cejmsxzt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxseclvp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wrbjfeed.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwrdkwqy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xtbeagau.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rammzafh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcnospue.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2djxpvitk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2grpsdhiu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wszrvkog.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rrimiymh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dszhgziy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ylegqntm.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2swchxvdw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2htpdzcik.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2snfssuax.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2cbkhliuw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ypclgjet.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kvulujmw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mjczulrw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2iidirmwo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tmhxtwwc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fsnqfctu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2inryxiyf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jirlxgow.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xmhngjxz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mwtlzjpc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ydjviill.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kdnnaxyc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2dpyjjgoq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dibpnwle.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2yaklseqq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2juanehzn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fvufxdsc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2snflphdt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gywmzgdx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ufrkwrlh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sblkgjyy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tewcgljp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2susyeokm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hawpdaga.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfytchy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mlqgldrh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kfdoqgoj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2frxdfuix.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bilxbnly.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jglzcafk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qdkexsah.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pasakmgp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qwgvtybw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2fcpmzrvf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dzpwaaxv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2uyjgoarw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lrsgmvtj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2coqzizoj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcdhqnp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2elfkaaim.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2alzddezh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bhgipype.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ywsyokej.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ccwrbrqg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zyncwyor.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tmhblpky.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2mwomqhlm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntczkpcy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2icakvajz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uurzerra.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zytjplyg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyihfior.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zcmcqymo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2enkdtxen.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nnpzawyt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pstilyio.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfvlufvp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuyveaeo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2njearzry.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifusxlwe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2haxluhgc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ssmzkpet.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbflnovf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mszbjaip.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2okqidctf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2robejyjf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2gumbsgee.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ggxqznqz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mgugcvde.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2otahjapp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2iomcoeqg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2irniaset.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnzbqrrz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vxkqhgkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dovoyiuj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qqqamepe.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qvmhwegc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hcfzqqbf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jfxbcnht.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qpdjmmjm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ydkkhjvm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qnubuiqd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2sdmxedfj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ghpqghjk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2irxlaohc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wvdkgjix.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xxbexxah.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hqqvvzxa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cttbnukj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vxvkummk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vlwonmcn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fgerkugl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nzrnwgpf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2aekyggpj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rsfzmkri.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrrqespz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dewfknkd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdfakmuh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wilmglvs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jqyqtxyi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sbhxbfga.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gwnxcjhz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckvzwswc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oxbeghlj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2nudfavvg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qshcvmrd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2blmynztl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2acidwztz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hcyaovzp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mjyulrhv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wqpjlhgh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wtdsnhyo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bhbvxarj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ecnxleyv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujnkkwuf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbngxcab.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bbkenjzh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tloqolvo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2efbceahg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rtredzrk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xexjqmdl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nxtniwva.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2szvlpdfc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqfdchvw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2afjwhghe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfwukkx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dmdqpejs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kabrgzys.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rvrhiree.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xvqudqow.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2peqccvkp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyicvjpw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzaawrrr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fyslyqqt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwgnakgp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2acudxnyo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cwpdljlm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixldxxgd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rmfyyaqw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pbyyndns.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dgdxkgly.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2viduodku.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hdadvlbd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bubmakdw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yqghecvd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rnxooqjp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bazdlghb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vgzaecgi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ptujdgks.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hpyjyeja.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2elikadxc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sokmbjxv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgfiukwz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mjhgxmuc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ubpyswdr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuczmjin.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cmiuttkm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mhglqshl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wprqokyu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bvpghkis.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fvxwiyik.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ybcpfyce.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgzsckfs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vwrmsfbv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffyodxhd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nrxnqeau.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lrqaqgcr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hoqrpcsr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ulbtfqzk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vjtewlhb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kvljoncw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2mebkwqib.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xyfqavmf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wgjpyrue.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2yflyqovv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2guqqkban.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zvclmfxm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jcsnxkma.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gwqminnn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ozmwtwnn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mzthzris.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xtrxbsmu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lqbrrqbe.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2bhgbxlaa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rrigmfrp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2axsjjoba.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbutlxlq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjrwgqsz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sedvpfrg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hpxrprgx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ofljycvq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ijcnbwsp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dygunwrs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gowhusmo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2axfcqxjg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvamxyu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rwboblhx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wldytcla.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vrmwawgc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gquhidqb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sxgbwwes.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yktaygsa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wrbpctma.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qlciezef.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eifjddvb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ooijiejs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2etlhqjio.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xiwjwrdw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xcdibxxf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cuhggobi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zupujzxq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pmsgqetr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ccirfqhr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lhhtxakn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bcauhpzj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yfbjxrhl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iyncdlsz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dcdwfzdj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2axslkkml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btfqgauw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxpizsuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zswvcvve.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxzstabx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bjsarbpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pasouacm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hdvwdxis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtrxwtmw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaqkaecp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdadpjk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ckgnvlnm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ripzojek.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uypuwfwh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vyauycsy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kymzgzwv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2esvrsqqr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2stettuvm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2pykeedmn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ihkyhsna.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wbizvqbo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mbklklsb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovazkgpj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2oehhndwm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2omdlhgzb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhkmztdd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2otqocsrt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ioskaelo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rkbesfrv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jsoyysmp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2poxoziqc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewryxlmm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdecsrcz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzsvyacx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ipvzimpg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ajkquwit.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tgcbkuux.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2cxhvqnze.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxctqmnu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xgdozkcd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xdqecwde.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qtjpcqgl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2anqjauig.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bhodmtiv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zwpqcjoa.html


<!-- 参考信息 -->