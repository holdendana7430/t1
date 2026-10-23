代发 wailian999

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iaomftqj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ychqjzzp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3sqvufzau.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rrhmtetk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nszupqkl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ypdzovzl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ttggarev.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xjupmwkd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dtcwmlkp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dzhyjejj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dvfqeces.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vawmsjtw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnsnhqim.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3euftepxi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3veawxgpq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3izmjvbzo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gfwvrjoz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3obagsldb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vhlembvu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3dojmgkns.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ficldocn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxcwsijc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rsatdytu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3fdljilwd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gkcwrbtz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jroodosz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqmipok.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ahnudmfp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3olqrtwsx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kcndhwiz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ydzitfzt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3abctfysd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eqgjyqph.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vajnfuth.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fymhiefl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzncsxkc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gsidxkta.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3yfrfrmhl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3sgjxagrl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3txqpqyot.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3trmpsqmi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3foewffrq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3swxsngzo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3orpnyoxi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oaojyqle.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rrifswnt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fvqvldjn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zlmasexd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ujnwdbiy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmunhhpe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnzpvraz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfatqyvz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbjakoce.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kkgcerpq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3olxxjzga.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mumgjbka.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xybyzaxj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cutplepy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3aowunwre.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nocnhjgc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hdcpozza.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rxncumbx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jbovmjec.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qrckjtkp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tnjnnsor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azjkbfwv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mbkqignp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvjvbalm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hhzafmqn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ftgolhbw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3pqukcduy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kykgffmv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3syakkeoh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fefpipnt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wnucocel.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3thhgfyqs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qguseoie.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xiupruld.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3buslwjbs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kcmdgulo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pelaqghe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fihkdrcd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kbnfebqq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xkdttxms.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3woexdymz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cycojida.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3dglxxden.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xztweorl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcrncmeg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dxuulmjq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3etpwwecm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qxmbhjgi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3noxubrid.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ygcnxafh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jubjewis.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iouktkxr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3pzembarf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3muxfxgia.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaqgyhyw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fcyautre.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wskqfwka.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wubrlhsd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3gortfxst.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cumcjotm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ksfcnkcd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gcjoglbx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogufjptl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xdomielc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhkbssxs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lpabmmzi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3reijmhxf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3putjdjoe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocoafkhw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xcqfaarl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dgrcfqyo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fziedrak.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ahyamwyv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fywbsjvw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlqckeys.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ptmipdrg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zjmnhurj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mtjsvixm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lspkiqop.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftcyohjo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3omzvybjc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ogxguegh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuxcmajq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ebpjcuik.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mvixldwl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgahwrsa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgshagrv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3pbvsplbg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ntueqrzq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3edssiksu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mtxiszrv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yzloaedl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fdhgmagi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmpgxdoi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fkfxfpur.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mrfsyotd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fgzphwfy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3sypxvxsh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynlvtxgy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrpuqtp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hkkdiwpk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ribxwtux.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wzdagixa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gwcfgpsg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3crvopryp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rrxbsymy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kyzvkelp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgjvxls.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ytdhnshq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vyxffbpu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqmmtxxe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vkspwnfq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zaffbnna.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekrqemgn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3odbkwudw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3svubbuco.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xdgngqgb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iqocsmpr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3azcobwxo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3boktjwjp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jkiasxsu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lmjofzsj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zqiswthu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tpjngrab.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3umozictn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3mjackphw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vbdjbrfa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dlspotns.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3whpqizwl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3exqbemfi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wmxuletz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qiitsdhp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lpsxrbym.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nhomubyg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cpgadynl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wtmedlds.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alprnddg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qvxvgeer.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvjeekw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hgaggkuu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ctagvwrb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hducnoag.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3npisfarr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xjtubxok.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lguozbop.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3daacnurz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crgblutj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cogerjnb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3akcnrhrv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkrqxunc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3iwlvbwxa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nihsywpi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3aifknxsq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ixurlzdy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wwgehaek.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cggkghvx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ogmfawql.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jmeyyqmi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yicrexbd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ryqpalbw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3owggaliy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3upfukpdd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vhlbpydj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3woybyrkk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pxvaktvx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3akrxweam.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pkxzmitt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nwvtazum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojtahrub.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pygzetjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibsvyfvx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3caoyfbdc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vfiajfdi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqahypea.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jqllbsqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sqsnlxsj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obkcihxe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tfhdtmsl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lmwqvlay.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3giycmzdp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vmtfwrqh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xctmixuk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3khwuazwc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggcxmjwf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxotywqo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3czuggcpn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lukpfewm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3repcublf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xparpmyo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3maudlpbr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3soqaxxxc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3veyqajgp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ujtzmirp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3stttjwne.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgjhtjob.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bqsefxbc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3dssyxqpg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nwatyifu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ugtxmxse.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vkebtygo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wvuowhzp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tfseflck.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3pprglsjb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gvlrcmxt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvgxsqpm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rsnbuphb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jfxkrdjh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qzpacawp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qiohqlyb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kafjmtkr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3purkclyk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vqjzdebt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nvjisgoh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rtwrrimq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qdsbazum.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kmsejmsg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xyuxuckp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ihbncuos.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gfmjruma.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xvmmzrdc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lxmfnwbp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yvpmyydz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hzgljyrk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vdizuocu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qowyovze.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nnuqmwqf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zaoohxch.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dkkppqle.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dwuhynsd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uvaoulim.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ekoebdtf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3locschdr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hutgdqfw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3akwusntn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kdpjwwvi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vhhurbhl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnlenwhl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mduzpviz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckwfzwbw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dymfraac.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3iqlscuvx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jqpzmnjt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rvxusciv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xfecrenk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqzeezpj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xqojysou.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3apzooekr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jgihqage.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yscqiqns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhxgehr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3srmgltgr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3shwqkifc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3phcomniw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nabkpjlv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3azuztlhp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gsuvibaz.html


<!-- 参考信息 -->