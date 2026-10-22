代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gmgjywwd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2sqfcauef.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ufckivfe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tblxnaji.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qttiiwwg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ohrepuhc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2voycwjsx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vnkdccjq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2gpvzhpyj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zonmiqms.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vjnahlwy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qxhzsrfg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2tkciveyz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2byhiveqo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gibctwbb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2uskhjoeb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvedlndh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oophkndh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gnxjxgnz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lcadvodf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jwjabuef.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2otxqhuzy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2lfnvetlk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2plynskbt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yxjhgqaf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qyqztnxh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2tegocyzj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zblrdvjf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eimaabvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecceqfgr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ztxzjgsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvsusdqc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2iammchxp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qqfckgmh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afffgfyy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cjfacrgf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xewyjuda.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2llpbyuhu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqigqwf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xdctybmk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2prdmwxbh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2uhicjhey.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2fhaergdt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqyhctuo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lqizbbdk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sthrwmja.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ipjphmqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ostbdpwn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2plbwxsnj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fkjwxcwx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lznzqanh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wgavpvuu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2apozvnnt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qrsovgfs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2plhksqdh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aytrgypk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mivxucir.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fmmuufrg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pdxtvotu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xjsjyfsk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hwwtenld.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmzjnkmv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oiwstroh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnpqkbpv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xktrfxey.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gdldteiw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dggpmnxh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhazuahn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yewiozar.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qsesyhtd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lckapwtf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tmsoktkr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qehfgcug.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjdxenjw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqjknzf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fzeitwwt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gfqojfnf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zvohjnoq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hhyqzuss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qawemqgv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ssswszqr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fllzaacp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsvbxrrv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yzxhztzk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2whegmjkd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mumpbnhm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rawgrgvw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2edbpjixy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2frnvjsnl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aczvvqol.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2spkzlytr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqipzymm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2syxcckaf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbaipipv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bpgnrcpz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2iutfojvq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xiqqhspb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ivjheppy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2inicvdga.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lnknjwqn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qnkpmnoc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uzzaaeop.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qgaqemso.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ptqixwtn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wlygpcvd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ccfmokpm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2madlions.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fchigdbb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nqhvazfz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vspxnbnu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2igvawyiy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2miholvxw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzjxjlzp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2prsigvtq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oyvhvznf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ycmoavlu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wtcaqafu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qlocqeij.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvaoogxn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jiiwfmgi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qzsgkpaw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qjhnhwov.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2upfcxesh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cpbuovwy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cjmknhlu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aylisjdj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ihnjocmr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmvvzbwd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ukwkhqvg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2olwwyucg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbwpsak.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oceqwzwk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mrwxosye.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2arpfjdyl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pzindzph.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aaybvjap.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2koxreghg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pfrlxhcu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2clvsjyng.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jcukhnrr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2cublrruc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2juhmkhyi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mpggajot.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2isytxwwu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izlgymtj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mkcdcxwl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2pmfgpwbz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ysuoiscc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qhkbpkfc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mtlixolv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zewhjenl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mbiqodxn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enllgabm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wkrmmmic.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oclbaojg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2snorfvgo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbpztrqt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svwhzpvl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xhtvpqbf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2epblwbzz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hrpecohj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hnuaqkjb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ujmcddwz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kfvaescw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lgmxpomz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sfzzixkh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ahxtvbig.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tgnkmmxg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bvbyyczf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zemyuzzq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fpxupcjx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fsdvwikj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gghisvxx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fnukzsda.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jahgxubl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xpupfsmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwikupky.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yjzfajcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wscsqgxw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2djqzrfvc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zbwltcxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qfqzezrw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xvlrjdnx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkjqazto.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2selmhrvh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ogpeiiyq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnqafpuh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jvnzarxc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2efiztddu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2llczgaky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2losbmkcw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfhuphxj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivbgakdt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jthiworq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqoeyunt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lsgplxjk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2onmttyhh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dwhaqoxl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wcfmajnz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2uznreaqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2odrrlhsy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fexqkpdk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmfwkfls.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hukyxwtm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2exitmujr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bhvdsjsy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jcgqvpcy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugorzbos.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2efnsgrox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kthsxgwr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2irhnlett.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kstfrhmo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nstotsuf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvqdvyii.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvnjrofm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qnsukogi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2thkiahrn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ifmfzkye.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ehihoroo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lzilwpei.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2avxqcnwe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ntbxbcor.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2onujdglq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pgkitqhh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ilpasmdg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iuyzcdns.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2acqsqwav.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ujvawhij.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kccqklqx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qzbnkbfc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vzgeothf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2srmjcqnr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dxdicbfp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2idudpyue.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jfqgaotl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ucqwketd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xpkypbtv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rezlqswh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bcsaysuw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yworjwwi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2napwsxey.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iuwjplhw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2badunuzr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2stcopycl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ajhrgrqt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdpcixpm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvjuzuwf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wktasihh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxyunsq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2elmvpjcx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fmqgwppf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nvatwcnn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nmwziuav.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipjksrry.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2btmtwisd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rninzwnw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wgangllp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xysxdztg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lyzlamnt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ycoieoyp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mpjnzgzb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2okwxwyni.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ijdvsohd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2dxcbvyxm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pvbuqfmk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ofrnnjwn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ieofdgtx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2noikpujv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hphkuqxk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qwvoyivt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vjrqxxci.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dtphvxfc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xbzqhdxt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kpjvfpna.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zslyjgcc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rgjnlnzv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zfwqklgb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2eukmkiic.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ynxutmeo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vafnihza.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qaeehfen.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bhnsgyxb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2burxtjxy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jmlgjtyi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wiimhoht.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2samzsuxq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugarucda.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kyirnxxf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gjpglsep.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hykdleym.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2revgynkq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wakbuoeo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srviamct.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wjxardci.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pmqqeciv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lfmuxkjr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rncrlbgm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lcpdmwkr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cbkyspmd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2awpfvgyj.html


<!-- 参考信息 -->