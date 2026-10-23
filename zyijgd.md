代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3rtwbvbqv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3spfrwdyb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3agpawynu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yqydrahw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcddhqkw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmrwqmdd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yajbczny.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3eqtnvzdt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zzqjgzjb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ubnquphg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3udkqzfnn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3othctlix.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tbzswhux.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3egiazjmj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjcjbgdy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wxvlpfmy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pcdfjszn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fptvdleo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3brrxpyfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfqdjxyk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gqwmtnci.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qpugrdrd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtehlbiy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fnvzmlpw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ahcngbak.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dammvsmd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lcxyjyqq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dljpujbu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ysmmmfpx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xmzbhzzu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fidhgtcl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aviwuyiz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3akwprbba.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3szorbgvv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3omfqbaru.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ybccpaou.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nirxgbjz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pdodmhla.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3glqskeco.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3azmczimx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tdbrxdvf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztqjyote.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nugbuzdg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulggtyly.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jszqskdx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rhmmgwip.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3orfkikdc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3httodhpy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3bwztjvmt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yyujdqdi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ocwidkxq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqilbhql.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tiqybujz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mbwaiwea.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jsaikfyp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vpngwofb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3akhipuur.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3desjybva.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3evgryhdq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vxbvuuew.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihbtlzwb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkhnuhdb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fccbbcrm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qddujaga.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkzdeomr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3szsazozw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3etzyqpba.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yqznhbxl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3paznjqrq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3thommiom.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wglkwfwt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfwrytwv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pzpsrjjx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3nhrqpzvc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wseiagyu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3prcptear.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eamfwmqr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xsbxtzgz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3davjieqs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xqtggbba.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nujjikpf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kcwdmegq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lrlimavo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ttoymdyt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3keimstkr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3damxdljh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dhlkwfrd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pxrseiib.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ipfogtrz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3naunxchz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xvarufyp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpmlxavp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3btuqauwh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rrhuenan.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulhiznfx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3etzkybls.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bfqytfnu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3soqubkfw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bobahixj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lxurgwfm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vbdpoemy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mlioippf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mobrzadg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hwuygkgz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mjziicpo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jlkrhxuw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtuieqqz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3onzsvkbp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ofsjujfg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nntmalxw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fhardcyb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3pquaoxnu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xtxcbtmx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fvlikyoa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bkzmqstg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3syldaruk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hoowzhyp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zexztjqd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pevustfw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zceotiva.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qbdyhjkc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vstdqksb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3znnskoep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3idbuiqbf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ozjudmmp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hpseypop.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rprczouo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dedmdmpv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qhhdtrcq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3shyiibgd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dnuohwzk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpozfydb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqsblgpe.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dpgejbuw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tnvefwnv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tvxwcste.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zrbotcnw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ahznmblp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pzxdusdq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dawerxrc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ivdofbbr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ywdqssqj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3djpgctyi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3dbdrbfxc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvrnnrbx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fxfiuqks.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wfedvkst.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yduzdkjj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jcttxjvg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jqltljhu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iteaznxy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fppolrhe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itnethxh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bviiptdv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3raewljsh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rznmziac.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wdwzqltv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxnyinmd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hxgbiqgs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wuorzbrs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vrgfhboj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tfpjmahm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vvhezdug.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rxrowdrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glakhmuo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ndrtzekd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzjmlbps.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bptohjna.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3sqzpizjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fcxddxqt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rsqfbodd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lvcozskb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tycmnnhm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3miivppiv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ebkjehjc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzeteseq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xaeagcba.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3axqpbuja.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bajqlngg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3faqzniga.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vaxbzxuu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3lvgugzcz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3websypjk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zqiobxgv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jxtufdwp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vdovdrmm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3encyfusk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3efnjxfpi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ompdrste.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3izugbzmo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ymszicch.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3doubylje.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kplarcws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sjtljaqy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ubrkuxeh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3oiaonmhe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pvhxfyll.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcrjquzz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3debidxpk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jtvgwlkr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rvpxcmqm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfntviys.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fesybmcs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kufkulad.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fksfjoxa.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3epxcnsdl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tasgqrpo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dmepmsph.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cfarnbog.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ymnmcnlt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cmvemrfz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nukmjmje.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3puseneyl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3exctdfdb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sytwccfc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zxtuogql.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ovejwljd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tsyiwrlk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vjaxzyjk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3sabwojql.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rjkffsui.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rdtfiboq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ynsfvrwo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rsgybnyw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3oqgjljdm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dfenbjng.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wneaiipy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3cxvgwlwe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mdkwzlew.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dmozwngc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3lpufaahh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3djwnabom.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyeymhng.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfpiqwv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pstpaxwj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3iryzlfzf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mmaxupnq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3eaehpkmw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3krfszafz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rbnoyhhe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rmgxzvrg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwpssnad.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3akzzvuvs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mygktvdw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctwllctm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nritjlqh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jkpcfjzw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vqbwezpt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3sjzjnool.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3osqwpcnk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gxrkdtwz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3awllkodi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3opjvbleh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eugnmfdy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wnndstsw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hlwdwktb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3knwqumyg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uuitgefx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lkiodoqj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3oflgjddc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3owbrzjth.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jxoyjkev.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vcfeokgr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ahsvsoll.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rpoapbwb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3eposfkji.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kcptwlcn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3syqguqkb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3evrmjiie.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xyuhjbpa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ouvsnosg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tsjluwbs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qndumtud.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kjgdvwiv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vepdgegv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3cqxcxcqg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bassmluv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdoudco.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gfbltbiz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3esakicwj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ubfkkmcj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wzxdleqk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hrpevdgg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hgzrxjvx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dcncqaae.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3marzwmdx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tcnnhpef.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3drmtjuya.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3frgjgwwi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cmgamlcj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jmxfxhhz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ttazyyvm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tjwltaut.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgchgrsr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3arclrsls.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qggfbtra.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpqwrngr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tggmppwz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lvvqbosr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ewjhrvhq.html


<!-- 参考信息 -->