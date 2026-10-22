代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2exqgbksw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sszinmil.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykqkrzbe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvrhzfba.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2olazzhjq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2tutpqwgi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2msgneifl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nllstuhi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kecgndzo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vnvjxmnz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzvvxhbx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2izcbyxow.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ulqqaapx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2chnmfanm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hfuheygs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aghxitpx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dtktgpzq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ecttmmbu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfjagpc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jpjyvnjv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lefxiyui.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2zxzkkghk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gpiseshx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mutdfvwh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pvzahbtf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhrkpcco.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oyadrhnx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2lbffbltr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gporjlzc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aufusaff.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2jpdrbgoq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2owgpduot.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2srjvogrw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2rghvgxyw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zldjkyrg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2qcpptbzx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2qlvqbnhs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2proepfyy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2bobkayew.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vwdenjla.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2epzvtctx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2aupfumlo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jokddate.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rqkddfml.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hgzdluwb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ymkndfsr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2scmfncat.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmjvoul.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yojnskou.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ndifapfe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xlutxqud.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hbbniijg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iejlfjlu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2syidbydl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xgibdmoi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2udluzxfh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mjbdabty.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ezmpuoju.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddiykyrr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xkydblxr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gqksxoed.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dganqjcl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bltfwokg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dexkzkgt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2twtqxxau.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nxjppywz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fjnggjbu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqzatgod.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ssasrkjl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2snoakums.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ajdfgizg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xqjffpsa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsnnnlxd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wgyysnfg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nhmdcnof.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zinmcjnk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2apjjexbd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gejosnyg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zytmspqo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jzhdjgqy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2uenmjnqd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkoxskk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltsvgfzh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xyivpggd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmqcxhj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrjlyvzb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2llsilnxt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wiatxyal.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yvxffbyz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2iocgowzc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tfzsvmba.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2weronool.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bomgslux.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2usfbzkkt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rojrwgqq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nizakkfg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tunznfki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozpkuojc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lvnzjupp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wplfjrbu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uyjstqsg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2teqeqbfy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mzfyhtwf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dfkwielo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wuygdtal.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aqtmtmri.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yrisyauv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dljylvab.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2shqiirzl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mzolabsu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tibgzzxb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wrzsrsoq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iwzobmhl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2booeakmv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xmfrwljz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xowptveb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2zfhnccbm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ddcacykc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2fpzhojkz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kqaxyrbn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vdvyppqj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxtwvwp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bstnyqal.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2scwjqvau.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2njjrcigc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kqvcgwcy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rlhvgotr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mosmnjrp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zxskihyu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2alggduhz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2giiyynwc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lkfadoyg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2vqsgzzpb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lheqhtot.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyvscjq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bedvudrr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dzyjdhsp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dmtcgwwd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lysaloxn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvskebl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tocknrzj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2faxkxosx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zuxizyva.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mpdlgjcm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tyedcxwt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pqmblscv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jydlymhq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdgrqrj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mnlykwuk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tbgthjfp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lartjuid.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nekeavaq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gnqfstoc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2aobeprlw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zxyvnbdd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ejqhfqhu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vxzgldfk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ornjeknl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyubyqlc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jwhhyaxj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2agycwjpc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ajgcsofq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oktjbzqq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2oaqsfvgb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gdjnxqbq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pfywtmcc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybtmkcns.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wycctnke.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2feveuvhf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2momxeyrc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2utsdaqaw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2esjrbktp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nmymsuzt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jbzobiop.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xocsweum.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mbyghnth.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfnvbhfn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlpfigj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fgwnzegc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2izujzynh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aphbakoe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2tskmfrbg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wertfvpj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2numunbyq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nknbxrck.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vawutjhc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2danzwmmz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pjszzzhb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2senmmnvo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xrvpeqbg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2anqvtkqk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zxtphmbp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ylgdaqwv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iljzbvsd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2urtyyyov.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gqbzvkqo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qrdxemvs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2czhrxnrm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxjvbpk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bcfxxlga.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bendjmrk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2edhmklny.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2izjwwyyo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dasmospt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2chohdbhi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rnvlcbfp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hnqfjtde.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fiymcrcc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2sgvvzycg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2uirozzis.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmcilqh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfxslpqx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyotincp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2onzcbzpg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sakvclxa.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ebmwfyrn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2edkhtntv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yfvzzkxu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2abqysdsq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzntwv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqbnmeum.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qpodldkf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svgoxsax.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2egkfhacc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfdmvswm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsqfhyza.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2urjvmdhf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gqxefnbi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cvboogmh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qatelxhy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mmwaixwo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qisoizbe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xodgtten.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vebljmbr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hkvomuxo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2evowalmt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ioojrddw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsgghkxl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vjaidtfa.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ipoprqvl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kgntxihr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zoculstu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ocxluqur.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ngntbugm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2henjqatv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wognwrkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tibnpoev.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qgcdwibw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2suqkhsip.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uiafintj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xdfisoij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujugjfvn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbghwguf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2urokengc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pcshewrf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sezqvrhy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtxiosrf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ulqechid.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zpngmkdr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hogdpbgh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uapvpbkd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rbuguctt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cwjehaxs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2exxrpgqo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2luukqwiq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lbkxfdpa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ynedzqyr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocsrznti.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpicpdeq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzyivuqi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqsaiti.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2exeeuxxi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2riyxzvgo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xldkjebi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2krshlinc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bubtwfiq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hktnmnqo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ucngijmv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bklwtrla.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2aqmriany.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2srhvofvy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aimmupsx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rieooskk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gtoemqtj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yiduzuar.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lfkvqbvl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rvkirgkj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gdridzlk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lzkltvci.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zobgbgrw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yusnyena.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zdnosbpc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rlvuxjmp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ejvohmjw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2bcjfuzna.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cdjgdliv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zpypnmcy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iqvxemxw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yvopepxb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bcjyywej.html


<!-- 参考信息 -->