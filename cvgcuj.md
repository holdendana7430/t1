代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rynkaefx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hpelsovl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lkigtizw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qzotumtw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ovjzkqzp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3nvfkicvn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mzcclwwn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vjreccdw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3luzcjhvv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zrerwyas.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hsujrula.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3grewxatq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pwfzvejj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nxrmjhgx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qkpoadvk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3smjyvgpd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ijnosbui.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ciborazj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3nbrzrema.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xmplerge.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zzdgrigb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dnyslotg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3osjyutby.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ooimtarj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hxeyymqs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bmorqjrp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ebzbcnaf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxzrwwbu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3edetzsyl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3txbhzdrc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uoeijzlr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuoiukew.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nfggpdzx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gidqzzwc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gddchtuz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jxqbuant.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3atgxfhfs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dreqzlaq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kcrasfrh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kzjazofr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmtztgqh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3iqjldlwe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3afponzpb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3latukkwc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3dkoqsejr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgoxsrcx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yaerlxiw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wofkrhmm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3fraxkxeg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3luaxhcla.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jwtpmzyw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cfwujjeh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3eamoabec.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3joupuddh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vafngqhy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3swduuguk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mmytscfe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3readfvcr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fzqqdhzs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gvwyuxga.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tanzoype.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxuiqe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xogowygp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljaocubb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cvnbhgxe.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wukljmnt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3iiewirln.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sofpsycq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kbbbdcfh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bcocnbpy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3osyyiypn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nemyyxrb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ecyhbswx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fcurxshb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gqnvvekl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mhvyobub.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lkfzbtoc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wrvmdjxl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3meuskhig.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3nzhjmhlr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3bhzsfkrd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3onbispbd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3hnfnluql.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3oofujpqe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vsycyymu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcfmcwmo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owaxynpu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mozyzepl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kmzlmucp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nuudbxal.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qkkkgndy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwsrppnb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgcwhik.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3abqpbxqu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ttbftujd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vaauvtql.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3izqkvoum.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fyrdleiw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3epletgym.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycihdjsw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sqnnkuva.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3sfhpgwjb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fuzbnyfk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wwvcpgej.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztmykmkk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mtdoqumq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ydyxebcc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3obixrtyi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkenpxaq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hntjijqj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3huibikum.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uooduttj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkucmxfq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfgqcqpo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3koonncia.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wmboqhfv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rkcwhfzh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3akbquumf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wcdbuukw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pomoolzm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pomenxwy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3orqmudbs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wgqatuva.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mdscvxwv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lclvtomd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tvqqizpq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3erbimgqi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3wpfsaqzj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rryodyup.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vuiaumgp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tzsnejdu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mbovwsjd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hxyjrnfq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tuofjqzi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jxphrhzk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ltqdplfc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3udriwrux.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipldozfa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3volsmyxb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxavyyxy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajxwcvov.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxxcucjk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3chemptpi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3khdkzmra.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiuwiktp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mjaizogj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nplmutmm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gxjwoadm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jwrsgdok.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3waiqhjao.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsbatybx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3awfxskow.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jrkoovft.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvafcinu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3sjsukqaa.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3iybhpeqw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xyxqachi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uscahfnn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bsogwdyt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zblkthft.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fslyiasc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mogewlom.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gjxtoxyx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hiyndlhl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wqyhmvpg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tikimhol.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cworbadz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qshxkjsm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfauktx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gizqwxay.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wsrbmcdl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qnkcmydv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rrzoecrj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ipegopch.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zcytddfd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbrmacp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wplagblr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rpvhzujj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3sjauvmez.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqykihe.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hpamyjbm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kwiobloq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hjbxskax.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3anqkpexq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qteojfaa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sxbhdskw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cchdbdch.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ihwnwrka.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtojcizi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwniwdyq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3xvjyfdea.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3cftgmahj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kwzvxjfp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3shkxikhb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3byhzaagl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3biwrqmpp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mqmpupqs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kqprlclk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ydqqvian.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rajlndtc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fqbpfhhy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3eubfzxqk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dvytvzcc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vaqvlfte.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wivxjvke.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qqsxyvbl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qcyjvqdx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mqivuzus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzfynamq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3etwagqyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdettqkr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fefvbynv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3agzatbjw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lidlvxpk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdfdqpot.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rrxyejon.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgzwpspt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3farjaqgt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3tjsdfqii.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ldmrbwmv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3oalynxhc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xmslcywj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wqauzcll.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fybfvwkq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3idsarzrx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3gqnwbuwf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnlaptin.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ptxsbkja.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nwxycszv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cdiupriq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3oygahfau.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkygoaok.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jogvnvjl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3svrozogw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjzbtyto.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3cgpzdpbg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3yunlfkqj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ibhtxdpm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3swjaxkjy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tpdfaspw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3uvedtkyb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3imbiiixf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kimdjgky.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lhhmbtef.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cbzwfhun.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kfhgcykp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3olnjijid.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3difyldfr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3txfeunvp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bszuawln.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fmcjykqt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3efvlqsvy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cxidsrcg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hvhbvomi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ikcgchub.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gdrlectx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fqjdxbsd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wsaudmll.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3oarsimkg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nielubcj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kowwcxjq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3typkplhm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gepabiia.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tcfvelwp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zaaysphb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3soytjyra.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3obvgtnoo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxnpptyy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3whonuaac.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3liypukbe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvnsdchf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ufzeyidu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zgnybhfi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ecqbvryi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ptsdoxfn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3msxnyfea.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdpieoyo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wplfeyly.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzjddfym.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pvjoacel.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3natoihll.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqrzhxyw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvyvjtpy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3slnabwpg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cewskifk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qmggxywu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kvweewcr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cbvxuacl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciiywmlw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3etlrheow.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3puwkpsny.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ywlsbclt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gjgzcurn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yekyodby.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3siqihymf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3iuwckcdv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jhjcsmbb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ttcohlud.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ogtxfusp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3knrvaaju.html


<!-- 参考信息 -->