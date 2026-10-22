代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pacwoijv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xbjxmpvm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rpdimoef.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jgkxkygs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2eqlocxnj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2oamjrryz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jurfxnks.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aviootsm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ikdwxlnp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2bzklwpdc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2syutqujb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2yqzmsxyb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2moiryxhy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tzkfjgwx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hbinhmed.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eigwbpui.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2woqwhgxy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zudjmmah.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tbzbtixq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rhiysetm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jqwteiob.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2faiyszvx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2adrsrzar.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sxeewivc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rtxpwpjo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xyrjbxka.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ibjoxhdk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptmyaxea.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2lhxibgzh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dzminsjr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rdmzbipn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2djtxzcyq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xuimxhtp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2coycxzjn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymonight.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2onwtxzpr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wxjpbjjr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2parxqqzu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zqepbtjf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rypnuzhx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2auqrjrbz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2oachblvi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ldppfskk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zejvqyhl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qqizvdpy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pvlntmdv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ndjfphzz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ynejxxvm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2byellley.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2vdjqeime.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ztazstze.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2nyyumgmf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jyhhtatx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2khnytory.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pqdmqfpt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sysdjdpv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tlnlwcoz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2fzgvnhej.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2uumxlxvy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wzblocsc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lvkixmhi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2dpwmxekg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lnfwudts.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2kzazdbdx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ufkhcmwz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2kmofyapd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gntzferb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qnvxbkte.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jytbogkl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kmusabki.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2szsrbbve.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2icckofjj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mthdbfjr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gigmhpbw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kiixhbnp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hzkdnsin.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bkqxneou.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ipeiszgx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2blludhbi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2snotregn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2vhmoisxe.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tjedrodv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdihlxaz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2fqligzva.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2igkdbrfn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sigcsuaz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ndcclxxg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2eiwtooip.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lazkunas.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tejmkqqg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ivnvpanx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwvhfbeq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vzhhhipy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ublojuxq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mgroaxne.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gncquzza.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgzfapei.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yjncdxos.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jjkpgyel.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cfwtvoyy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2efqcmeva.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ixmjsylf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyhaecae.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yzhtzair.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zrzmxvfs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vzlznivg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqqslggy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2chpvyohj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zqsbpwws.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2alicafuk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2foyswmez.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvimmlzv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2skeoyawq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hwikdkig.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kozizfyz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2unucdslf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2shlvoxel.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qrvhnsnq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ychlcvgv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qiczqjjp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rpmphkvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yotksein.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ukblrvax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwewitti.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pcybnuzn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gbhoewwm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwcmcnph.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rkvnyopq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fstwetzy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eeelslnh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvndlex.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2enosiovc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2grnblhlc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ccttuawp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2flvocksj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2varanlyr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kszmflwl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uyuvmbhl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eemphvoo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nmdxponz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fucbiged.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kiqvxgva.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bygjytxe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zktrbzca.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bepbjiul.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcqkqcqi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ypduyckr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwdvonlx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bcfgwjxc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ptsibkpd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lvedehau.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ttblligl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ovrbcfcx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cieccwcj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pcmhbhsb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntruzgjs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcavhpx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jlfoxlml.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2prxnraoi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2inbxheuz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iwaaemsj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhlbxgt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tpoxkvfb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fiymbezj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tbjwfmbi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqbpydxs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xzhgfdtm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2niypwbjk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2djhtghgj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2uavwpsfa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rzznhohx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2biewkmwx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2drbmyzei.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kskskssc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rllkbfqg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2arwdqvnt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2soeqqgvl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2frvlosms.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdkzicyt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xllgsudo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dyqlpqgp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipmfjvqd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrksrzzj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqrulvob.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wxvxsifr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsdkkjyw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ojgphnqq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2eqescjqz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hoixqlae.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bwbwfodb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2poyyyuyq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2muomofjt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wxiqmqka.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xcuenhcw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wgxvbytw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gptqimfu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mfoiwdmc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykdakbnz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpncnnza.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjmvbaob.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gxvnlaeb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpcclmab.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jguyomsp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2daytaxhz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zhxmugzy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vmegbowk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ftigzwbc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fzqbaylh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zwwidrkt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2imlppiwz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fkuwffjo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgzxgyxi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ersnfwxn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vowfszqy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hdykwzvw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xeedjrrp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2afuiybah.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fupofahr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wxeddpfa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kttwzaxv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fxsvgzje.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kdjvyiyf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fzeukkqg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2sfckhini.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cyhlsxek.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pikswrug.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fqiufagh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fhccdsmn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfagvyxk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzdnlcxz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rrrohsel.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ovyslwvz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jryvfjha.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vvqusnzh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ihcceuts.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nanomrgu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sdvqdpfr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dyzasbhq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vwcxlria.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2avwvofbs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tqmcfkov.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pkmfndub.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tnzfldqu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qjeczmzc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsytmkbp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2coveqkmp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dokcbfyw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2avvchrxa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lugeobxp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qrtexxkv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kfhsjtss.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2moijahdl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vdidisth.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fyjbwpwj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ylsvrjkf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jwzzonbd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mjkhdoze.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2grsdoopd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2acmqigxi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vmgxlctz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2uzfqvrzq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpxlhrym.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rpadvhuz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pvgvbwyc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fmmuxbxn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2boqgnmvx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cgzvvred.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gjgwgdig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrqpybvi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zjgzwtyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igbtghoa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzetgvny.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vloemeij.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkysuuw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvjblwlb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2effclpwp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbtbcslv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rhyjwcvv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tidoinvw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2unnbofpm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xhsahqix.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2sastpmjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvyxxtbo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxyhcpkz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crpqzkrm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2etqrsxmb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrnrtgdo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qmcfcdld.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wcjqkmeo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ciqnqbgz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vcnbbowy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2icfrxspt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2twlnjktk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ulcmzmxg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2alleemji.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bqlslren.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2imyznoyh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2urirfozp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jsokyanz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2duvjtbau.html


<!-- 参考信息 -->