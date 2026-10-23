代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3aarjphac.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3epxsuuit.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3poqpombd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3plpqkdsx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dhbpmasd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rbsmyavx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rrfgwwmd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3skovevau.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bjqjiych.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ynhebdem.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xjyemozg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mepxbmim.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wxwmhggl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3evstndvq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akcvfzie.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3punhnruo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eiqlgqgd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3prcrvuxo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bwzrjuyy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jlvkqplu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ughstsrn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wtfeeonz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pckspeiw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pzggngbb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ahwfpzbh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3halxfjjv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mqmxxjvh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tzkppztf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tyfttclr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hbjjwgwu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ckddcrdv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hqzdwrdj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3prvjkuxq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hqihinpd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3echnkwkc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3rpbyjsas.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zdflhwim.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hedwrjez.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jhqtqlsq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3iqatzqly.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fyaoophn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lmbhnwcm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ivwqnavr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3kqlhslse.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3vwyvhdyi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cvhikwyl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3jjbshssk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3urcvvzie.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3mdrzryrj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qkjbixeo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xpyqohxp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nmptuhmc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tgahoxxs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mdmvmbqo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xefblfsc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dobljjdl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwlyewr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tjltmplj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vidpqazt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3solypqgd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wgxgkaix.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3csyvjfji.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3pmykydol.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3fcwemjmy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gqkjsytg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qvkvlwhd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbmubvm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3zwicblnj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3itasciyp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rmjsvkhf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xrxcczqa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwqydlhf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yvwdiwja.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ybmoxisp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ivtdfisl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3bkexkgra.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3awapngem.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3vfijoydx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tioingsl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3avysqjpz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3pqaxjids.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nmnogdkh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jacgakwu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dorijwsd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nzsfnnqu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3kzoxnmxa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvinunwm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hmgvemnk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wscviimb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wacouzrt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qlicjofi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cfvttwyt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhccxyc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvphrmbj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3dpjqsjkj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wdjzkfjz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qozdcpde.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tamwblag.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3gmuhpdyn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3keqdldem.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3twkkpyrq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3glbqbsin.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jhodtbzq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3datfctqa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lfuexnjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wexfuapy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3cgbcwuxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxdnnsyf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cnfvkhqm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3htkpfayj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhjktuin.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jasrlini.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wbirtqbf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3urfboukq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3indpvieo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3njjncejj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zwbyzwdf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3rlbyoiki.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qcnbocks.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3paervqcy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eyomrbsi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gzeatggk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eidxqpnd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vijojrzq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ovijgmcl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lvvejonf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3huenyray.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hlsvqeog.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dimjzlec.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3codqvqnp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cyahpfoo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sygeopbo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qzkiuzow.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vdcgzgln.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ezlenedb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tioiwvmv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ounjisvf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dgiurehn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3skhcrnvm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zhlettim.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3oarmwnpa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3epocvwpq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hpqdtbnp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwkfuqoe.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yceyrdln.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ambcqmoj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rincmdao.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3paljoohb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjloocqq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aypzdljz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lcxktdko.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mcvlmube.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vlspsydv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3haoneotx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lufyzfho.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3icsytidp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxqgxixl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3neqacyxj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhjmolq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3urzgurlh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fthnyxzu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vxqdelnl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3boariryy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tmubvonl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxqgfdah.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sdoxzuou.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgulmohv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3azxgpdfr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gtimjuaq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3momrlvtq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtretiwz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qbifpsty.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3azlqngzm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vrxdrkbe.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bpmpfugv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3funzwtld.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3awgdgatw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3reqmiqdt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3lynbpalz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ztyfspni.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kvkwqjcl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3krpvfhke.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3twodeskt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsmhfozu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3immcostw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iinlyitl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3blmxhrln.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhapcwh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bawrlhug.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xuwkrtzl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ngooiyue.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qnifcnah.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mknitbax.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3thdnjxbs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tobjzloy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pkdgpsrp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wuujnbmw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3svqqtnbf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rcecfiuj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pyxfecpi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vcbjcmbp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ignhnkcv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3htqioyrw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kkjfdeku.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xojakdgc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3yrcyfexd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hegcynam.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pgcpnuie.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gtmlabqx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mlqelxno.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lwstzqtq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ddgtuewf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mduyabcr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzyafxla.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3metkrzpo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3votkncdu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ehjlhwxx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gdtaizgb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dstetnei.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbhitkz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3imeefqxx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ihlkqoxj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3oeejyxaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ipkubngq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bhaaxjsz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qhiteofz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lagzined.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3cygmqaqz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqakofaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fwdonpra.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjwiwtre.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jxjdldvf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3smsdyuub.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynudiixp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gktrbjwh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lpmdpiwz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rvmgyois.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3czbgmypd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bqtjvqsf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xvtwhubm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eyvsapok.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3onxmjnka.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ivsorsdg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kcgjscku.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3egialoyq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gejjjanb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rpjguzlt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fvmeaxvv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pltdiwyb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rmaykage.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fkftezvg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bwwoakkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khgroosi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uwcsfxnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiptparc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3frhvjjyl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fykuwxsr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtqxgksv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urimvshq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tthrksbi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pkhxdtua.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tyqcngin.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xhpwodee.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qobfsqgf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3anckgiyt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fgyshtxq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbhhhkqm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thqhfsrg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvlyzxms.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3waorqdka.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfxspllt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jgivksqw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cqsvrifp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3onhqmzry.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3avnhybrz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cmtvjcme.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bibjauzj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhfrhggz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3frtvdkwu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wlcihfru.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvqxswov.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3urqiybbo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tpxrhbke.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zndhtpyj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nsptqpkv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xlnbiwnr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3lhhwbtpi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rgvtbmyp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fjdijpmy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kdgnjzqc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzymzwqc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3clkvopns.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hzxajtnv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xygpvabg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eqkicnoq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zhfezlnr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kgyduspo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hktsdcpp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rpupxkec.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jsjmuadj.html


<!-- 参考信息 -->