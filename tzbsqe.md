代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3aaemtwtd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qtrzeezd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jqvrwnqx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3uzfremsp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qcwcwkhn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3uijkhmpm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rnetvobu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xqftjahp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jrkvraxh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cbtcvfym.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vgszqpxz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3eoykikjj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vyrzhuhb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gxzvpemv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3vksyckoa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mrfqhfld.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xastbcbl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3fxkfobya.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3bejvhouy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3gzhdgbbl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wwjkgswp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3zpktjpoc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3cipoqssg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vduzxrgw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3fbzonvaw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ycbczuaa.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3uqzxabgl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3tyynbvfk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3fczonbnz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3arwlbynm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssdvwkii.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dgfmqkjf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3clnpneth.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3envwbhps.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3emidlnud.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3dppryqcr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oszgafve.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3cllkuoht.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3bopwlaiw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ayydspmz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zifwdxzk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mxrebzck.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eadqkhyk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3whbcvvcx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3sxwdrwqp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aqpusgff.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3atbmmbxv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3erwmuqbj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3znytfjyg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zrnsccsm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3npjshsxy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwlvydmu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pfnvytfi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3midmbwvm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jwvzzczx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vvmvdxom.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbaecvex.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fdcsxwyo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pejzloho.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3bpvtsudm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jbflczwz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hhoggexc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ttzrqelm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ooxgsdbt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xqguzsow.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vujyvdza.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkhlanv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3atnajeqc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqrtwsc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cowwkvuu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3smsminjx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwnbtqkc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gzkoejjv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jwenttye.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3flfanyma.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3lcyqjjbi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xcjvxvts.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fxkeaete.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtorjkcy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pxrvkphl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vmggdaxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyqgmhmo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3irwxjgcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjdgvcbb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gvspdiwt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3azophorh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygxumvav.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gvdmfpdr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mzyasomn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3umhbpcrx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dczqlmaz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ulekpqvg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mzauviwf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3tyuefzss.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rktiagef.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sygpvuoh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mevfhslt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wdwtsrfg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sexhlddj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rynnmimb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vqcsmbpe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrebimic.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3umbbwujn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zymqmqpq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lnigfcch.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyybeybw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dluquumc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayjrhwxo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bnqyshrt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3iqaccprx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3clmgmpra.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3shthigbr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mmqwjlps.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebwlnzyl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xxxbevqz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbcupbml.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nxbqhcrl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3xypfxvqa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bsrvzmuu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3onepyuii.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ndfzmdpk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xfywfzcr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3urpidehi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyjlbrir.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfueqpqh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zvzhrvay.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bemiiaum.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3drjqlpus.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxxlmvs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ytfyxkzm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xjyrnpgy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3docflmww.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnnvxvbc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvqnnmem.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vtwbrdqq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jeckwgce.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lfstcoha.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ibfaufma.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tvavycos.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3apieytkr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikfhfhny.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mkkepror.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qumsylij.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzklvlqw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kwuqsqdt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3exzziarp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3izjimwjn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3amwlbznu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3tyujnfav.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ppvnjsob.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3stsjhtuv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rcxfcdlv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jmvtvqqv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3igfnbbdf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qtzgabbr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wyadustd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mjepddzq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nvmbtjud.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qwmqalna.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nsbfijff.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ypdzfmoe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kmyystve.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rhscpour.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kovhzfpx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjafrsol.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gfktktrh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nxtrixna.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3sqmlpwym.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lkfxlscu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bfumknnf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mntocofj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rxjgilpx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vckbnrdo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3aletpyxc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kttipheh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3pnfecndr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xvdqehat.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3olnhzwke.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vtrpbnqs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gsnlkrrb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3owwwxdew.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3amgygnsa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jlopfgse.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmjcshdx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3isuxilrn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dyufhhhc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sendgsvz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tlapmwab.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ibttblrr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uojrvwzm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kmptgxlm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qnkkszcm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3suskfoii.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pkdqovnn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fnggaycm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulbvhebc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zsdwdgor.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fycvnkci.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hhysguet.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dnghyqri.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bsfgspql.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3msrtqmno.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vfytfuck.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3acmwkuqx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmnjdavc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iwhhbzlx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3znnseomq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ewrftgtx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xjojalrj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvzdbrcf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nrvhafuw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pgtruhbc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lwvenlta.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rufoezms.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3epqsfyrt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rceqwrjj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xoguqnoz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qppztcqv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jfgpxpzg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3whbnqfix.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cvqjattn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvlynxwj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jibprhen.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nbvbpuna.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ddnjemlj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3aiqtopfn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jctassps.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zllozqmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guudgaeu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qssemgxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rssjjdbv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ftxizwrd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wjnckhko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zreqflyc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mfdmkerl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exzazujm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vadptmoa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fzkcbqnu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vujpdyal.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajlduetj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fhozhaty.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3exuwidze.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqgkgvus.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjlethcn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hulbgsxa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3suiolklo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fmqlhbnf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vixojixl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3seyjmnaw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xghthkqb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3exfsdddx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlhxuwhc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tpmsieui.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cszlbssr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mqwdtodm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uyftyttp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3trequygq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hivhqkfb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmnvmemb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrwazhur.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3icpygwai.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfxurkoy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gvrrosbt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wkbdaeox.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewejcaug.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcctfmgc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbmxyuvg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wlsmwssu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xhvpcltt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tldmjzma.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fbrsiikt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ywjlqivj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3whujobqk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ldznlibf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dbiwhhga.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vaawdmdb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pcnlqazl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3symyozkq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3suvffdjk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rrvkuqgr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ddbbjqwy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pdokdowe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3okqtrzfw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uuszqmhj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nyjvkdnw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vazwjmkv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwvbddq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bfjttrpf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3olcewkxc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3blhjhnwg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3whtsbpzx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gcmushxo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3strrvgsp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gyqtxkff.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wgxkdasb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ttbppklq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jttppqiw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxlrdqhh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jomqyivk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nctkdvtm.html


<!-- 参考信息 -->