代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ijmrfbvw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3iueybvql.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ttkifrgi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3oqchgalg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3nqnhyovu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bdoyaqdp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbnwazx.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jndbhnqe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tlnzdigz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tjawlpjm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3buzlbdna.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3oyvdotvc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wrvhlmsq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pxjwcbrb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3moafwbwq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jxpdmrfe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jbzjwzxy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qpjihkqb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vmagajgf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sutqxwof.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3sexfjjhc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eejzetts.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3audakyji.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwprbyys.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3djsctjvh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ohawibcc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cegquoer.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kuqsmumc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zwxvcllg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wcfpbijo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jkallzfy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3syjbejjg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndvtmniu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wjrpvzfl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lzfuatge.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vnavsfdb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3kypjxhnt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zacqzoga.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uxgahacw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jkrgfujf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3kxpbbeqn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3oldhvsif.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ofzszcmh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ahfnmqtu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjrzjczz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbschynw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3opnlkquq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkeakflq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3idxsxody.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fcefwbhk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3nukhjndy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3becvkrow.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pirnhhik.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cgsttvaz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3wdkgscmp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pntoxyvk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ghnlqkha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3webldcmo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bjwdaibk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvmxhhnq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nfptciid.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eonesrks.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sclojnvn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3etvfeqru.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pxcmqqlp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ifsndinm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rafklmvc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wrzdwydq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vuwuwiye.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dorcvghi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hzwwyeus.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zkjvlxdb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dvpwtfpe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3frmnisqr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qtthvkfj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mvcjllgx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jxmdbwgy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qfsbzzgd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kzcyooaa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vudpncjt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bxkdwfdh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kpfcpnqe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3joqjqjba.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybbjmhmq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3opzbknvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wcypxbqu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3httvvsdr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3meulorez.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lepelauy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cbpkstao.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tcowweou.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3igcxfqrx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wellzrvs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pmyrtwjx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ccpdnias.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqghaevn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ocxffcha.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bxedffla.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tlhgrhft.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sltaobma.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjygmdj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3iqwridcp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3hggsfrwu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lpzjdtlk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxdbwfwc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qqnyurlc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pqcauqkz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrzgfrso.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3khxozrmt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xhiemrif.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekxquekc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vigycokp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ealvhrlj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3baisehne.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tqdybsmq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3trltusqf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxtfnjoz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gucnukug.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlcrfyjo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcbxyiuk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3oxauwdxd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mqgitrxu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3obszorkh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3oehslomc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3nqldqxrr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qfkyidqq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xqhuqxfb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3immwqpfq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3udbrdoyh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yuhnjxoc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kffhofdv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jozgrivu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fxchgdwi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lecshtvi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ggjxntyu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3enhaimof.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xvijeckf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3immlmeve.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vtvkaern.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wcjkozab.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqmlfbes.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yhtrziwt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zmzipjri.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mdetfvzg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xqinjxgl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bvxkrkoe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ldwgozrz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3alornkcu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3djromiiy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3aubtpvaa.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ijhlmztu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mjckzxnz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tbbmteju.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3csnvnjza.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ypzwgwhx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ttsppqjw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3anysvxhy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dwejjjcd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kumorlba.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pomcncaf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zgwqhqwh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3uvpsdqpy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzqrbar.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eslxpsvn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxtazczd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tqwbnaux.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jsuhiijm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3krtjmbna.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fdkwbhbk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qhkrqubm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3znwnmmnt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3szicrmep.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nugjcbdb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3szsxirud.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pvjecubu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wsiphfkv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bfobreqg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gdcjnylz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3htlqmbll.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ygsdwvpa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nqhfmvbh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfpfwuvx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsvamxp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqtfocws.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwpgthtw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3borwawsx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xaicpoqk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3privbrym.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ualnioks.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wnqisutt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3olvflida.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3igkqeqjl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gaffdknv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qjagdjjo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oualdfdg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wowqyyvu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nvuvmxjx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hjvcoiyw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vzqjjjxk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qbnjoowc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cffywvmf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xcxafayt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3inolkfus.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pemokxbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pburvtex.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yiahkzve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhhevwob.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqckcheu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mwholhyb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apcrmphp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysmjetgk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3myhwatpy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oavdavpa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lmhbblbq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pcxwsenp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3umzbswwm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zcybwwlo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3lzcrjdig.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3opltcoil.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtpopgsg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpsphkk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bwnrzqyu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tffgvqif.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bfoserzd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jtyjrqfq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tijuqesm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pnypczci.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ljutgqpr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzmqefuh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvzhxbjd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuikwsqi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dbymfkzi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3anxasafo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pglkakbd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dcjkziyt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzswnfxs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xdqwcggc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3niaikfti.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fanjlnmk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uigukxty.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vdymkilm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rmqgyhjz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrtdyon.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cpogjaaw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jiwoesel.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nqmpwioo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xhjavrte.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wuukzuls.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ntlfwgqi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ngjeqfyj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dzjtkrmq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hivrrjfk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3boiskluh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ltexgqmk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jpefrmry.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3btksmijp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3prpcckpy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qqjgldvf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bvlzgiaf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3obyluagb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kgvxihto.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jbcuqutr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3yakmgclb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nafecden.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qkioldfc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3roqtbqjm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwjnvcvh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jxvfwnev.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3nftxjzle.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tnwefddg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ifxtqyma.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kvuypilv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3btrzgooe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xyeeypeu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fduhvuug.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sixuvoqu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rqvbhuql.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3biaaqori.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lucbdkpk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pkbyylfd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zilsgias.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ggghilwe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jylksnjt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ccgqyznt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksmtbqdp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3uzvcfeuq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdiwedhk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ifqkddwn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3igkggdzj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ofdfehgm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dgtjuzha.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xedwgboh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qmoaoynm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mrlfaelj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3plkxnive.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qvszgqhd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ohgafmog.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zzillcfi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fxwbafiy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ggiqypfc.html


<!-- 参考信息 -->