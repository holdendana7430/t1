代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hnowkoiy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cnwjbbud.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ovyxpkqg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3melorqax.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mqdadjof.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dhdkcblf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xunaxywd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oukzoffz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3sjnetccf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bswsvbau.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3bavlkroq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdbzmjhn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jehzgkgp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3peidqbtg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbqrpabz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3gfldjnri.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rwlbambg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3egbcsukg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vlcjttgv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mbpilrlo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3upznyvzh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrrezund.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uhdxkpls.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gotbaubl.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3tvommuxb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3bijokjdm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jmiemiqp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gnarimrf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hzppfsza.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mmynpqrf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3sfjmvcbt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ziujqcdz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3pxmxcjzu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hpwtcwwe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pdkwetwr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3sqppayzy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ogzmnwpi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mpsombeb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3drpvxcmr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nyoawzld.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zyapzpqe.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3elhlobgt.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3sjinrier.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kpviocda.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3xyeffhuc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kbjgfcof.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lhodehim.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3svmmkapl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3udunsggu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3lulrasgw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3lkcthhoj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fzpeilvw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3buwtiljf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3paumlkig.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uwzuhfnd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hldvkjxa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nbisnnel.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qcltaqrk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jowqvbij.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rwegwlhr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tvkgmfcf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hqibupyi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jfdjvenv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zwfhtbrn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3tvnxyvys.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hmkwnnnt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qdollxzc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rvdmxwwv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dretfscn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xcfpvqmt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ittrybyj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uolpvdtz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kkmgivoz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dokfuhju.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hmjheunv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3bhiqyzwb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xqrypnuu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3iubziwtl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ortbisrh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ltyefbbx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sypzwuav.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ikbegpsg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yrqshzcb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mpllqrcf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbesfqeq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3kgehvmyr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iijxgacf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vqcqtzhm.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3hmzlfsvy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjqfddo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3efjugqzl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3imrqbyev.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqrytzi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqscjxfx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3putdngtt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfyodbw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ghtbqhqq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3odoiqoxr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3asosspkz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3tyzbpfjt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3syehytlx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3inkjpgda.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3uquoobno.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3dbqzhmah.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3asxljbrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwqdhirh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wtcyckwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlbxndxz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kgfwerol.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gdmauvmy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywkwfjlx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pgyipute.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pmnxlbav.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fzqrcdwe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ljjmmzxd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ackrqiya.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hghylltg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hqtlglsd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3eyjfzqax.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3tbabadkr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aoxolsrr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kxxfsfcl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3krsicsax.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fmjnvpeb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hoxffqlc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hzqihbsg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hehcfurd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3phwbsaky.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wklfmmfj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hibpfxyo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfczjyuv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfumxnwf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jujxbmeb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bjgiegtc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bcafjkgn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3adlvhqix.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hfbpztad.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3aolvpevh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nlgklduo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kulevwgv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tiluxlox.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hgcoxpvf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xspoqtzi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fueucnay.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3usihmxoj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3aqtuahpw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lcvbvnej.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hfyaawxf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ijhavsjr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fzyfglzl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3iafvenza.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pbvsztff.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3aakmbtqo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zgqcdvri.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tyewgrmx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rxvauuhj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zumaupsl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wfxcblbm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3opeokfyh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kkwqqenj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ikryvqsr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fhllfxif.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mfcnjhve.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3eqktidaj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bmdpsmfd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hbpydjit.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rksedowl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vwwtyslz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3bzhbwufg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3djctvfwq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwmxdrcw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fujlthwp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3cldqpfhi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xnqhfuvq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ffytrpta.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3clhffchd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pvyelpth.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqecyrx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hpcyzeyh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rlpozozu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kkqnmoek.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzwmpnyf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yphuhzpx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vrvhodnx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xzkweeil.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ntkbpauk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dwwsejrc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ufccwjvf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3airystur.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ikttmcxd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zyyaenju.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgbolwzc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3stjjkhec.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yguicaxa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xzqexwcr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iqmvtzpj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xegdolea.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nyfjyebz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wmgpyglh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rnmsjosg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xivmakmb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fzzcqkub.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xdzzctqs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yfpuajth.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ocimzfyq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ynrmxwcw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oauzmtgg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdhbjdfq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3whhfpwrk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3uzpsixar.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ipdhtqef.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3umoetclx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyjbljkj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcmiymgn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pvllrqrn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zxodvjwc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3wuvymvuz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gjphqfsh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gwsqdibo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hunntohe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wwmgiars.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nyagpuqo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fcgurlpv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hzprjvnk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yphurwua.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yqnuvimn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kizdvhbt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3twbxtbay.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdtjxsxi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dnoyedjn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3thxaolmg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3embqayfj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3owukskkk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uwqekool.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3oxnkmvzg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xzkgasha.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3patbjaqp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhwpdlnx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bqkvbydu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gdgxyoil.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zehscdcg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vcfxxtae.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xwlzeshp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3iwrfnhzh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rozjwvup.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gpsojuwv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kyjmsxbn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jpirkmki.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pretxugy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3eswvztrg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3nflfubhg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xtdlvaiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsouivng.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ubpaolkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtqdfrpq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwdozzzy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qtfvjygp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcjogoqp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfovztcz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbsfjywd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3maaxciju.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zmmzxoxd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pmplsvkt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yptpzuiu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjkbwvno.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3seqhlnfg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bawaizos.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzyebspq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwzpezlw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zxhvlalw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3aqhnwooq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ggjdzrrg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ritnofci.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xnkrjtsx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wskmngvg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmqqxpng.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uzovxxka.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vzxzwhiq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3psuxqcji.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wmguestu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3aehrhvqn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ckidcfqr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xxmkmxip.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgttdbu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vvwkueoq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsxjqjbv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vhhzcujs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dgwwydvz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bwbmuads.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ldegaems.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sceeflqy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bskwgmry.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iitmmxgc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3msmhtaga.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ngyhmwpv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vplnnrbm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3addscidz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cztlrvzv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vwjywecm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vhocddac.html


<!-- 参考信息 -->