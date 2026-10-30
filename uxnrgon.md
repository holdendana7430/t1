代发 wailian999

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gumjfaril.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/ghfizrouf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gmamitzeo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gaaizmqfk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/guelibamf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gsyckuphn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gqvfpcdfg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gkoqzseog.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/geijyotpu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gfkntkknh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gpgyrovma.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/ggudbuluo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gdpranfxd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gjlqvhldk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/glqveldey.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gsfyfiuso.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gdleuqpkw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gmqmhoozz.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gsmgvwwgq.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gjhhimebx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/ggikeevlh.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ghxflfrpl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/glfqlrgqs.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gknxcsqiw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gwrvnbbtc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gganpbanf.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gupbzhjkb.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gnxfaytws.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gzvwuhphs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gryrusvdd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gewromvjb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ghkcjdyrk.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gvasmedmh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gcwmtublm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gajgtyldn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gffflreot.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gmqeksgem.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gduhxotmr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gqwfnasnl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gyczjzykv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ggxzqepyd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gafmonnnh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/ggljtrcal.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsnqjsbl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gdqgmbwet.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gosryrnzl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gumjgikbm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gcjydoqmg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gcbgyiqjw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gkhmfokdh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/grvxrqcgp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gotcowdxz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/grkkxmkxy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/glksqtzbc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gqcbhtgtj.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gmunqidyk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gmbfpeoge.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gziyztkng.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gvvblvqey.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gidzbxowf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/ghoogdwtv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gwpawyros.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/grnxfkwkh.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gaxqlodzz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gsdxncqvp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gufcrggbf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/ghhqedjxc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/glbskkwht.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gooyihiah.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gusbmxouh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/glhxusank.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gwxglpntm.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/ggragrnft.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gehdkiqnb.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gqvrmtiek.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gcgadixom.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gcshxszjx.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gmysgedxv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gijmlqxyl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gpgyalczd.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gplhegfdy.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/glusmiirc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gvzopjmfo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjglokqk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/giikccwuf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/geimhzjjc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gvhqoccao.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/ggmgdtuok.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gmwfzjqke.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gjlwurswo.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gtqkebity.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gtdwuuvpy.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/giiizuicd.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxzlvihmu.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gaeoqxmsm.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzvlemyty.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gomqlqamp.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gxzvxxvqp.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggqsaofke.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gwcnfcixz.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/glhgzasnp.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/goitegkov.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gkujtqzqk.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/giklvdwou.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gqtahjvlw.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/giarbfasc.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gbaevavju.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gwenrcfwd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gueugkvcg.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/glbexgzmj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwlszefnw.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gyknqxinv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gwonbdqrs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggktxytcj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grfeeouix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gthpqqatk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxfnibycl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gsoprbcas.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gcdihtwli.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfczkcwjs.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gzghmomyc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gjhdqmpuc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gbmersgqw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzakwiznt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzxmxoes.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gjokpfenz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjhabhjiu.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/grenepakh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gqyqqzezb.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/glvaqojxz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gthzrurqm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gipjtxsch.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gcyfpwksa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gvqnyaoea.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gvyrqsayu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/grmlcovym.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gidrekjjo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gfxtvtqle.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/glfpvnkjc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/ggewlnjzo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gmfexudid.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdanhuskz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gfvqhgsnf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gzfdkqavp.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/grrnrvejn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gqwykejos.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzgfovvvy.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gmyiiujud.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gdzfjfyby.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gpwdlgupl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gudzljvsa.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gaeoosdbs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/ggyhamfgy.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gromempot.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gnqgunxzh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gojooubdt.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gvivvpzbw.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/ghipwzkba.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/goydczrik.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gypjkbmes.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gryxuzibm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpmtotkxs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gsaksufib.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gblmyewpm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gbjzunago.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gfpxhdglr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gegzzurqy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdjduhvvr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/ginsetkuf.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gennlxifo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gmxpislvp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/guzfmwbaw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gezzdfmkz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/ggctxdmcn.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gfqoffrxm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gujgtwhwl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gdtgirzjh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/ggwfgvkjp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gdzpcqmkm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gyiqghjdo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gicxudhrc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gyooxjheo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gydaciopw.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gajvebvfm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gtbojzkoy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gjxxwwbhj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/ghcdiczzd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gufwxaqrn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gxjmwbepb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gielghmbg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/giuiebxne.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gxedizlwg.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gtidjjqzu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gmbeojvum.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gnqwwizpy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/guuvkliyk.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/grnbahlfq.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gwqquwzws.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gztiukgez.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gdewawrgm.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gufxnyzhd.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/giogiawuh.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gayqmzddi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gvpfhjwka.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbdmflawp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/guzqxhzbe.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gqwxczlwy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gstmzzaad.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gjyescjll.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gchqkmvln.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gatuxyvcw.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gnwpstbql.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gseufhmxn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gpcenaoyw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gtagymvkq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gvltzxeon.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/grxwdfnyz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gblmrdryw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gljwchswf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/goqxvcugd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/goscsitnp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gbpueeily.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/grreqarrg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gykxcgmsl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gqzdcktsa.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gxvcqxjvw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gmwzgkpsx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gyzfluyrs.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gqcxohlpn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gtumyohrr.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gruioxseq.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/geutgfhuo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/glnqlrwun.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gyqhmcidx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/geffjkkoz.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gyqwsdqpn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/giwsdgteu.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gdtevscrc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gjgyutdpe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gtvzhfkqk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gslzozgvw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gpdqzisep.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gpbfkngmp.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gknhekigh.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gizmogkyl.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gbqrgdjmu.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gmwacoink.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gepsihkbl.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/glyhxyepu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/guiimazvb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gahpjmoif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gggzihsdl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gucxtxfbt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gtrweshhm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/ggtpzoinc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gipewmmcn.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gtezwesws.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjanofxae.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gddedazch.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gkhfkngeo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gorbazafb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gcnunblck.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gcuddkccg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gykdfvare.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gkdyuuhtd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gjsbczhzh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gyexdfeaw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gouedgofz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/grctprkwh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gbsesjqza.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/garbcweds.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gobkvhndm.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gdvnpatgt.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gffmmvqdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/ghcnmzjmf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gyizcgjvw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gygsrbxxh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gpplpoehy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gwadcknac.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gwosssvno.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gpdcsvdxh.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gkgfmxbxb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/glkipjykr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gturryome.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gbqejlgel.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gkilubell.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gokqjdlfj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gssdiwlyx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gzhlosqna.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/granogfik.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/guiovttvg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/ggxcrpobv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/ggejwrqlq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmgfpndfc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gjembyddw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gnkopjsex.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/geiictwau.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gavbuwcyd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gxlqspbrh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrtmnym.sHtML


<!-- 参考信息 -->