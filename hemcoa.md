代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2boymwggq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2bzeomftn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2orbxulmw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ncovbjpg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ixboemmt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2bykkdxnl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mccmrmgh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2qywshzmh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cakwxlbw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mrqztqnq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wumakynj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2icakfbna.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2omxpdmei.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lyqwbozj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ytfzfjfe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xtbhvjdu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ucocsqlb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cqhcvxqv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ljvnpwoo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ywugqqtz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2nzkxanby.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rubuhhot.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jhgyzswr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2oenmndhc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rqqvpzhb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uyuihcxk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgkrzzqn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2fhhbfdwz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lnyirvqj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cdhkqsly.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xxntysme.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dokdoejv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vholdkky.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xwjuijjo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2drhoqqiq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uuxtkzyj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rideszbe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hnlouyvf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jfayqube.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bgsnpzbk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mchmtwfo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2uciyoptl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ywzkbtfn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lvtjvsky.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2pgkzxgsk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rlgcmrof.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2timlopcj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2udjcihms.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kzyfmqje.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tryuemtb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2bdbjvkwi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rkzmelby.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qflmizpt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jkrmejzn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wrotabsp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nfyaohgb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2aalbdpzt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ufuytmvl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rzinjoxa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bthhlgsu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zyvsrloa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ybdkimge.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qzwjvull.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yqtnothd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ylptdjhd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uftxhsil.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vroxzzxm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkylngng.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lucifqjh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2brmvdsyx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hwpibhbt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2vdhypioa.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tgoveqfg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ruwbfsjd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sqjpxxte.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2szzvgerj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ichxzzxa.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2pfijzgnh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2aqqrbepd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2waljzfgp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pmmunksk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cglfyffw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vlqihtow.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2yjfbbxbf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uumljwul.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gpenlhju.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2reldgmjy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2stufiuoi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2obpvumwz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2sxbypkvg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vmwuhjgp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tvunztur.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kcyyqwud.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rkotaovr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2umnohtdg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2watnepfh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ryshfjnw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2cmiwmwlk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aghgmzuw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zlvvfscy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2pflpktds.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxigkge.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2irrrkuxu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vssborna.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2idxvenzj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkpncvsl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2iaflkgww.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xajzvqyr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hbmsuaoy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2iqopjubs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2issjbfen.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lpijpsah.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2mjjdpgul.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lljvvkhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2obawsvkh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2eondlxsk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mezopgbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnatniva.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jcwcviex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlfjilmp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kojzuppw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jtagaghj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2torvulfc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zmlqsflq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ysblghqj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zsctxtmn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hnlawkve.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gtpmmqxe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2niahhmue.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2kwoxuaew.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2jawkfnqi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpzbuemp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzlsavrr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzcgmxdx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fghxzycs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2scwejivx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ypjjtdfe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ucdapofh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2miefqjom.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ogilaycn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqnwsztz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jikhoiib.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woeysoai.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2soccdkvw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2poyqdnpx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mgdejjns.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2svcyzomn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dwugehrh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lejqsddq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hchlguzl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnihgpfx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvgaaxx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxiwhlye.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdororit.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2meppqqxn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aopnufky.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2watvmmgk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nmhdhsxd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcwcnrz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vdjxuesv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mglmnuex.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tnbacxey.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tfoxbjqt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yxszzgkc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovtevivl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vepzhxbk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2klztesci.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lconhnpn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2znfovdqr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qivvlowz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgojhetf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fgjeitgm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lbfwepex.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kxtobknl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ygmnmigp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ukwcerti.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2anqfmmze.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ihhnpzij.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uamtfhqq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tnoocfxv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dzevyfow.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hrkdhitm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckysmdex.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2txvndkrj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pdveshqe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zcuxpflf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pwzsyzit.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2icgtiagf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ywvadqyr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2srjwtyyj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gzhsvdju.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cidktexk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ggdhdfzi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ylkhyfau.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ubnxkbfj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yxopkkrw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2emgcjirj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jskxgwsc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xwerumxl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pusinqaw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kibgakam.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mbgwxtmv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gvdfmipp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mehoomyl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zjzyfrxg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pkhkfdwm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rurzbgle.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xicdaqcs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cvfhmrsj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nqcqwbyi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2woyxbqlg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ukmqfxwl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wrchuuri.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vquehsbb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mcnhlvru.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ouicqljs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2okipveyk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ypqzcoia.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2whztmdjl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qspnotci.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ozhzjbyj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2luyhcmri.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kwxrbrrq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gzrjpqou.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yjtpjzum.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2deaapfhs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uqcephyi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2pvqkozvz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zmmoromj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cydddpdi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccghxoqe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bfqbfhwu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cfrydgwb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2sakctzhx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pelmqsjo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2huarppvj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qzvjkikd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tmxkirej.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2icgogies.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tejovkdd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zjkkvwak.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zuacbwhm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uqetzgkb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzlcjizs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yjbkfnuh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nixgwnlb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2lxljfzrx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2edhwjdbl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2djebeagg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aruanetu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uznfxori.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kfpmkqkn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2seaoysya.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tlxheemk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ukkkpyzc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yjicccmg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pnspouzg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2aoikytcs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gpbjnzts.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hvluejgn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iwhubpgj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2whnecttr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ogxdgkqz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tfdwtxxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijbyrdff.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nrwwpnhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdrjizkb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jysdkoqa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2teuoikti.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ehraeacy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcidqhet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vznzepgx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwgqnmuv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2agaycpru.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pknidpps.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sxutpyhe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tchbokmj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cmvzoelm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvvgpdhg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kzhpycsj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbwpxnk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2znzabptg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohdmglug.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ztbimnge.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ptqyacew.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zanmrzoo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kpnxqwfp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkjjfkny.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kopejqkg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmyhpnnx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrrnvorn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjvkdbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vznbvycs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bysidrtu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2pnivujsv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnbaphx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2moqgaopg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ostpvmba.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ipolwrlf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2awpiqofj.html


<!-- 参考信息 -->