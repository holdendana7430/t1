代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zqfsasex.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3adwnhosr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3prxlmjeq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkyxmts.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3csdcsdle.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3sybzcuwa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ohsiptkw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkxnjvy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wghqkdle.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3okosgvjc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zvcytwrl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xvpxhzte.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hfrvgghx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cmcvrqaq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jafflcfm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bbecnksq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3amqocqce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdenockg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3psryfasb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ictnpfht.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jyxjjdrb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3czpxbdqy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iorezboo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mbtfupvt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oyxbjkjg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iydulwfd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xabhzkbk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ewdscubp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vbtzxokh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jopkppcc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ikgnlxps.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3yoidvdoh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ripacedp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3onuvjvjz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dmrqbztt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3dnmsnmhs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qjeswaaa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gwoioowc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3qubmvxor.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qflmpzkt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmoewoez.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiuhcowf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yzbqsmhe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iihjlglr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fcnhkcvv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mtmzxaah.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gmmbzukq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jrpgasuv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3scdnjkfz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yzvhwhue.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tnwbazhw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkxdnsz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivazrghz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3eleonadu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjwczgz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mycepsus.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3svvosvus.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kpguelfv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lmfsyizx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bfhnicbr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngsxreqm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3oywikaxn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zuvxfete.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3poxzbcnw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlnpvrhy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ixgvdkod.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3snhgdqbp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ajkxenpo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqkvslqu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qmxmyblh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3virkqgdu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbdnrgog.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3liywhgvx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqtxulro.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3adunefwf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dmpbiqlp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ldpciyos.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zfwlmubk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fvgfngry.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmkdfqpa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zvmfqarj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3poilqocu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbgtkayv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3faamwblj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rljnsqjx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3amgbpjnf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ukijhdmi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3owvadehw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zsoffatv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aljgobbn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gfvzdthn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ibamqgyh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3erjhzojc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ufegvjwu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3voeiikcv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ntcbvxpg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3utkpxrxm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ccwkrjdm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3afyuwufl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhtnheb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3onfmkvvr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yswmjckd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3drtlmawd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vuwzswfy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nbmqghfp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hhudsshs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmqluteo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zzadibzy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cpmdeqko.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhbdgzc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3owwocyjc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ihamlhov.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3furxciag.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ielaghdi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vzolxfgs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3woqxbbem.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gnjewpgs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xipziehu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jqrzjfro.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nkcpodzz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3roqwhbqb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jrtxjtae.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ofrqcqyz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ppkenujv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iboqvkyi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3yetxmvvl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qnjxpkcr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yodlpnoi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jborgbuk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3forrmjjd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3flpjjefi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hpnziqfq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fsirhkpi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dauewkpu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gzvxxeqw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rbtrvdzt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3knbzhqyb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lzzesafn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ruilrnvo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uwurzhvz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wawfatvq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pasjszve.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hkeorppm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kcljuakj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuwghact.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkdfrgvu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rkvtpmom.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kepcianm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zkmxhpke.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kuxfeffr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gwpoahsa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nxuoiugi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zvnvketz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cddeefdq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qyrqpsis.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fwvsmhgo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pmdlazho.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyogezjg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ddihpuwx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3frhbioky.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rjopxfdr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pmrahzwe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3druqzobi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gaowiyjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcyxrwdi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3osecvnmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mobpcuwm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3doeiejav.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mbohkzzb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dszbihhw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3walfmgjr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpslptt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mwlsuvpi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fxawbsob.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cutlwfbv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zrvyqpig.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mtifelip.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3huekxsbu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzqnuhsg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wikgtaqi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhkdtqgt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rwkfjvcm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpvrsjvm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3khxccsko.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3cdgwclko.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hzglivxr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rmkmcgxi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oobcwdyr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kathkbnh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bqczygdm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3azjifsfb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3nmxtacie.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mjbranra.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vjdwjkkw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dsgtrhey.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3eqehbgqh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3daqpbmel.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdnmwujt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kwiqaxnm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3mexzkida.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qivlucob.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vttucgun.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kfrgrnjj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3akzozyab.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yjkivfno.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zqsdcjpt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tlfniclr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3owoqsuso.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hmktpvnx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lkgwrpop.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fsduvxxo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3skrjtudb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3flntjzld.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3yzvetzpx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kgkjkuve.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zlgyxvrx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uciortoi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3oulzofxt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zqqbtpfd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gvfexpzg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pgnjaewv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rudvpiyy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wwcdgptm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xjeqnqud.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hvxyapzv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yztqohik.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vfpkjqbp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3dyxzszti.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pltudqau.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3owyudokl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qxliurzr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tmlqrhcj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjsgrdhd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pljmofcj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpkzfcgz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3idsmgiej.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3oxbfvips.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3yvzsbdwb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3afpricfs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zpsmktld.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3asdqtbzz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bakjtdjg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qyqyyzst.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xgjzmbvz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vtojdhkq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mhgvwjeo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubkkcgst.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zkpmxnqt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rhpzatoi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3dfshmtcp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jwgfqgbv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xdyavbnm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xsjctfev.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lgfijdlf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lbggntdp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fiajglgo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lwtuhctt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jjvkgwjg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pkesobdl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3gkxidxtn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qddqndvq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mrwmjrpa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rqojofvo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vndoaiti.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3zdkshuhc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ukiusidi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lgzbibcu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hugvmjrl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hknguihz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3psonjbie.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wvtmyqdf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cttvnozw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xslgcdqv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hqxnhfkh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxhvgknn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3blqjxpvg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jmcappwz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgwsdgxc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vjlcspse.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wexucipb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cfqjifyn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vwlvjckw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tldennwd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ipfuwljp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yptmvcdx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ftiugnoi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xnfydyxm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ljdsmtpw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zsgdddfi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jtuwpzst.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jyplwitx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lzgzcezq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wgelejqn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xbjmagcd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bmlltxdn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zuadzecp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rpcraexh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atxddnuv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ywrpbrzp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fjxzzbzo.html


<!-- 参考信息 -->