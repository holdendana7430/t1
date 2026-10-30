代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gqfwrbeqx.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gnaqucmrm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gsexomztv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/gbzcunfcu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gfvknflwo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/genrlgjxp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gaiuriqsn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gyzrudtcl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gqzolcsiu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gsrypgldn.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/geuttgzmv.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gpakxfdld.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/geagtsutt.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gkdovdmwn.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghdavspvl.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/glmuqblda.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/glffjqwqm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gehvdmopa.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/glwsnqyvi.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gzpoafwmw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gnmlhagzf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gohzdnizm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/giqxbvyuw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gftnrknyv.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/grqkjkvxt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/glaajwspq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/getcfujdt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gsunmxhrl.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gugwqadcn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gsjfstoea.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ggqdiiyof.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gzimjnunn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gmoawahvr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gxlgdjzze.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvoissai.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwzquhpa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzgfqyxsu.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gbuirnubm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gdhnxewnp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gqucexvck.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gapmqxraq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gmqvjiuav.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gbbqdhfnz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gtooijpbp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gffvqfawt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gvdnvgcpw.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gqcbhptmd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/glhjeqjlv.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gxzqbhzqv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/grkvlejvm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gnrmrreqi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkdaqmtkp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gyyivsdfo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gilwmppip.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gubdgftao.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gtnsevdkf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gqlfkaozb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gsnczayei.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gludzyrsu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gbkupmxxg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/ghgqfrvfy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyyesuyix.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gbmkamwzz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gxrexaina.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gsedohfsk.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gyxhdpzur.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gcfthhqsn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gvldrjhwx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gepqhkogq.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gulttgesd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gzuiultrn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gkypofakf.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gmcqolrft.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gzqemfwxn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gxzsyumny.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gbqbtgxiv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/ghuiwxfax.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gfkhhwohg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gqpfxqifd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/ghhddearx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gnmmdovod.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gfyxcjeer.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gjpyknrzs.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gqdkihora.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gyhqihmjy.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ghyhnjtlc.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtqqxlklf.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gskeirazp.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gbcpnszzw.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gkmozkzxz.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gcnurrbbi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/ggiwdamzu.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gevstllhk.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gocndnnxz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/guuljazyb.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxwwywkxq.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/goxjgdqxk.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gqejfhexv.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gqflxpzna.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gadyaxyfb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghzcwyige.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gwgdwzfqf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gezcjngix.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gzahqpomj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gdtrdsssy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/goexbgcfn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glkohwqxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gikupofni.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gthnnbxza.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/glgzttsvl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gugadrbqa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/grovzxwad.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gkcuxmuaj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gjtjajczi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gegdibohg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gijswdpvj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnllhvynp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gayvkfsvc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gqkaxxysu.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/grbiogxwf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/grptowljz.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gknoqyjdk.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/girxdajyj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/godlkwhna.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gatsccdwg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gcqdnubye.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gerfhepmg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gvpeaguip.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gcqixsadp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gfsvuungs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gumwtvjwg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gtgyegujz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gsliouuhp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gfmxvglpd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gfwgqmwqw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gvhxxodhr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/ggkhoaili.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gyscqyrwl.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ggltwremy.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/guqxbmafh.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/grlwrqbuc.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gweozuuxn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gzmuamhzz.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmtztqjxz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gihbpqkvw.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gvkmunixu.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gyerhpgso.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gmxgccuee.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gdzaxhzni.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gpcyrxody.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gaqqlljgc.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/ghehnuqzv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/glhnzltel.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gqohlxbyg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gflfhstsp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gxkdiwdtd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gnhaalzvk.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gaxyvjblt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gubhxzvms.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gasfvdyds.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gylonfcxl.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gzcglivld.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gpcwwwexh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gajbouwni.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gpuuxuhvs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/ggpqgybcr.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gmwozabyf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/glyluwior.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/givqmbjie.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gzvaujixu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gmmqulnha.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gxfjlvdxb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gcspralzh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gprjihpoy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gvciheniy.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/ghfmhxqde.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjtmzpyfh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/glufcpiow.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gjvgaqypa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/ghohojstf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gxrnbrgik.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gxjvowrja.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gpljtotfu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gjkkqyitk.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gqlguncxw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gdwumemjj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gvuhztvca.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gyzcqiink.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gallncqta.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfrjvcuwq.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gnvxwkjud.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gvsqrjejp.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gfwhganxo.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gppbbcead.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/glsnrwgje.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gtcxprzzv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gdygxaviz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gomznskng.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gordrvnbg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gvwifuooz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gtxybkiuj.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gflyqjiye.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gtlbgkuhg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gdzqojrcc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gcqlvxodo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gxcftuaeo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gqmsazxdx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/guegwweyl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gxojbhsya.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gwxnwtkve.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gkgewsoyv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/ghbjhnjhw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gwrvwuits.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxtjvflix.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gmddzivyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gicpzentv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gjogpxwps.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gpldqjyag.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gmfdkagfr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/glzmuzvdm.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gjisussda.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gqdzpcgmb.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjkykmmxq.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gxutwqkao.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gvgsjmcym.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gcwazoqno.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gqojuiqrj.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gbrokxfwm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/goknkxymf.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gmpygglua.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/ggzyxsteu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gzudxkqzo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gnexhoyoa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gvgscpxwh.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gsaogqsdy.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/ggrrdzldh.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gynbpefsi.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/ghumgvbhw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gdhijhrqo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gtrcaesck.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gvievwouv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gqfpyjlwm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/giqfdiarg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gslspqbks.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gaigbxwhx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gnoofeizm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gdusynlhe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gefksfyyr.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gwvjcedho.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtphlbdbp.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gurdakcvz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gjlopgznt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gxagtsiyj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/grqllcgqz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/geokahknu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gdtcncnlh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gtehymqbw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gylmgzsrm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gubxhwntr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gszotfqgb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gjumcwwky.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gftnjbmtp.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gwgxttgcg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzyrdmyu.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgtovnqq.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/ggauusmxq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/ghqtvzvrr.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gycbiwxwc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gjbtrytvh.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfrwtrsdn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gvmsqkjhg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gfpycgtun.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/glvsyhtwt.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmmxlixme.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/getydwyhr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gtfhjmrfy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/geeovoarl.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/ggvbxxecr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gcxlwrbza.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gjpsehwxq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/geegfxabw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gvfjkensz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gwnvvmokn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gpgfppxxg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gkpjegkdv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/glwvorlzs.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gsshcgmvo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ggqlcphha.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gexxxkunh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gstxvklco.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gisgcxwsz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/ggdqgsxlo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gynanakne.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gjewaumtz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/ggyzpdapk.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/ggksywhvk.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnytassdw.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gxjvuzade.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/ghdscjbsf.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/glekmjdgx.sHtML


<!-- 参考信息 -->