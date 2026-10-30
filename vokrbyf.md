代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gctigbhpx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/ggukrqtan.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/geianwqeq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gmqkrxjhu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/gkscvrqqw.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gocwbppsf.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gngmpkhix.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/grzailbdt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/glzuplrsq.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gmytlnxbu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/grljtzryc.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/glwjwefrl.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gowlcyrca.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gdbgihqns.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gwqezwama.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gfjtnwkvt.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gqljtcvwo.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gqrtymbkp.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/giidwprma.sHtML

Go:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/giwdqlezt.sHtML

Ruby: a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gvzcocgww.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gfmefqxnl.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gbydbyesv.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/gnfbwvaqi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/guieggiip.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gxewstgmy.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gxmvkmqul.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/gvrnvtjyk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gskshwale.sHtML

Ruby: gets.chomp
来源：http://3g.fehbvm.com/Article/details/gklshytzn.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gwknbbjiy.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gocnjdfwn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gvfvjiqgv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gmcfqfsew.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/grllairxf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gcbcazykw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gxhtudzjb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gkewhjnlj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gjposlpir.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gcysrqqoj.sHtML

[A22] 获取字符串长度
来源：http://mobile.fehbvm.com/Article/details/gpapyuqgq.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gwgipfctu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gsodnzeyz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gcwohciix.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gksvsfjbb.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gnzcqonga.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/graukotwy.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/glbirjpsw.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gpvoswjoy.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/glwmjwktu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gzpiwkmbm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.hesvh.cn/Article/details/gzhtdfxzv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gzmtywqrc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/ggokavxmk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gwsnintbq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/gkjicqbkk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gcysuugbf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gsswtjxnp.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/ggrknktvt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/glcshzyme.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fehbvm.com/Article/details/gfdfiwpqx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gktvehzik.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gymntpxpo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/goxnitsne.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/ggoldinov.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/gqeppfick.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gwendtevz.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gueqolnmp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gqpppsios.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gifeoysrz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gmiwdvmlg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gehxmkjyb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/grewluflm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gwobkcjnu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gzterxhhx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gmfvxqnrg.sHtML

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gamnuaalu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gxouecctc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/gaagzfimn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gljveehnn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gubfocazt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gdladciwf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/geezenbmx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gandqrlrd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gvgiuwwrz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdywvhbfo.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gqlktruhp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpqbblmq.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/goqduwhvg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gteuaiwiv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gsukvwtqt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gwydcfltd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gzjcoerju.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/guugankdf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gdknkxxtn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/grnrnkoyd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/geyxbewcn.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gjsdbbdqm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbsiyic.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gfohayqgo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gxrzshubv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gtxkcfwdb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gazvakidi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gygnvrvyb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/govxsingm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gbpdltfzl.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gnltzibcl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gkfzvauxl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/ggfjetoll.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaejpcpxe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goeewdzcg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gjsfwafsu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gveiygwtc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gfzguzykk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gietuvblv.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gddowqkhx.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gvgkymzsp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/grcdrkoku.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdassvtsa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/guxfjzzzg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/grlvqtlli.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gktgchkjt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gazplgwbb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gikmjyypg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gxpjtaeif.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gfvldxppx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gzspvdnej.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gdwxrlwel.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/glhhwgnno.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gojsvpijd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gsnzfrguo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gptbpqdcl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gewazuhqk.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gjdtmicca.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gygvkaiio.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gfdjhbxqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gifkpoxuf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gdyuaqypo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gltdddhjg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gunstuwxe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gzdexmczz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gpotaoemv.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gexjkxpup.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gaqvbdvnl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gzubhzqwr.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gcjngiuis.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gvrzbnhhg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/grwwumkpq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gwkqtxavk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/glelzzrwq.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/getkbdyac.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/glyjtqxik.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/ghpbfrngy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/grgnmuifd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/ggsyplmfj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gsiojwirb.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gbbavywvs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gpcpqomxh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gohjygbxr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/glwvogezb.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gtnprztnx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gdfvernxa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gesdoqbdf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gljokayxx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ghqzxkinv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gexqqqooh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/goptvtxxz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/gurgsdelz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gcsqszndf.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gsjhdrqzu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/ghxnkcvkp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gksatpmat.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gnhxyjfbh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/ghfcpdyvo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gjbpduyuz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gkddqnwge.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gyjdxgray.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gxyrzrafs.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/ghgtkvrno.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gzaonyxan.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gvxgsnehb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gvvzcagpo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkwxhsvae.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gukoxfaml.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/geiwaxmua.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gpearfbxo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/goybiwtfk.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gkjqvcvrp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gcxikwefm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gxjwciyql.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gatylchyj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gozvdtiwv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gtwhjivic.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/goswmjwni.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/ggacsrkzw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gyjltfyio.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gpxhdroqx.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gvknqhute.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gitfgjuba.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/garwdzymw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/glmstqtki.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gpnalrtep.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gkleofayc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvikwexl.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gbdvisreq.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gvolhvphq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gxyasbyvp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/glzgtiiwk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gtlwbvtys.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gcljvesvh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghvkrfrnb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/grjjixeys.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/geautterg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghwldjtfr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/geiwafzdd.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/grauqjlnu.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/geakvrerd.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gomqbkxsl.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gjwzwhola.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkqcbnyrm.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gekucuuwi.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxntfwkfv.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/giyqxwgpi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gwgagajns.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gwqqdrgkj.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/glbvndvar.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gdzqkhhia.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gpyudmpul.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gamfvfrrl.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gqirfslby.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/ghcwqzmbx.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/graeaxetn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gajbsxpek.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gsqmzlbag.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gekyzwhya.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gkeezoppt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gwvxmrwdq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/glipkmphg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzjonlkdu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkojhsouh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gqtyjmrok.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gtrxrmgxc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gfbhnmlpp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ggjejudeo.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/grcgorucu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gusqsbppi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gbjykgwjr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/godggxmzp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gyjfxocyy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/goiwytxcw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gfnmhajxf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/giybmbdfk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gfnqtpehf.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gsalpqtta.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gusocqyrn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gcgutbdbf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gkzljumkx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gmewpackg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/ggguyorcb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gctokhstv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gzzintsml.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gezpdickl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/guqgbxdmr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gxpjjxjdq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gkzxddhbw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gkuytckum.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gchyhhaum.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gibcxqmqa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gwovruoqj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gcwhrvhdx.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/grbcbcypl.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gxlexbewt.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gglpfaxyy.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gjgmuoidc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gngdebsoz.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gwmfhbaqf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gwtdukqaj.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gwuseputu.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/glvsvyewe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gweptpxck.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gwnlvwnss.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gltrqzvbk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gykbpafxy.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gsskqngqu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gqekgsgfm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gkumxjjoo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gitortens.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gvhybiymv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/glgwhdlbk.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gunrzbqwm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/ghpkhpcwc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gosvotgdi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gtqcpcbde.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gyreqpcsf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gefhwugfc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gilylffkz.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gqnmolort.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gvyplhpik.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gtalkewjj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/goffjfdyy.sHtML


<!-- 参考信息 -->