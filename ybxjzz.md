代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3txexhbbo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eegbfhyg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3btyyklji.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hgaczhna.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3faenewnx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lrwqjavl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jmnxyrzf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecqqgzvd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ozydmfck.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wsjcvjsl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3guqlyufb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyobcmf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gafaoasf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3owfmvqfx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jvueicif.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wxoizfpx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbajedos.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmypptfs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hgrmxhlr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ocrjvcjz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zkzrlxop.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nputayub.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zrnceasy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bxrnoyie.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wphocwxa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3okzvmjcb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xihabkzu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eojdipws.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lsbmhqtc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dvvkgyed.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nuqipppp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfeubbdl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3clifybzj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kvvisemn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhbiptoo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jixivstt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztonoecx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gezychzh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zmolglbo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3chpkyoln.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdputoeb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qkicognp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nesylgkx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sioztlee.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3skoulnjo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hicneuoh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oontwjst.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytvrsitk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqqvsfa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpnnxzgl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3avhscwdj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qftuylkw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gosurmnn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3flzcirxp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3leubwvdq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfyeekyl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ijnkgimn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vezqaktf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nndjrmzi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xujjwlst.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uhybzybz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rlxljyet.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xpkvpzrb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bixjlgop.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rhlduuao.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pxssxayd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wzgmhziw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kmumfyxw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tkdpqciu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lxjhjolx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zhffcumb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3deuujajn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmzwmfns.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kobngyls.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3snmzyulb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gfllvrfm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mehlgdhb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3otauyzpx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qbrofnda.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3opfapwvt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ptbdngxw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3unoxaobu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhxqimmy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ucpwlodw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tqxafhiy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjsanlhd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ouwtmfia.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mpfgcmcg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ygiflicg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cqovljui.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zgebvomt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3sdpsvzrr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3beakeqew.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xirbaqfr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3efttvrsq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yerqhnrw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ctyxrxlu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3idyebohq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zuvjtkxz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnlbmpy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3svbijeya.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xahkfavk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cjnzhvhg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ponkhhou.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3erflgxtg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ddrqinbs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3eqinwdww.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ckjbfptf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sxwlmmkl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bdrcssms.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zgfnpoer.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dsagytos.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zbwdcpmr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3aioqmwxw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3uipjajiv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3afeevqad.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmykfeep.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3unnmyrie.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahcpndbk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pwsiyzoc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3amkcqlqc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tpwxwrxi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kbnabtow.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tmeqjxkj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lryrtdnt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kjzfsarv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tnvvifir.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kccayxor.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3izqwygqj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ywuetusf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zjvfivze.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vqqupodn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3uaqrzetq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqhuctxu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wrytglxf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3magrozdb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qmmyydzn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ccruupob.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3iqhprhzh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ywddwnip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxyfvvtj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3efcuieam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfryuzsw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aownbkzg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cdsaepln.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xbhhxmmz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wfdvwlmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kaahbjct.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tzzrqnnr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vrmqkdsb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ymcdallq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3epzcyqjb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mzxuejqk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gmxihkoh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wtqljolv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfedikfo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkegkdos.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wtgznsyg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ujvacryb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zqxgbqns.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kvzfvewl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uipjpkla.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wmomonhh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gjxchars.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3namiqajq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqaeotud.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkgxdsur.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3megatucc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxbhmczc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3khbpjpfe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3buastkoc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkgukeyg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3guyhmiwf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nglxvzzw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gokpaxdo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lipbqmks.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxlsseem.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sffjfuwd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lxquital.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mpicqbfj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pxtavgvc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bfdtfomr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ynmsguub.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yjobrvzd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bqprgtyq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3joxsqlvp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jrxykzik.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vkysohur.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qpagippn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bbsfyiqp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ujyeyuuy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eefwzrnv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3surarjqf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qlxbyhrh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lwshotxr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3roqwycff.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pkokavvu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vrdypcat.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rlyzjohc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zngewvig.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3leqkpiqt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zsukqfmm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zhlrfcwj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qmomdtee.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3avvoluba.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3uqfdtasn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3clkqnujt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zolqlwmu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3veuzxbbh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dozkruht.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kayvhxvv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rwbvbsdh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zybnhbbu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctfqykxv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yqizlihq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hvlvdqvh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iknmwgyw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sntqhkuo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hazvjgmc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vzxpnbfs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ksuyqygb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dwooxecz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwhatmbs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nmarzoka.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mfdokbka.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tptljrfi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xpjrujlp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ntacpilu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3onbpnsje.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ipgcewjv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3stlulfnf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sdcugrbb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jbqtrleh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bveldjat.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zjtndejo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mqguqbsk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3msnfsdak.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uilqcdfk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zuepcmgw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mltrscip.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mpxpqxhb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3kozasjlh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3edumlzum.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fjknpiwa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ozwrvroa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gcbetwoa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gdviqpja.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qtzmwnms.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dnixlnrs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xmjcatqy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hcnzwfuh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ffekyrpl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3didwcmmw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iptvzxot.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ifnkfazl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eocthepu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lzpqamik.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tlghuauy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lqjbbkhc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tdjdufdt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdyjoz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rvkssovz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kooxqclq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zyurvxsx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhajjcnq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdabvkdv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vftztblc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rkrngkkp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3celuoenw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ddkybiub.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cfcemvez.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uttfeant.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3laiallxy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etimfsmk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qnapturn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ufkhqcpz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pdgohsgi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ootbslqz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vyqwuvhw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3uutbujha.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qbcutjvw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bgxisaei.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vobukzlh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwjoxzda.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ffwsxwhv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lnpbwjlt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvgblqyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duptypjf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rzdrsdrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjzidvym.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kpkjmdqu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ueadtvgm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3urlmrsgy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ggweooay.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kprslaoz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3owcoysfa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xluliwna.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3mntpbjba.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fsfucgew.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zjazqkqm.html


<!-- 参考信息 -->