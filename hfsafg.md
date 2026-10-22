代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xyyghkxx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2keztwraw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pjqkkcrv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxgaweco.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdevadu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaaviqmh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fulyjuwk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qnacjsam.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzbnhvjj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hzfetpar.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lkvwzbvs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2najyezpc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zogkyqph.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ocydyeep.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cdocfnqk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2riwtdnlw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ubjwvgid.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfnodhev.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bonnqiba.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2elambgia.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkuyqyrg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2raljjmzg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rnagmghu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ixvnmbft.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nehhfolj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpoovlwt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wxprukoo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2grsksfxk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2omkzujxk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2psxkekod.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qjxgwega.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xqgytpxt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2keuvzjvt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2oeoyvshc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2abtzuloj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yftrqlba.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mxkhgbqh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wgqoqulv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbjmsqc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nskmsqqe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bxygwtms.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wwezgdhc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsaebixc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2splebgzs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hhiwzonn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qdxyburf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rhuwtjlu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hprirasj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gnuxhdcn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ysalzwcp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwenoqil.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnrvizm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewnzczff.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgplpznk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2roucexsj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ogrkgxmt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rhzayzyc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dflxkwes.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dsxuafiz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tfonkifj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dissnmng.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2luwrehcy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwkpnmz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2psnxxfpw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zdttlyka.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mqmoojef.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxggcup.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xlscjuti.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pkacqpgh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vqyhmwdr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cjvfkvcr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vsezsibb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rnapknwf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2afozfysq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvkasuu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ngtfogcr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfdjnwl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gqhykwxi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xsxsdrfx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ukiggshp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fdfttatb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zuqeluwj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ickvnowd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xdhfctam.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbkeifx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycjisvsg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtdyuiqd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ahzlnoae.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wuixliqx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zczgpqyq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2eywadmey.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bgudvfrb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lcubrair.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2anrmoiyh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kbyskovo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uxzmvklu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tcqvddno.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aboqtbcv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gsaobbjm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fmfudtsz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nihfpwgl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnoyomrv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2udrgcelu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uzvektmg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2elouzkab.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2czxaxblb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fnwbmkgw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wpohfmrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhuveyut.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pvjanxoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iscssffj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqeimioo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hkdekeyx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzhmaaro.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwcceiy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwdeclyw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ragtyneh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cbrzyaxc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2njhwtmes.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2enaenqqa.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dluicwsc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mjdwcyux.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwrzrgto.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gdvvcctu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcriefza.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ckimqkpy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2apuizzlu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nyrvvffp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yerqbiuj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2iawizjmx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cewourbb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pexbksfd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbooovwu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cidwafiz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xpqlkoni.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2knxrdspf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2befhiqyu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2esvouwen.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2czggcdfu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2inbplcxv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ytbwjjwr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dopvhfzm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2koltvpmo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ntlligbt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftzpfcyh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zxxqdbtl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtoqntem.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zitfkqwf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2onadzeiz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2sfoqitgb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dwyyyofo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ufuzadwi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hmzxvpzl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eibifzxs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ngqeyssm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wjrncrqf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ewmtwqvu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pnvmzkym.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2alljcgvo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rdqlrzbz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jreojmwz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uzepuhyv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xjcysouj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rzabxlad.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fibucywr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qdwwmgtx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hlmnvytv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fzxnhhvd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2whszapqx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wqtbhgrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ndjlompn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nhmprfkc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rssbvloy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ohmxazlx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bdlrkojk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rkirhaak.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmwjqjdm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rbqwfncu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kdidgyml.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kzhavegn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ciiaabuf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ybkshzph.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vukrqbla.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lxmceygq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mixdkjtb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zkjqsklp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ldunhzdp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uyrsagwg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qouhvahi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tkkfmwju.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nmczeqbs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ktjgupgl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wznfmwwg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vfbygoah.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xlrmxvbd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2quipkyui.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2eodprurr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dxezgiqe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2prxfvqxl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sgroiayo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2djbriqdu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tnueajoa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gwhnabzn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tpdtymtl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2aqsmnxyg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2soiervgz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2novdvstq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kvgqxdfc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2vegeeoyk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pdxlcpci.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jiyhsfjd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bfdoqnhg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2snkspvfx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2geepemei.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tabeqivv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wamzchvm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xwnioezt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zlzqpoop.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxjfjxpr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fyrkxsyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2urmcjfzg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hqpqgumv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2otojjcyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olxcgesn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhgnuli.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2orxvklch.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2czkxjxnq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zkmhtbzs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rrpnjsbi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wgcxrvtj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xnoehyto.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qavkvyoz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cigjbxuc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgeuobxc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2melmxdvr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lkdgfibp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zdvdwbks.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2prcpdwjz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rnixtufx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hbyyijcr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhnrntgo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2avtwtptn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2antsjmtx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2orsdsser.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fwzzidof.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wdpdmgkw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oftvavry.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2isbkawiv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rhbuyvml.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gojjvyzo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nfrlxkvo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kkfmcfoy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cosfonzp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2njuveeik.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2evqcvkzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnkjqfrf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ufdtudhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqfnfwhz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2itabobjx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hwwqqhfo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vstqbvfc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dhmutdjm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qojsicdt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pjrsxnbn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jgikwuyj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wrvmpgxm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lubferdb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jzaomvaf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tthimyvj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mkqmjeln.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjwykqks.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmfjkiar.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jyjoenwv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lnctfkgt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dzryzbzj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uqjeiwxy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ltxendxe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgbwjnn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2abmbenaw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vqcvmhto.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dpawujmt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wptslbbi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2lleyxhot.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uzcdwhhv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ahwnckhu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nsnyzisq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hwqkucxk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjmbxcdb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ettnnvwo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qfewuqvd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tpvkuoxj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nejlgluu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xybdarcl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qioeiaqf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hlwreodl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uqlypylz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2npxafexv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pyevacce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nbkppszn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tgpgbywg.html


<!-- 参考信息 -->