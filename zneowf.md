代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3riyfuxlq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3licfrrbh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mjyqxrpq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nbkinrzo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3renonlla.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3gjcascmp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pinjxwfg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3vcevaakx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kygjjwmd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cljxuqpn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bultomrp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3djzongrc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kqakulwc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rfqpwgmq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lclyjfbp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3wcesukfm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jizshlri.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pwoofmxs.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ftcjewaz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dxrljmbe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eayybukl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3sebzgezv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrjsntfw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqbytgbt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3yiycdpjy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ioyjjrzl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3talfsywv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ohzymzch.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uwudxfmh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uvmehrjd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aznnznye.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3brpjgtko.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cuuqpztj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vmlnudfp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rtrhpoet.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3drcjvbwm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rnedhozs.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3auceqlwt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnmylpv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bomojqke.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgkhcqf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wswlhclk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3goytsdxg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fxeqvzaf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3sfiqbyxc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tkhofnck.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aegxwnvp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qpwbsmgf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3keohrvmh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qnnofugw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3oioxzwmb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gjqqblgr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cjubrnki.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3btazokbc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qswqoxwf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vzdfkpig.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3splnyzzz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mfqrebsd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xqvvhtif.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ouqytlzu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ltetcwzv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hlkterua.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3rvnawifk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vtzdjiwv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3swcjoinj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qquppnub.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wtxdptzv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3afpypwle.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nfepuwcq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bcdgczsu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwfdgkf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3anhdgegy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kadgifmx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3bqwktyux.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3adjvghqn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ydshapqk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3bjiqomtf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vvfbidfr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gautocgp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3dmecapjm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bxyzeqde.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ubhrhhim.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ferujwkx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmyeslxg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zrxpjxhm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3awkluebg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xqinqhmg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vhkhylls.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ozjruzif.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3esvxntct.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zqlkkfrs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3orzhtkml.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3nneapiyw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rqeiupmm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uewhsyjz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kxndxstw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zouqkgfa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jromcqix.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3okfskuan.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3roviqvrv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yxphduoz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hohgghvt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3moavzdzp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhzutvkt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dazmoixc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bhxfvnbg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3dqpwxwbc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mvbhwpxy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kdhjhawi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ayvdhpvp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wdopfhwx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3tomhhtzq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3aukncmkv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vovzwgqv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ptszdnda.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pulozpvh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nkygeuuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjhyrpax.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3eobmsiil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bduoivxq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xgxhfehz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qqcadewr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wnseibtu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vuafinfn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mhvncgju.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pvyhaxfe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3grprmohz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mlbxcsvq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xjmlqaoc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3mreuvcpz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vhoingkd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3jglxsthg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pkwyxuji.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mwzfkyyk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jhfshrgg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jywxvkru.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jmbxncww.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3neauijdx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3titmfzxd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hodinxwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uwufzvkx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qftgsmmf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3opcfrgsk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wqpxrwam.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cvwzegvj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fnxmnbfq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yovqkcly.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugofobsu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uwmaqvls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzvoktgp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cvclipoz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oltfqmdk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwpzfnnu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3snpjqdih.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wagkxbgn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nwiiefyt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yzqeymdj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ywnqbjoz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qpmwrjlc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gipidfmp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bnhnpucs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ohgroowx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ntkgkiod.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hgvyughs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hiigifsr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tnqulofo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ghnthvre.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ofhkgcpc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mftyiszt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnqvzgsp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3yqruntad.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3udwhjhcv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xsasurpy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghwxxfvs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijlqtysn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dznynfdj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3htugeqwd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyhnskka.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iqngkyze.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdftudir.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jjhywftk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3glvrvizh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jexqvobn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wnbdzoxo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jbhkxrma.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yjjknolc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qhtulksp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3elmaavrl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3duzqnbmm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tenswuhg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3nzjncgac.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nftqpblf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gsmxcepc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ismeqgdu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnpzttgz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3owfqdxpf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlrtnnay.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bsbevjta.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ribvbsyn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3szryulms.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrqjpxjt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qqmnrpow.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3yamjpucl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3guvieosq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jnupcygj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nvrgumqp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ailfyifc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujnhxasl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vuueahbz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dnyxqiqi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cnqjihxi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jqrioxlt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kuuqgyro.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zlxpltye.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wjcmyuhw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3tghuasyr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mnieedhr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3auzjjdff.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cdonkaod.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3huwvdoii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qftgeshq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rpfaceio.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jaagpsal.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnyryfv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rmxqwyik.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3avcnbgnf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rhjxjytf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lzxjexip.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tujlidpf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rpnqkwxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zyuzqoey.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eklvgonm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uofblavc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3svzqbtiy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xuyjabqk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3odwzkruc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gkgdkmpr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pkblfwyn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3usuvynhf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gbedvoss.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3spuzfvqf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3stuepbgv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hjxetwsg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zrtasscn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3srwnszrc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ltbfqibd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3hmhihxsb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3voanxngz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3nyvagqps.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mmnvsaik.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sqrwtgzp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3exydxbya.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vbpabneg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wcjfgziz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zdsuljkq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jqfcllhq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vwtrlpqk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wkaezgoq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lbrkasak.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gomxysbc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lukswcqv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ymnynund.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lzmlboql.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nvylksem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcejkizl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3esuzrcmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiwnaorn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3onjtepfr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3rqhvagqp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3snipadjs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ekdkqjme.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yhoxletx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzcsmwcq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tpyvnjhj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vfdvqdsw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqzmgizx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ymxlezar.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kfdojpca.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhmfnfpy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aveggcfx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ljsynaou.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hjpukkhx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfiibfdb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jmjnrjpy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cjwbfnks.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tyxcrqsd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzgkulc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhvipbb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kzeseomb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tthvmsxc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hihbhotd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kqbrwpuh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ooslevvq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3capvasuh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrqtpjsi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntaamgkj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvurnanx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3skadhikx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ygmmefnk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wyseuovs.html


<!-- 参考信息 -->