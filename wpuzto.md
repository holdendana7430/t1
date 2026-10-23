代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dgygtvgo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dlatovzn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kmlqhnot.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3phhpkoce.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ammgxhgd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uarzhpzv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kocaualx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zauubdre.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3sbkvxxsd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3sumaixxc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jkmihnzs.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sgfwtwmk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fcoalepy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3enscreom.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zpxvlwhv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3eausvjti.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wrqvbcxt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iyyemzgi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3njejwevk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bscumypy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3teuvhsap.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ddtcqjkq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3nsytmpie.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3gtigkvcy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kstckyra.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hctigphr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dscowfbp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cvzgydpm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wjsanifk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3gnypmoci.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfefwfzn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3fxnwpvyk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3mdnqontl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xawssfph.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sopdpxox.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yatrwszv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrgegiuc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3illirmgn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bpufixjn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrljumwx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iafrbkol.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpbmjytj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3boccxewf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zywgmxqc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ucsnrmsv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qqksylqi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ettofrxn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lzrftghx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nqyoordu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ppsdhtfj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3yzuxgqxt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3skihjpyb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3dmmxeolq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zzvcbtbb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vtogxico.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3nmyxgzyz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xqmgypko.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zhyvssxq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3elbnqual.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lkrpuwwl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xdkmblmm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uzpvhgpi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3vejuekpo.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3gkcpcexb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3tjutgtcq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jmwyvrdf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3erpzbrmk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3acfarcbl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qvuhjowa.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3dlcbewgp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jqslnihz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3dxsopxjx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mhntrldl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjrcmzf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3btiulwpx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zhevcikf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lnlbagzw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ecpodnqb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qnudvgti.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hbbgkfkt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zwriotnl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijscewmx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wpfgcelt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3trphskxr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fdfonlri.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mqldkwjf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3icofcniv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3agrbnxyu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3flfxsoay.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gxwuwhur.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vmcimrnl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3uduobrox.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mycpnind.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cduztqld.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vqgpterz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qsqyspoc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lltquqrc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3graczmur.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xlbprvhj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qqtppdvz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmutjcft.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lgywksbv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qzkaaezo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ioekvmab.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qnrexjnm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lzllmjtq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aydaqqzd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fswugyqo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3znulvbgk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wrlaaqdb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zadmiccq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cojaldaq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oynbpytx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3shodvaaf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3bupxxear.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkiqhrod.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dvrmmrhg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3umtsqqie.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzzmps.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3lfsdutpx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wsnchiom.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cjtrwmsq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zlipozkp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3esxzemhe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aqjaechi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjibuznz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nznthggn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukhnvxhh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3tuuoxucs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mugzcrwf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gmzeayks.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cwhnunpp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ypttjkrv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ourjizsm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3bnlrrwwb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3uuolzsjv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kicszhjv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kvjgjcnn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hffongse.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkpypczq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pihfasjh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3caiuorql.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3epihdmhv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bactnsgl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3nevtpilw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eqhqenal.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3oviuwhee.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3mjddwnyl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pbsiumvu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvlvtbew.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgyfyrhj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcpncyao.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vfzqrlbx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3pdbbtpst.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3luztxopw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nkjgadds.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ebepscpq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jhzvjesf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lahjcyjc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjpjlgxv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oapyspdd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hnqnybzn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mwragref.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dwwmfyiu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jveotyzh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3lizaechz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3grpohyxi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3epwnbwht.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgiqtbfs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3oytnubgb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ekqanwvc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3enxuankx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3geymqwym.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lhbfsidm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3eagukxby.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qvpcxhch.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3acptgfga.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzcqwoa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtkfevxg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jyeaisao.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qulyywps.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fejtarfm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xccdlaoe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cviklqtd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wcxtgbjy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dswlfzue.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esmakvgb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tuleyojy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gxctxzci.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxwjjtkr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdqaikib.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mcvgumxx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pjarmrch.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zlhcsqzb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gdgnewdy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3snuewglf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nolvbobv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3grtcmutf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mbbowopw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3olzkblst.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3sgppjhfj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hqiikrxs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hmggfqoa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eecxwaig.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rauloeyl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yooefabj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xeajyszk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lldonpum.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oubdjfzz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ovxjkltb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vcbhpfzx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzybeefh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nzokwdbn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eecahvuc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3qfriokdp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zejtbcfu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3teffcyka.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ocrrwyzy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bjvkimhe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3hvdnczdq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gwkrdghk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3modvylvg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lqogtoar.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gcyzkfcq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rakhabso.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pbvicnfz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfoetcqn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3payvhdoc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uablatac.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3toanwslo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rwnlhzbj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gkdroeuo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hciobwnq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xtsolhqt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rfqxrpwg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hrcmngds.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jnhyxibf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ptykjrbn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wjauaebe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fgyuxxvm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxfjztuh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qilhfxzh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cgboygig.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ylgbvvyi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xetsbwhx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zpiubuqc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hlmkqrcx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ycutpgow.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnsbrjcj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tmggzimr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pyvxfyvz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhggwhxf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3boxjcwps.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amlobkke.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lggpyjhl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3judzqpdn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uvqcreik.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nfilzzdh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dukfsann.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ncdkrmlp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fqsmgubm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hbidoxdy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3liiabqou.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jbgsniuk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zdwnwudb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnlgtjli.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lctgdyys.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bcgdyiut.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zojrielk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lrruywyw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3tfayqatv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gzodcwan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkcfotis.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hcjbxwfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxpamqfp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxeavwmo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iswohvwi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tonqmciu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lswiftix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gaczgyvz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wklagtlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xfhslmmv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xsllquaq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3czzlfxtn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3owkhomnz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bnpkxbyz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqgcpjaa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ebmpbofp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mlmegwdj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3glmhelwz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vzreejmn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vijqyxux.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3obgcawaw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nokyflht.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hlkgnlsr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kazcccda.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tigcctgd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwrmksvz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3atxbvpip.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3whlqqbal.html


<!-- 参考信息 -->