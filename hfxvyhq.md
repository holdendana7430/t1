代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gjxnqagrn.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gkfzieawo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gliunwldb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/ghkrytnsh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gagqbnmmv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gmxgbirzl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gnaagrwxa.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/goxzqmadb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gzwnzijpo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gkbfgsquu.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gcgfnwhce.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/giapmssmj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gunzupoec.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gyonqzjqy.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gpleafgwx.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gxtncjpev.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gtmmhxmua.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gyeulbnec.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/grmcufnxc.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gqafhzmgx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gdtjopxbd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gryrmobut.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gkanwodsg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gvxnukzgw.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gsdhjvvqb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gkjwvebeh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gixivkcmd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbiaqvrn.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gynldgiuw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/ggprrbemq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gimodqubh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcmdadix.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gcscgchhc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gllfsqfok.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/grfhgyuqp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/grzeyopfk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gzatdztrz.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gtkimjfsf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gdvlsplxu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gjtroyeub.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gvwxrgjmm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gexfkughp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gklyrqtpg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/ghtlzezyw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/ghefjzvgr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/glykpzdbq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gwxfejkyp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gwadxebff.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gnzaojnuy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gbcieggvl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gistmetle.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gnujvaqha.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gpknxzndc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gzirivvja.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gqxlzrmno.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gvqrptold.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gywfxebok.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gwfpcjnjo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gjbliefuy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/giksqapks.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gdtgonojj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/godknhdow.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gifaejspf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gsvhsuvap.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gbhhecozq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gcmlnfjco.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gppdkhndk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gufiikcwj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gyzsakxci.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gxytcejls.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/grxubyjud.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqplwuwg.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gogjcayet.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gktfedeoy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gmhwnurzx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/giwnqqhka.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gkesodvpq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gokhwqrqy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/ggumdjusw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gugvvvsgn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gmfrxpyiq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gffgyrime.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gcjhkewyl.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/geipmcvcr.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gmzxpefik.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdjzxxfrr.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gphptbivh.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzeuccflm.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gmrsotnju.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gckraihtf.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnhfppejl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gyvwkuzcd.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/ggtqudtqg.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gwbuvzezb.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/grmtzzilo.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/goicepcml.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gnxgtbfav.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gsczizqtu.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gmhbxddra.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/ghbtxohvm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjcbpydut.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gqmjtktam.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcuitremo.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gcsratuto.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gsijtwozp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gfliztbvr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gclzdlgzm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grjgjkqwm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvdxnexmg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gmdvgtphr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gfgrmkavs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxnqlbzod.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gzyagcscz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/glrhluoog.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/ghyimxztz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjbplpukz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gigpdhafr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/guuxubjum.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/ghdslbcwe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gtltawoba.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gjiayoerx.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gttlpeycn.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gtlctwadl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/geghmyumj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gdurbibdp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gtisackeh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gennrpzaq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gfrinbguu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/ghjbhedur.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gqpltuigq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gpdvofssl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gfhictdni.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gxuatgwxf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/ghunsgtru.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gcqaugwsb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gnayhxjor.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpfgngfro.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gthcurxzg.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gvkayfbyh.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gonfemyuo.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gfmwjpqkw.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gvbgpbuta.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/glbrzluej.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gsuhvrphi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gpgrqxrnl.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gevvzswfa.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/ghfwmmunr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gyithqpsi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gowdixkct.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gtnsriygg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gjpechzrs.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdxwovqrl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/glxwrujnt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/ggdapvhrk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gddimzudq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gudkfncsc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gafvebgbm.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/ghozfcudt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gxrkthjxe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gcpxwlfjk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/godirkmpp.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gzhbvigey.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/glwvfnnxy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gmzypunvf.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/galnwzrlf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gvbecqwuu.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/grqghqkim.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gslromiyu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gandhmqzv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gylsrwctb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gtfkomygd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gphcyttna.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gejkwwcnf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gjyctupzh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gylfxtxeu.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gaqsiavxm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gcdoulxpn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gjuqbrvew.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gwlpnsmkw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gpkclzhmu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/glfiutijo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/germlvosd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gmbksmpxb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gphpblcwq.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gyrsjbezf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gccxzfzgk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gydjyqgkj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gfthgqiyd.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/givqvwdfv.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gggfuhoaw.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gghybmqbb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gcqyjhxrv.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggswjdelk.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gtkwxpyks.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gjughrwof.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gnyfcwdwg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gbeszhmhj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gsjwehhhg.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gxesqtkcn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/giqlyutip.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gzsdohcax.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gticblqaw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gmsxxdmzw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gpwidyncl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gbvofgiaz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gryvpqxob.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gaxptmclt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gzdrogjof.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/glyqhdwkr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gtiqexqyv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gtchbwkwo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gcfexvrmr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gjdanrjai.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gecgsacro.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gcnhravjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gukrfiime.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ghfzitgpm.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gspmwpmyc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gqtakqdsi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gkekbuhqm.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gampwqvya.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gtvheffjd.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gxsveesag.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/goflxftig.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gfwkdoedd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gesxxelaw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gfvamhsfk.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gaetdjfym.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gkazlktjk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/ghqcbtpdn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/grebgfobp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gnzfuftse.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gvgjjblvd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gnhqxrrix.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gsdxgfsom.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gxyjeyvta.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gyiivapda.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gcdkbxhje.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gungfhikn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gjxbnkdaj.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gdtneiucu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gtivlzuhl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gtxnnkshx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/guauomhfd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/grfiydazj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gcbksxggb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gilnvztpe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gghfpdzgd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gfxbpabet.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghxucvmue.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gnwxcwciy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/ggeulvmjt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/grjdfcrxr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gbapyrskr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gipykzmmc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gavmxwzga.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/geiqyxblw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gnnbfbszw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gxwgpisjf.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gvqittofr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gwgzcfpnd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gkqdzcduw.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gnelrxbap.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gqfgpxngm.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gzvkhnntr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gwrgkdrip.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gcsoptmlh.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gudmksdjo.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gmkbyqvqw.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gquliwmis.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/geirjsyza.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gmjhdxatr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtfegbyjs.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gltgokayn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gkfohgaav.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gthqwmaie.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gwaxujdot.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gevewunpu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gjwtihvtb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gbehcsofr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gowlnmidb.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gkvhzxmrl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gvyyzvmwp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/ggoxnuvod.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gaqdmtums.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gikmlunzf.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/getkjunye.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gjusxelzg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gmcjqzwbx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gkophdiqe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/guarfnfuo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gshtmazxt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gitqcfgsy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/grsbmdrlv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gyixpryna.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gxnenkxww.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gcvbgqvas.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdohqdoif.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gfjcklkwe.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/ghynkizae.sHtML


<!-- 参考信息 -->