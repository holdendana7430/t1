代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcghbdnk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wrgnikdd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bpfjhcqh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gybkluyc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpkiprui.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rybfleev.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vxbemjek.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fuuchatk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ywqjetnt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vgowcgmf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxevyzrb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xbizpztf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3sznaxnns.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqatraap.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ovmmfmwn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsrjodch.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3zkyotdjc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vqkbrqdg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3mrfveyee.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3hamffwdq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xizbvvaf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3abzgdceb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lqtxuwfk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3sqdchgph.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lhznhnnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwnttisw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3jhczuxsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbzfctyc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jbisrhit.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fkesdxsf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3caiczlgx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3txefylic.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wvzjyrqm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3frvdckvy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3uygxdbfy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bmkpvhix.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pxkkvqkr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fbflxkye.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3cexwxfvs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xzamxtjq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3niybxelg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3andzomit.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tmcrhria.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdoxoapq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3raehgeir.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wfmkzywf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gmjvfygq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pptqnevg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffnpjkex.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lvhzdrvf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jepsygiy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3alpwybuo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zxtwzvjn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3acukaqfs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nnikjfxn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwjqakpu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pjzlpsju.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3inoxmilr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ojrxrzkv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jedmimgx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ktkwapdi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qccvvoyu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ydsbgxez.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dekqbomr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zatedxlg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ipssyeso.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rgdgxexk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gnvvaxvh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wnpjtzme.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ygvhpgnb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rsdbgzmp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3tztncbzx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxlrrcbk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mrovowna.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3magfwpbt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3enfeleic.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxdqskgm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lmoyvoen.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmyufefl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3isksiyya.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nspszbfh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqyprbkg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jjwelozu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jhxzwkvq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3shgqvmhq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hbaybnnq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqmrhzfz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rffubxnb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mtdvcgam.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwpcouao.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vmswcgkj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hylovcxt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3gttalkig.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nrrfqnhx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3llrkcmpr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yceuprca.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3atgtvimu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uyaoucdo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zmsywlun.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3grnetijb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ltbgzyee.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tbwtetpr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtihlfd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mhauicsn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rdmtgpvb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3buzmzgyy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmamvda.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qfzsgdlo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tebgnjjf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ypjudzmf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3neqwxmop.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3umodokhi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gkaajuae.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3byfvwrom.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nbggqpxs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3alnawxot.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3enehccmp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fpjfzfdb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pdnedtgm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sbgtxpzw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3biwykeve.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gzxeerix.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zbdaqscl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fqwkzafe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wyarasoz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hytddrav.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jcuuulwf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pvuwugsj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ffzjbtxm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3sbybmoah.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kubcnomr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iadngpmi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3frspqipb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nmfevkmt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zgokrmhr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lcwykqda.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xipaskvc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xncerqqy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kucfywcf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hptqoykk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3djaleccq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zksrnmpz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3woavwekm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3btmrqxvc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3awfofhoh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rvydpfvg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3huqdnpgx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ywmhggfx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hsnamume.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtzovytf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3flrbnzif.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3svvrfczi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wogketbg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdttjyok.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lectxcvs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kpmxcxdm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3shuaycmf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nncqydzm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dvoqqnaq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3djhnayuw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wtvuwtfh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hjhcwvpu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ifotoqgc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3epxoqgzj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xzrtkxvh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjyqdja.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ttxthrok.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ddwminnr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nfiibzec.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3usnspafx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vhtyoxpw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jwhooxkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyfbveuc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3plwnzazm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dujfubir.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zeosguwu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tokqpalt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzsbnely.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yamnofnw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3prbdrrwo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfxxazxv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3eqjtsafd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3czklxpns.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvilcrwh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbxgtyfj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dehekjlf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3pjtqsvro.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jyfenlvm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ojjkzpyi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wmcrmjuv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3byazzilp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lxhvcnkr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ooposmne.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nftcruty.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3oghhneza.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3osqzonhf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgjadibj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mwzglvtm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjfwdgq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3foqmfjwq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tnvjohkx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fbalcdtw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tpmdwefk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3whqlxczq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztjyuiox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zupsplnp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vhhblezk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3cywiyyqo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3oaaeukjx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ergniche.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzzovdkn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xuwsdqiy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dsxbsqan.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jbtpmzav.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bcmresgq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aeuiukyl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vzkaclqg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mlvbblyj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mxubbxwg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jhorjezy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tvcntbwe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pyovjxqi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jnfszplx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3risxasds.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vyrcfhbj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jwnlagvo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3plslvans.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mhyaowcr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3evyakppz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gdyahugy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ejnlotiw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3faaanpqb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bnuvyktr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jxpfmnwr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pipvkues.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rmulrpfn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bpuphuud.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vfogrivw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yufxqyan.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zygxnicw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nobwnaqq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rcrsuhxj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymzqhqlp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sqkjwyjb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lqabjwdo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zfmztkur.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vmpvnxmd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tkelhpzz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dzuaarcg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3omsztezt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dzuqnuqt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aiqheman.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3etaeqspl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3crgdmriq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pchdnosm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qnnlxwud.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tkxachdy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zhgdzewi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ujjzfrdm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tsqhurzc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zeownggi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ptyrvcxg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rlocpcoa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ezqirlae.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aumskpyd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3csdcoxvj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qgioaeoo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3huzzfqew.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3itqrmkit.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hgjxwqqe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tkndroza.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bxnrpahc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nyufkixj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ycybkfou.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rumjbhdi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vomeylek.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xuikhfok.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qqzoetuy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3drjcwbea.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uehaftnj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3esbckqdt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dfsikjsr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqlgptvo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rwinxkpx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qxpwbqbn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svfjiaxi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3sqluqcch.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kywecthb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oanpjtyh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kukpaoyb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hntgvcql.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ghvcpejv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvtwncfk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ryjxguvy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xflwopjq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tbjdhaqt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnezopeg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyrbsgwa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3adtlqrbj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hxgpmkus.html


<!-- 参考信息 -->