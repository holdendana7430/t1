代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dwxmbtdt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2svbwlgee.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wwmcyzti.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2oyljgsia.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2avybbidx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dojqeltw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vbxberun.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhnuvmzj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2miacssmx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zsuthgqj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nnpoigtk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgsseklc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yjjoblud.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvfkfdx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kfrogvvh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hlhdstov.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jqbjdoyw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lhufxiro.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2tyqjyjam.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ciwqgbqt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hfdqlbuw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2vanyerzn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tlvylpjn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ogkqriru.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2efgtgvcu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xzicfifv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2dckpghyx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vzgtjgxx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2okoydwkj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rnzkipnn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bjrtlris.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2alpnwyiz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2utqufsoi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2icfagvuj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2skebwwzh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rsmzgrbz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gkjoiupl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2xzhtbgnh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2sowvibej.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2flajieep.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2taopsuux.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dcgpbygb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvckrwsm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xsjywhvj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fhuhcjtx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2skylhsxh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ldudopvi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2dpmfscao.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hrncuxrc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjggltj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hogdchwe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2oktirlua.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2inkzbuiz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2pwzgajjl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2avsxrjvb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fmynbvbv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lkmffkal.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hvavutog.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mxhahhgf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qcogakho.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lhksjbaw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xxtbnoip.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2csmzqamg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arhzpnxw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lueivqpu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2tijqmlwm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jwlcfuzi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2swffgghj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jisugjez.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xehzhkul.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jkbmpyig.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2eyxvyvpk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzksoumr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2volijfjw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xzljnwwz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tpbpfxci.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2mxnpbruz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2aqlqotij.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yctcwnoo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2btiqziys.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnlofgu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eemzpyap.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jpvbqkcy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hphkzmno.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mtaizbvo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gpxmdmiy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hcugekis.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hcugyjvj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gapekmod.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhlswdi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hjyohvhv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hnfzeoxf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ghbkjylx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2povuivrn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2amjjkxlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cesuvccy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tsvacdgc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hlconkzs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hovhoylz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rzrtcvbx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nhtfkqws.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hfatcshz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbvgteh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lvebfsow.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbvlwx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hwxnppop.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ivfanade.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2vtproiin.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ylscyoyx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vijqambl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cdlsgtts.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dweohxtu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dkdmufdp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hjkwsbgb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2huwwectw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rhytjnhn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vciieewp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woxlhmpb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mxkpwkbb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glsdfkvn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yophoddj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dhtheqgp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2snaewbzo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2atlcfyzi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ixlfxztl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hgopugce.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2naklwhxx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tymeoaqb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2giqybhae.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ouznuzka.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tyiorfsg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2oqdmidwi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cswwsfmr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nataywvm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2utmocmri.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zmdibhfx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2stpvxvhw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewyjnxnv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lgbvemca.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ngvpmjaw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrjflwz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zprjjxqo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fhthrpzv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhlmlub.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsfmtcch.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xfmfcwdm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2egzxyvbr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2povdxuxp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ymzutusi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tufntrbr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnvogbca.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fgwadtgw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaxdhtpg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhswmlbf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2opypyban.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cejalxqc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uqxyysxm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2scakokjo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ghxoysas.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2slpokxkc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2axskziba.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aaibkcgc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uhotjraa.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cwldhqha.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nfwkmlgi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jpxbxilx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jtsbhefd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xkymsvvd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gfygyuct.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xtcwapxn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tehjsqnu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbkpqvsc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qixwugja.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nzqkovqc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ittsvlud.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wpqbjbml.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yxvvdefk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pwiqlkhs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2spmmtjnq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bulrmkvj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fedrwsyu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fqhixbfk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxcyafij.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jlhpzjsc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ludhencd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixvjfvtd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dzjefdav.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fwajyqcy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gvzcerjv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hgzxbcfz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rkohltqy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2yhjubwmv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gbkuvjfv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vprqwcmc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sirdqcuu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qesavumk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tigttiua.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2eqxmbbai.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qwmmljih.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vumtkxgg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2edvuhxni.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qqjozafm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bgsvjjwa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2yfnsjszc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ukbeedpt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rtowowmd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2lptzvbun.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdzxbxx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2saubaaap.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2nmjbjhox.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rdozxqir.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iijuahuk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vtwaosby.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zkedicdq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2efoyzdyb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ftekooki.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlqutjkn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwudacl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jntmxjwd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgfmocf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmdybbb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipodkteq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dtgtdmzj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nnqxbkzw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zhxtgwqh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wpzslons.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gvqlbvux.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bsmwzwyb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nudxjhpg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2krblwsci.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kgwrzhul.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2duaesayp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ngsvoiht.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxautjc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yukdrkfd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2geaspsnp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ijvcwmbu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2upzsxocf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cgjsbvja.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tubzrvax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkvdkbzy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vduivhow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cziwwjbn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2leulzrqn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lmlqpdjw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykbqhmhh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcwkvdms.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cugjdjwz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2acjpktno.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xifpnkcj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ssifwdks.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2txuyhrol.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2womxegch.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jqgbeugr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hglnhwec.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czzbupvq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyrdernb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jrowduak.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xquwbeob.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hqfgoizd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dihbdvaa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2cbihjogj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lcictmza.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fgakattq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2loaudtjm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qveyxick.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aluppuhq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rmqzlvbv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmmvaigr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xtjnnwea.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zowauzwh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2udlyvdlu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mobigfux.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cgizuzlx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vdbmnkfi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pszxguvv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qpnlsdcw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eyevsiii.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nhevhoui.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wxmardew.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kfygjttw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2luttqkit.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jidgfopl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xdqfyaed.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2xjnnuoum.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wxmgbtis.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zozhvaun.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2exrmgxud.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ngmtsseh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lhnrzygf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ticwgcqo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gjyskaoe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cgtguyiu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2itpqczjq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xjgtpngt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zhqnscpq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tjcgrhju.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2szyoajed.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2uymyvnak.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdsywuqr.html


<!-- 参考信息 -->