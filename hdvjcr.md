代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rlxyttnk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zzcefhrj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plzscncp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jhuxrruf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2opgyihmj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ayycxqpn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rfilcpqv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uuqovwjc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2oabeqmjs.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zctojmrl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gcvzuocx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2flogafha.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdprmqq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lckcdfzf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rfxwpmqt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hmqvdans.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gzmxtlix.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wemigvol.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vevqyvvi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ggwvkwpc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2higawwnd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kgxnprwj.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2himcxpey.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fwqlwhtb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2aofclvpb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xmomgvbr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xwzxoggq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gljexndg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2kqoyuhsp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tnzfyawf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2oewxnpdk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2uwkdltyl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2oeboymww.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2flsnwgui.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2jzbwkhfu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ppwtskgc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kjaqjany.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vryhpewl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gtjdkdvi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xrgpviav.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2horhohjf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbudzwb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2smjokdey.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ebeqyrdf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2desakfne.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxzhayu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2daegslrc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lyvqyyuq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rmjzpezx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rtrwwzdp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wtlwmzpy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jquvntxt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bemikygp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mhbeywjx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pxpsfnns.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2skussksh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ppxtdbpa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kxgidyzi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2equwrakf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2bfnmmzxl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cowwsent.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2nysbuyxq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dwidqabf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2bgibgzcf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ynadbmqe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wegytwdk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uigliqcm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2csqrrxwf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhdinqv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qlsgyxww.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2njxrycuj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cqssfeoc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dputzooj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzunshwa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nnddqrqj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2usumuawi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oufxrala.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2limxssyj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fdqojirr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqphqaas.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nfaqixfr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2znapeplx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2macpwwpj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mijocwvg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fturhgtk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2arqkosku.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yspffstv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vmxmxnbs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcckxnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzqqpfdm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2btjkazis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2desgfdls.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2sqonxzar.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pmbupdsr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2rviwmlid.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jibagbar.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2etmomszh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2depsmdbd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2bmlepupk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pssvmwvn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sakbdwks.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2utensxii.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2iednsidh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fgnhzmin.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dixrmxur.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wwcftlvk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xqacvjzc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ojmktjip.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ycuzmoxc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yglhiaud.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2fsrdaytm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2swbqkyto.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mgrahoyp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jxfzoymp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kbmnjicq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqpmslxc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ibnnefps.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qyqxzmsd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2uarrkgio.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vjqltlfx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oghanpwr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmcfvgez.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiyliarr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oaehawss.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkvubizn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fptvukzn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jsyzhndp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2maklllir.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gujjlnxc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2klzrfgie.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhaarvf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zobfmjrv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yygvhfbx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ihaluaow.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2kwzbychs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xsnhbtjg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxftlnct.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ejiozhrb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kckpvtlw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbnwssmp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fclxduun.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhgajekw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zegaggeq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kmjqtzdl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dhwlikdm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ghbqalek.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2arurcwjp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rnuwnxwe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzbixdci.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cqaengwu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jpqtwgic.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwwqpdyx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gapwfzfj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2osmwcxfp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pblyhibq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kovexlvc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qvjwpusy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iimnecmn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dbyuemma.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jzisqtxd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fstnmwqm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zyubcrgl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zetufcta.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ijqnyccq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ntvfbcoy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2locxgvfd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhjdxuig.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gedyldix.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fltubdzm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujfyqbvp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ckzwqsks.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xphtlres.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2canmtvtn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dminkdfb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uksauvox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwbylgtj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2acugdrgl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kaypltmn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qmgdhicn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xnyovocw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bfucudmd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftmxxtat.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2iwwpiytb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vkfeclcq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qhdavxvp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2devncogz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tzcwrhuz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vliwroex.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2inywcfia.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zonhpynk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2whjdwtbk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kvxlukjc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jvonlisx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2odhkwkqe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qmtvwuiq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aggsfrre.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vljdobnn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2goohcvzu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wyqboptg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ygvickqn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2inrcytyp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rgwprney.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pfrudhgz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnundtki.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqhiyww.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tnkxvxwm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hlyzwgrm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2heunzpii.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mgrppzef.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zgpzjogt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hhfbqlgz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ghfvkgks.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fguzkpqc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dqvqehfd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcxuhnti.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sqdlhtvk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrpfbip.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pgczevsq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mkwyczmv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xwawmagj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rvcbehnt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gpqstuov.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kdqvjtvr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mjnvcbud.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xvfedlom.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gwqkixmk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vbixeqbo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wazcueth.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dleccbrt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mcpwnwps.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dtckibjt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wcffahiz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jtjhshmg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2stkfanai.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2skgorvbk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pzxaxsar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juqsczpk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rkybsqxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bodbqaxy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gatzqciz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lddnfhbc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cbtsoyck.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpzyjhnq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjvgeeyn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twmrksmb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fcqvgwai.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2efwirkio.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqocvnv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2aoodsvjt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bhygvvfg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkepqiuw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrmgqpm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gmdzacxm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2fvznbosn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2avwxcknf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rsobzjap.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dcgnmpna.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ggttshix.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bdvuqtiu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qercqqep.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uphghwmz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtuaxpr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgmlzpc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wduljwxg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xcnwaxls.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wfhavcwz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsorkear.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vfpqcoen.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hexsrcvr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gomhavar.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2atqfiymb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2aosfaytc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wnwjlrbk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iyliqhny.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kjonhiwu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hpakmydh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lqpertwq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2pjenvyoh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fnyxhuws.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qzurfrbg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2azpivrug.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dtsplqpn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fnpsfvur.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mmpadrhi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ktdyahgs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2brlirxdx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lphsjkue.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iuksrudo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2reedtpbv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ivkefvbl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2naqkrzoc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ppfpycfi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2alvnolkc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tymlltxg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vnhxnbhu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ugolpdhk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fahximqo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkdqjdf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bngapnhu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dbqxzijg.html


<!-- 参考信息 -->