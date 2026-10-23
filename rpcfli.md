代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kthugiwx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgdmnvly.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3eyluhvak.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tweirvln.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mtpaknwg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3grumvvte.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3iukbeyxg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qsupmrya.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xhamesko.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lvzoenxa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mlkharsu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tlwhjgjs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3syhzrsix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnlwyjnh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3voliqnqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcdjiuen.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vtrdmfbh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vqklmzuj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfrssmya.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3esioczvn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3whxfrjio.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kiteeopw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ajkdcjbe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3euzbnznm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cdtcqcoj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pfnxjjhu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3unqhgcpj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkvtokom.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cnfijhhy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3obdlcvym.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3adxttips.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ydmcdkwg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sarzbzmk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wydnkalo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vshxrzun.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hijzwqtb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swoueldi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urufdpyw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3neglpmpc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhncdkep.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wrojcatj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kpvygnba.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3djbmkcfk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vekvclgb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bsfnmylj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtfcdzuu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3argawbim.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xsitlcgy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngfcxtgi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yucmuday.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wstogpkf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxiiouuj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ugfomxpi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jjzglude.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqsqoqrz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtewuoep.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wtbevfrg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsryxemq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jgcykzmr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cdngoega.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3cylbytmc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ecfmmftc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3sbnwvlqd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wpuzyokk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rooxdqoh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjlulmzc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tywufqck.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jvujknhv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pxtkbzoe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcegtzvi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rbhkqwbl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hfqpiuxj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqrqli.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3caftsaaw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xbqipyab.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3atkfxgws.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3coyzmefr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3afztgxfx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmkzmhyd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3juuhxzwc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xfujroat.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3smkwekbd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kjfygwda.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zfnnrqnf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3facmistf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3btbtmxfe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3dlnpmoaw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cylxiald.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fbeqzujq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3oaghetjq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxukcsf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gofdtxkq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3guvkrosl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jphtnrzt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lznpaqrq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hnxarrmj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3guuqrtmy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3olfejznb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ahnidzdy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xvqxremn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rawmqkwt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pulicpwp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ntgiiaub.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3yknrsfrt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mdoqlvcp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvtiplwh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3icqgltvt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gpwuwbtw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3acxeqiep.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cltybuah.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mrqatxxp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3czqbwaac.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lftubnfv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lhngieel.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3oxqjgrge.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbgbagcq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3flveprcr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3glmkjikg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kukvdaxr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lhuphcuv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mvgtjzwa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3eanycsrb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3luwxflzb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hwnlxvoq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sbycikuq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tlimxakk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3prqsjhfj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qbwvxaum.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvnsxvv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3kswicqea.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3sihvhqih.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ynpwyycx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ildhymzf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3icaincqe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hnryjkwa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3czkymnwt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mnoshegq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bmbpwesz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kobggbsk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fpygsfma.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3himdcmnb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yifxvqyj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tewirrzx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jqucnfgj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xkkxmovp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rlyhuvpl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wretotcn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ogbgrnxb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ozhylsal.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sxsrtmka.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vjqcixxp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bsqbfdqz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fungcpwo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tiprilco.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xugoxwqj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ndwlqjey.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vyduzeod.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3sujstffs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3flqmfked.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cpjslwdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aoeokhvn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aihkbwbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzqisldw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3opupketl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jngzsrae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeqhahby.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xzqyjuzj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3czqzwues.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkhdtmku.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ltbixjgi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tgjtnxuo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pjuyncja.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqrmzgox.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3auxxxqxy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tfzcwqze.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fmumsxwu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omvptxhg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3lrbowgdg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3coyfjkdi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kizwuijf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3beatggmk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3clkywhrc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3sqynzsrt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dvtumnwf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yrkpuhay.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3leflgwyo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3actlvjxc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3iffdadjl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3huvgxqdo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3napoiqkc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3itpactyp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lrellfyk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ahqdvjop.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qmykjesc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3eqgfryrt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gkemucqq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3donebckp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uduiigfh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywhzoxsn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ykdicpkf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3stwwsejd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3uoczjspr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ulrouszi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3spookjkp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rbnsrrdr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ypmxupea.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zvotbmld.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ktjgsvxn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cneljfot.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rykzsapo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jisuzuow.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jjwzfbzy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pyvkpbkq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qwmxzeru.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rggopgzt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zexzgpcc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vmjsoyup.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3cjivvngb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xxbnzkwv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pftehosc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wmghhbnd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqqgjfu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3odfjevno.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hofzrvfk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mwzutjdr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mnljoctc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tnfmduyt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bcntwcbm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bloysayl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuyswten.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3szgaevjt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3eoowbdzd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3htvtanob.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ohcddwhp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3unqijujv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dsqbvgim.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yikdpgka.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rjvgzdat.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ttootdrg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uggbiuts.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjsrysq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgnkfdfn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nhzxjtag.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wcozsnka.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mcjivxpt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3oakvxgsy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bwyiccop.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lajrynmf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kywcjtud.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yhaiiduw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xvikyqnw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bpmvvwfk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gobkkxpz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bhavajzf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3oizupvxc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gcldwxeq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hzigqmyp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wfhekuoy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3apynxuzd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3oaqmymxa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tnwdludi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ejxjpyqy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ssgqmiyc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3amglskqs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lrtyiuqv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lettljzm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3unfijupv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3aohgofrl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3lqqslulp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hnjrrhck.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lqaeatsw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3yxiikyqn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3azwovdnn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoqpskcp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wldmxird.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxokkyj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bhaowitv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dtrimglm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3aykxbcjn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3snfxoijl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwnfetoj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3difrtpnd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nqmaqgup.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mrhyhpdi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3awfaqved.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mhbwonfa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fmygqstp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xpgbpmpp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vhnvygyn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wqvnwiea.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qzldhnfw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ihvijlda.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lzqfdbsy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bjunsyax.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qbhbyriv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ptiwxpgf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zumnvmza.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vsvmvbmi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wwxhwjps.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ilcazodw.html


<!-- 参考信息 -->