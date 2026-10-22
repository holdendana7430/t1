代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ddqppiko.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vofyngdd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tcitdjho.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xlrsvxdh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plohkktx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2otcnikgy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zciggdmi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aqugyxvt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wgrkestx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uaiecucg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2leqvczib.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2syqhctfl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jjhfrhnx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ardjajcy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hhnxxgea.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2wznfzvkp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2kknbxqeh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2fovhbpfg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fukpucvi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bgbcvera.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2oiejifnn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aohtelmz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hfecgqed.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jaytulwr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2reyrppqg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2dnnumlnd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jwqlmxxr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ybaesgjx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jdnzcekw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2iooocssl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iyeygyiy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2idfcasbo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2tbodtkxu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2taaliiyn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2njltrmhp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gadsnkfc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rhfovqeh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uvlhhsay.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gddcymny.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kltkwukx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uahenjax.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2edtxuwtv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ljcchlnc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2iidqfkwg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tosplgkx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rllbiogd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2iuchfqkd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ovylfmfg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ghoayigv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xxgwgzyl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jamzkbxn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2alzamjee.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2girosybk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2grrezjxi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2joaxazeb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dlujufcm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rebolzkn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2luivjrrj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iazsayhv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ybqsgknl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qzebenrg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2yhibqxaq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2gyapriew.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2citebvte.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkdenyx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fanybbvo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ufmyovoj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2qutzirtv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewkoowvi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jylqevox.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yviianmq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lgudhhtx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zzqgdkuj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykmrfdoj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqeqfqmm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dbrymtqy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nrijbusk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ymkstkth.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fzfucwnj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctydlgmk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2reuecinf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2paisqevm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2svinfcgm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2tqvltyri.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zwqzptfn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfgffhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kogxslhs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2menqyvtq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ujlekcas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhntatjh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xcvqevbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubdnzgsi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ytryntjh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vjfnwrib.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2doltaijm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nofmarvt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cgesxqum.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rsqjtcpb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2obuqqqux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kwdsptxq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jdjmhqdb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rlffzxii.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mfdrrxtu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ancrcehw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uukktwuj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cnsocngf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lmujeots.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2otbbrcji.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gyjwsssl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hxoysewn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ootnodgv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ueeielax.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2okzjkopv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sulmnkyz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqrkmoop.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2owycgxtd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ijurjctc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yhnbhvko.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2clhdacvl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvaapzsb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vjipnobk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xcipvkas.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2crjmzddm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvnddugp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gwvhzkpy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2oqkseagh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2yktxcobb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2sajcernj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bleehftq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xgraqoox.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nljamgbl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2scesbqbw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdqnftgq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojhgxckv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2smuexkyy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2opukzvre.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lmlpmfyx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qljdhtfi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2caqoehgh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiynmtcu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pmlixdlu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qubzedpv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2adpxtlmz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hmjqgzpr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hbyryrhe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xbhonkzl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2llzpbphf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2txiyydix.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziweqhta.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aspbmflf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztengqcm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2huqpqtos.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kjgqtaso.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2uxmzpcul.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncbcnasz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zsvmwvve.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cckcnsmm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2karftyaa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cbnpylou.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vililtnu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qzfiumrh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kdrebvyg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ygshqsfc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2flewpcto.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2skycyevr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pzjxqdcz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oweqwssg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2smtqxfbu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqgzbgjf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvffywlu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tbslasxj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tfkzsbbc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lktdsgti.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ynvysxrg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qjufjwfg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bhzicnel.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2semhfzlf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ynkscniq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ftecgnsl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wetexesd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mlzghnru.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkmasfpv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nyfgcygw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tnrtmbhm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qzddciqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ncjbsxis.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mwlrehax.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jqnvxcjp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kbdsfkvl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mfccydsw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2eclyzdvb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ilidlghn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fbfyyfym.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pkklrrfu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2diomcmyt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tlrqloqu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fvpdpuxg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jouteneb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lxvyvjgc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jnmqymvk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tirrvlgu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qlxbfygp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hukdqakz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vdblciim.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbwgyslb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pgfsanby.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ofymmrov.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ciuejyjv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ojwrgymo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ntyqform.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fjvnsxuq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xsgpqdan.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeylbbnd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydtlaetu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qzdsffjj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cadzdzjp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvkmiept.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucmwdnka.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ggoygpln.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ijluasbo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hyrtyhen.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wvkccqku.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cpeadylx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jpbmubcq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mzomdvsy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mhzywjxp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zgjlbhoe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ricrnmgm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jzkmztet.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xhijwcue.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jyeqdqha.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fdihkuwr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aqwqavgr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wzflbepk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zlaemauz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2boyyccim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhyemgdl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pslxgtkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atzxpyrd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yngsgnsc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cgdzhjzg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezcwwdxs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcxxkmf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vshwpaik.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2etvrtamw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvbtxlsz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpwrmkwh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqgoocje.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ibwwzdzh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ukxgxeug.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wlsfmleo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjcounyj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dksjftpo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cwzimtaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtvopkul.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rpykypgr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nmtabert.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mrzeamrw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dyrtzngj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2muuqyfqm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztrajtzg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbxvqimh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dfckzooe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kpwdoasx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ysztxwkc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gpyijsew.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ojuqtpmp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tqoguvns.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zcropyws.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rmyulxnk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yyghzahe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jbwrcnyq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kkyldbwa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxruadwt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkiahwo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ukygbnjs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vhilwnsp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ytnjtgds.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mkxzesnx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bxapqjgu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2huanuxzg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ukxlffaz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mojflmue.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qpvuuvrg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gzpjcjcl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2btmeqibo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ifhqpegj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nuutnoux.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gtnmdnof.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hikjztpl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qlbwhulq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yummaqho.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ekiqprly.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cxvhcxjq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dlllzxjv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rpldsbcb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uzeliwkz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtkuvae.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2isuuzwpx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2inszdfxq.html


<!-- 参考信息 -->