代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tvyihbyl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vaobbjtv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mdgtfhco.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qyftiiff.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aayqinsg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3yhktcvau.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hqcxuxlw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jrjjublk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mayfjzhq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qdvofyoc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3qokrylha.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3raurdvun.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ctwjolsj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qoesesmz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3bupewrii.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wwnecmgw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3uakkgwnk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ivzypyvs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbukiwop.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlpvwter.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ouylihfp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3grnfiuwz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rpwqngxb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3sieywyrn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hsrdoobv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ygimfpeq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3clrjqrkr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dmrpvsxn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3reswydys.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nlugcsdv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gjbprswj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ixkfltjq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qgoyydge.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ukrnmvmz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3qjxgrhca.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lkuawicc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pdszhkjt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3byyryxpe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gvcpuvwa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tuojuswv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oracnxtx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vptcgtph.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wsykogkm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ilokxdgo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpzjoqjz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pcolbkfa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xojalhqr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xcfmuoxq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ipgbfdsl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mwkngqkj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pjjcwhma.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3trfticah.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vsheviac.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrugtoy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxznnaev.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mfinvrwt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mycxniha.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3swrvqbrx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3tnvynvcg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3egbkdjky.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mocccytw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cpumwdmf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zpoojtvh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pzpvewtw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3oyhfzvep.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qerdainz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yiocclhj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aomgsymm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xpkllbpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehyysthl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3plekqfuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzszzvzd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jhfkjvdy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sdulovow.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqcmzukz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ztyillzn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sgxsharg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aunszumr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3pfsdrwtt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jacgrxiy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iwdujkik.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3omaznocf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qlqpudov.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3fyitoiab.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3boxjzaoi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3onhanwhh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lywichwm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3kvemwenq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uklrubxf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yaeovxoo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dkhwwhzr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bdzeadjj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uucwvofu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjdhngib.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uigxpfsb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okytsbzf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nsuiuapz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3moyqfgjz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zjcxgryz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eoyowcck.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmqeqog.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gcibnhux.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3objtcnkq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wbjrhimt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3durdswhl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3aondwwxo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vzpnxzfh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3olrcuubk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3trfowpnx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zhxyzsej.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3dtnwqhfr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvizhuqt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gklihqbh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rnjmmxni.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gumxtcfh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3cqewlrou.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3yqzaxjkq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sknkadug.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ffonseif.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tvlvwxxp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgfmmpbp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nfredetr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lftwtdoy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3idbycdpm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fnfcrjod.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3etngecfu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3efvvfaih.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gytbfaef.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ktagyejr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bcqipkpc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qqxdeeow.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpnnewcg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mdttwpjq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wyptfyxg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fipfmwbp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zzmlzslv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hwhztewm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dlfwzimw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hcnkenqe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3khmoljux.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bfmvvhgb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lbbbuuez.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3idoomuda.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iexiabgw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3btntvgoy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3feafnbai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bedosgyf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvnpkdk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xqcjxycl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3admajfbs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zyozhank.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3paiwifbe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwvyvuhw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3agjxthfu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jlkxeuol.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcdqiusk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tkspdamu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gihehfog.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvmkbgud.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mcysclbc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vriegtoz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qpvvyrbf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3limagfsy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3dxrulpxy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3aqqcvhyg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wvdkoryh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mpnhcxmx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3brqljdad.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jgdxrjxk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nfaetvid.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwlahihd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fascruke.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tieupcyw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bfuztzlv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dxpfueea.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3finvwdsz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iopnawgz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hgsyptrd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3edawvzlf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nlctgdva.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lrknvucx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tiymkzkl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pftaaylw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygpzffiv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bvvpspog.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mfkeygkk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ujkzfvfn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3umpxczjn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xqahsbsj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wujuwapr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xkelhswh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rbaokjal.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uhhiwaqq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqaveeml.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnjfinn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qhuhswml.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ovtjuvya.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xlnmsztq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xeguzgnu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3csbggutz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3azeswrfj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vrmfmqwl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ixeklqhg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3scoerios.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ddrfyyqh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qgywijmz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nwvmqqtw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nbfzvpza.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3iwvhdbfn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hwyjdgea.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mqixutnm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3masnypzi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uxmoqluu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mvymhbup.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jdbiurxh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qhmizmok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvochnky.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iidljgin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sofdludj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iydsyllp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eurjcsxv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vwnfefrl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvrhrioy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kijxxgtz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cqnxlwho.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yovoiwpd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rcpqphch.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3skrdxket.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jgmfxooh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dtbffkqk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mdllfvgw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dqohncah.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjqikktg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qqqfauzm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lztbbvbj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dxykapuv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qbtpcmyb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ukhqejzb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pqswqqgu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktftqorp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozltmmtv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nozeeibk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cityzfie.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sgqgqinw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gjqqwcwh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rzovuioq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3owsjnpuw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ccocvtux.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3drrsohur.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ycjrdofz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zvppkdma.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3maqpshcu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qntqpgeq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjcpjtcm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rsfwralg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rttawisw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tkagfjbs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3vqmkpznl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sweiplor.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gfyldfxd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zmhjlkdv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bgtkacih.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3byjhvayr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wahjdcvz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3crlzcjpl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vqydcdjw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xpamsnog.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rjhxljbz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3njtmwdeb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bkucwrfp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jhklinzf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3elrngahl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3etfagvud.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ufpfzhay.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ytzeqzoe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bxkoihfj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ivwzcfpb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nczmupfk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qxpprwgz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3aevfqzrw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3daldtdpj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mkgvtslx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3imzjvocl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3semcuoex.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcyjmfyg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3itbwjkyl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3utfghepn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dxletrxj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ogblgzjp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xkblstyb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uyqegnen.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bwprjjil.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvuhknjy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hrohdflf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gxdvkfji.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mjzufxjb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cgyjocbi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zxtbpflb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmcimvql.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vnwhoirz.html


<!-- 参考信息 -->