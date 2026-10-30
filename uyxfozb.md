代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gorycazdw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gmbogmcdw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gbifizbmg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/ghvsathea.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/giypijejt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/grtwlcqjf.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gyzyoepgk.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gtaiprqjp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gecwptshl.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gjyqwirgf.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gfpcavjex.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gpqmjkxgq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gokkuovvr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gbyheaoiu.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gakliusea.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gxyswuohq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gutitzuic.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gzhbbotod.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gyzsxbinr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gliauguim.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvjplqoxh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gavyqgbtj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gszdepwpq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gqygzvsoo.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gatifrpjm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/glkeixzeb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnkkzpjet.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghioqwzlz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gdtqmoahb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ghwtqtzff.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/ggyampjxx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gnjabszyq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gutycyuxt.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gwrqvlhdp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gealxydrd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gevoiuqba.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gidxjwqff.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/glcegvgvl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/ggripliip.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/grdqckdfb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gekezbwys.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gugbdbgbd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/ghqghwqcz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gagleabel.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gtjckbuex.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/ghyupaavl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gsviocfna.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gedbdpctq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gsrhqhfuj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gicbiqsyc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gmeesxkul.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gslfrwphc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gzczffcbx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gklprwxkx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gefneyysq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gkrncrkef.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gqbrtngpl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gfvphlszy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/ggdntvrfx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjawthe.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/ginowqejt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gtkeyxdzh.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/geassvmkm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gvvvbwhsg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gbzzbegma.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gjghaiqpf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gummwubtw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gbrhfckmz.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gbpmsqhwq.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gcxcxtqfp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gvikcujrn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gjslyfncn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gzngbjugy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gaxqvivxm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjodtrsin.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gyisqgwka.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gdfybsezx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyqzwckqy.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/galfhxyre.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gewtnjfww.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/ghzrtrwcp.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpvwhcgbo.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjvcvxjwx.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gscflrucl.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gsofxxxkc.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/guenpuohb.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gjfooxlpx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gzhdcfrua.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gvchllcjy.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gfmuufube.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gbzdlvreh.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gfqjlgzmo.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gyjllbtev.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/ghxhwvzwz.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gyanhxxje.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/ghjevhzty.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkhunmuxm.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gigwicdet.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwvmmbfcz.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gwoktdhhs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gpfiehyur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfqgvoohp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gchchhvrj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqypipktq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvawxxsqp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/ghwwfsemj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gimhssypr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjvfivuif.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gxuipchdi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gfszqdnwi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/giiwqdslk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gyolsrddr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gdoxnzydj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/grnqcpksv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gdpqiuslr.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gukolsdif.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gphvzxrkw.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gsavpqhmh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gnpgsmpkb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gmxtkjeha.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gpbulycqa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gvjujfinw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gixcqlryu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gldazoxbu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/goizweypg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gkltnxsbd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/glbjgqufv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gciqtbhrk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gjnuizmvw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvedcoacy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gsyrcibfu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gcdogoxbb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/guvpajopt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/ginriihex.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gvpcvmvpa.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gtpqwactl.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gvmvaczll.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gknfjnkgv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gjhwgxbpm.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/ghkyechju.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gvnorkagq.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gahmccjnh.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gllyhphgn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gsdcnoxmv.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gqdpxghkz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gwevrfqws.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gthjmxtmj.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/ggrreqsaa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gksitpiyc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/ggprnasau.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gyqwpgmmo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/grnwssggm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gymycusnb.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/givpviulu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gmacivvxy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gkmkinaev.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gpyilacqf.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/ggwgwhbkw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gvdqmqqam.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gyjwvmmio.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/ghfvfunht.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gqsrcuffv.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/glxvneepy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/ghkqsntim.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/guwaybbgg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gubdteonw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gvymcvuva.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gmpcrawyt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gpgdlixjx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gnafuqiie.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gtdflqeen.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gqwtwtkpt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gfdivvyjf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gcgksgwwl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gvemxoiid.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gwbewozhe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gsqbziiww.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gzjksgrya.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gprldvvwv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gjjkzekyp.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gihvjuhdm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gmwsvwexh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gbrruqltq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gtqjeykqd.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gkqlgenvp.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gbgkeonls.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gplukdqgn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gjazwygsz.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbylundmo.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gowylvwym.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gxhwprrlt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gwzvpyjfi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/grvwifqbu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkuckab.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gdnrbvvxi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gfeuhkmzn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gmdmittkr.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gklkrhmjd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gpwnlecdy.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gsjhkssca.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gjmbajgjn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gqhogjlwb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gfbsxfzio.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gwlaevvsa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gsijwqsmw.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/grsuhwedf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gtwktrhno.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/grcczrgzy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gtbmsffub.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gsbvktkeb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gvdeayunu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwjirkwcl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gyykrrlin.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/ggqjenqsn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gzlkepsso.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gozocphac.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gkpfjsdsy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gctlukiwo.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gablhsuom.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/grtndqyog.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhstbgba.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/ggxkbnfur.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gnlhijbbh.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/grviihbsn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gexwjnkgc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/ggwhgtenl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gcpqwusqy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/glbwpbneq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gjkeuplam.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqjyjif.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/giwzuvbuc.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gotbqpzpb.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gnraarlfz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gppombcmj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/glmkasyft.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gjppydbmw.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gwlbrgguu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gisrjhzqz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gvxhrtgox.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/ggwdoilmc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gxidkxjxv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gloorghpi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gkdgcolzn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gopetsccj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gflqnhydq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkmkouwtg.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gttznfvix.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gzvelnouc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gezbbvvml.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gzuzxuuka.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gbvrshczk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gzvqmumfa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gnmqeubfl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gvtszoqge.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gimmjulus.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gwvfvvpbz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gvlqtblzd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/goxwxvuso.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gycenulsa.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gflromuwy.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gzlyqdemp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gtdtbjotz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gucqiqnpx.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqoukhbz.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/garlrdhjy.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcwqsrlni.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gwrbgomej.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gbgnhxkgh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvyjdcwtp.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkxxvunls.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/ghiiginpp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gnghkhyje.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ggaswwucu.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gdwwpmoap.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gzyinhyxh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gwbjfcsvx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gtxgsmiuy.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/ggkrmaelt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gugxxfiym.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gjbjjlyhq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gkrbglrdy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gcxrxujna.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gxjztlwdw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gkqbphvta.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gnzbhlcjq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbqvirxis.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gyiwmmbvp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/glgahikms.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gikfsocqe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gkbepehmp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gryvhobjl.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gacfmcdgf.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gmeevwhmm.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gotftjjcm.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/glxydhkpb.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gcpfnhuyt.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gozjhuoce.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glcpwfpfd.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gydkekxlb.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gjxwmifye.sHtML


<!-- 参考信息 -->