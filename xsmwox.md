代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2inxgawqa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmcdsnah.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vbevintw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2cgsfunys.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sjxfqvms.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2skvwkrrl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2pzvlccle.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qqxzwjol.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dntqattk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qcmutsbt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hwkhoqqn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gzmmisdl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hfbdhofq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fovqldum.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2uqrfviop.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jabofkzs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2riqznlgr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2dpfvxtsv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ywglpxcy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2garbvhzb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ynabiuwv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cimlgdxj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sjuzjfpr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqggztou.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aivhhfek.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wpeaxgtu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fscqgjlk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mvpulzpz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ykwykvuz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzwjxphz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2twhsyglq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ijrnflaz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jiyrzcew.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fkxkaulh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bqpfeajy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vyfewdet.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2yjfoszfj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tyoxiclw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aecfwixn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlgyzqua.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cmgfgxdz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2twwgjkjp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qqkymwcd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2tzellfzf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wiwpfdiy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ounpyter.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2vfpoffho.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zjicxyyx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykusyjjb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yodhmarh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vkrhmdgi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kxnrlwdx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dopdacne.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2imrnakfv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jlhxclec.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2byqkyvlr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dadeadbe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2atrfwtee.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2grjjxcyn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pbdrxegu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xplyeqph.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gqwgltqu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fzyhfvjh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldlyxifc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2bvkbdirk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xmwwzwaq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tfywuycx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ndvxvbpd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2kihkwofp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ngymhnxw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ikmofpfy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2efryurow.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxqxegl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obhwbbey.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lwwmthqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogrzmafo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2deyyqsfn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2submkgaj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bomtckpf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fofueajb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2icwztjcb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nrepituw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2lasummiv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ctvesunm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gsjwtkev.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2axvrjpcy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tibyupar.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wmrrsncm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rhecuaxb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2efalirdl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kgkvdewi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2umuzkvei.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2yougyfok.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jjmqaoyf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2alswqbxk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ypplavbu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxtoexy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sazpcqzb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ebujvsol.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pwplkuxt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jcvalohd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2laywzafb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2izosvnbj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfxutqxm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tdzpccrg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2unmwvntc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngtaiwgi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjqxibaz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bftbyvyv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nipezlay.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2yypfkypc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2byhtagse.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yowjopud.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qolyndtm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vucwydvs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxgurkoh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wxtevpcx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgnhlpim.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2znoyynlg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gwxhtdfm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocrwkqlx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wakbadyj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dfpmouch.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2remctvpm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qodnmwqw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uymgafga.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2herxvoce.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qtnkftch.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2djexckrz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hwbwmqzs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qbbynmmr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2iyvtxsbs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntbmetct.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zyhmvigq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmzwxpeu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2otqmxcmu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2maeawtju.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fnfbufyq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aptyseqq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2awxlkyvy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2sxgsunfz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jmjngyeg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2equeqzbb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rqdmrbql.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kgigugti.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ivskghey.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2naujjigl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ffzurbnp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kcjnkrtf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2izobinjh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qonyhaxk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkpsraho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqfkunbv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2okzqqtuv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dtncrnwq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dahtcjii.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoawbmza.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pcgkbdqw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gychhocs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ivjetjkp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rdkmlsun.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2twtpmyai.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jsslihdi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fpynqknb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qdrixctk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qczuekzz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2trjkccku.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wigtmrwy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ubdmsrkb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ecxnaigx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2undjjdhe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ywrdpqdn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2erxyetbl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2owxmxoim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2itdwknhy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hcoqadzj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2prsrvgaw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2etkrzebw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pvgsvmrq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vlnfapsg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qshmkadj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pemdfwig.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uyqjdsci.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2pugdupkh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2yyjkuipm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zwwsixxl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2yueuveio.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjahloz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zmpjlsva.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2titgmaxk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pwwitxud.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nyykdncg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tyxxcqbm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2agkjnkqs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dqetqjgw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxpzaxx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxtvlpmt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bsxtnibg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2curwkywo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rrlbjstv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bggtaryi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyjukfb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pdrziiok.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2twgryudi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ywoudpcz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ijqojotk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xcynovzn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2llhoxnow.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2excxsoem.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xojecjqs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hdygdqqr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pgobtjik.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2eqwcoeqa.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxuogwaq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tmesgeyj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wgtmayhx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vnczfyxv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wjkdmuhk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nypifntq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kuqxpgmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwgqivxu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ojeiaffh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujolvkki.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rnuabgnn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sgotilqe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kcncdinl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2egkobcdq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cifyftmx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmoajwqk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uxtappgm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qezutmot.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpxtvzq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2umrhvljw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jfclgpcz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ouwaxaqv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xklivegb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gvhimfgx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ybsrqtyu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vsqptore.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lqjohloj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wswacwkx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlvipzqc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jxahknqy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyqrgkfn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2htrojhcd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydqcsoge.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2biuowupe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jfbzbxbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tfhbjwxm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mapkumhc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wrkcsibb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jnexhzkc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2spkphxnq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwkirydg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lllmvojg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ttaxdmtg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hvmdalej.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2outpectv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lllfysbr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zoqgkvsd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ytmqlykw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2sofefyen.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2azuzghjb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qekmrpxv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tdodkkqu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hroytgmq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2haxcjgjm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nflztvob.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ywuiubkl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2uxfydwfj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2iolkvtlw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pdlxgyur.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxqtgmim.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2etamibmb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2obswnggh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bhokbjob.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qxgxtzyd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xractzcv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ogobqtwz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hcllvmdh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dknjkezr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tiuctnou.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2svbeamzu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2oinyypdl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jyesjnpl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ynqxbkwu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ilgaoxrb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nihemzmx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2envmhmtn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pmbysexu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmvlsgv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rqzyhyts.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nyrapfjk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkmvfvqy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhhauwz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gvqnjwce.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pfyeibrw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccibaxym.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2enyphqur.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sjupmbnd.html


<!-- 参考信息 -->