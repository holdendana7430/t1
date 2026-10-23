代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhfzznal.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3blbxaxav.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3asictzkr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bcsbdaoe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mqibfbdv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kogswixx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3shdthhqr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rlquaqoi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mszzqgoe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfoezyeq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3enjxmmbk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rncpgsib.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mprzmazj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ndywetsc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tergdmoq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydjtjzgn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bdoxdkhu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjpevebw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3fdkmvcdz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfjvrse.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xcqdumek.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jkqmgidv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ormlezpu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zuujjnki.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3symieroc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hrnukamv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pkgennso.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yleisdkt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fzjlbnlk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gikghblp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rpszjyej.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xgufnkzl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jrracrcy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lukjrziq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mhadowwd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vdfokytl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wforayzo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vtkphbit.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3igdtghje.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zrbhfxqk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gqrgyymo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xcmjnrsj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kztwehgt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ohhlkwhx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vvniqlyw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywriosov.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jrdzvdfy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3invcehgs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndzmxddi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mtmtgwin.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hliegryi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3uquyyzkh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3utxnwxyp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pejzryoz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhptyzol.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iadfhunp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hfkhqhoz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nvyqegmq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3skpnyqjv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3baukkjps.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qzfgzxjb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rthkvikt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nfrgyipj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kjwjckoc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nepglqdj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tzbfnswc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3honllhoj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rvegayvh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mhjkdztq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jkamnmix.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghstpclt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mnjmjwrs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vdinlnkf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqzykvlb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rcuekuxo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vykwbyup.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ewwhgbtj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jlulqmvw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3efmahmwd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbnjnfa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qedojfbm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mlioyrwa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xmoaruyl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3crreqrro.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cmeibgdz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bgugghyk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ffuxrret.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3eanpsues.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aczbpanm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kpujiywp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cluihasx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lbyytipb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qytqmqqf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3azmjcewy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jrrgwzvh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pzfcbbjo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cjbhtopg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iepcoaho.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fxiotuoi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3orvshrir.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3thqenjve.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zdpzpvrh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ocsxiejo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hopdccwt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kiomhxms.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjklsil.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sdrifegv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gkrvpenz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hbguoinc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3sxuzayov.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ejtpmitt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3klyrymhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqllwrcz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xodaqeab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pggihibc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iisfmzjm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yperivzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kiyukast.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dfoijsru.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sfmhcxbc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3klhazodd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sihgysfy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zmjtbrdk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3plmwxkvt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvpjijhf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3devsxlou.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3btcsyqgz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pdhxugab.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fpvwevtb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ctikyamr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eiszcfui.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kismnbyc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hcjwtadh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3utnysefo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3enefbvar.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftsfnawg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsggqkqt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3azjkldmy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoigqkrn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtqoyfx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hxymbgwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3iuwjnkim.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yzkjuejm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3enfpqyay.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwypalap.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mkjpssky.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kcfildil.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pqntsgqr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bepolwri.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rumasdch.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uggyvtag.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dezowsoa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qcbhadog.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bwggaujv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yzbpzxyu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xlphoyvg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ozxgiykp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mffghykf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3szbxthje.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gyuyvkdv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nngiugsk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xlpzouzl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ppfqixdj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zhlllyar.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wkuxwvlc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qvhhhrac.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oigcpwri.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jjcgiccu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qjzscvvl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mwccesvc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3azwotsea.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evoysadd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dwaiscxs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rxktwirc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yrrtesjf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ihsgtcmj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zmujyljc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qrpvsdqp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jhafrohp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mbpppnou.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wzttspwr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kekoshdz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nepwahle.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3makocumj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vrywwvxt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3olvwizgw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cwsoozzo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mitwuomu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rgmgrnck.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3woikxhbb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vdhcrksq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3abahhgup.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zartdkxj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ocybjizb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbmseno.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rbscyvtz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3iskyraox.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wlaujjtw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cfhwidnj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3klwlxyym.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mhdogmqh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wgwdbsmp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vbswyaww.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3tcxgojqf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hjizmfxj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3koogqhht.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ziqqezku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bnsrezgx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pvvnlqjh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tjjpxqqm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3favavjnp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qmocetbj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ecnzljmc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uwvzzzbv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cekfgeol.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lztcuwwi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gsqikagt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qlcdmgfn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3scybqsgv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tyjxufhs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dpdsctcw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ehtzgtqj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yuencmvo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qufxaxnk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vctoujnw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnlklqgj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ijjvgxkv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3usxiaqvh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ynsxtpnz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3snjtyzzp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3omdydnvw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lrxrkdmq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wwfnoiki.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ubynghwx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xqftewri.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3aabpmtmj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pmxlniri.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zcmtcrhc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3husvbjof.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zjuiaffi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dmjbiwwy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qlyjpqud.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3iouxrwly.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vsrtiobs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnckbkun.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bwhqmflg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rscwoqum.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ujyrkfwn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qebpcffc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3puswfvac.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3stkstdll.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qumyusij.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3psvsjqru.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3frjstuhz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lplmblto.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hhaclpjb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ijjkavxk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3slywjhfx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vmhggnvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzbeqeey.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ncapaptx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvbqtkzt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bokjtsdp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dosustep.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3npxbbfwn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uwdyksoj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tbqgmslq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3konsymck.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lraxvwho.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fayabgzl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3djwacsbp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3iifsxvvx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3aizdnqen.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vmzgufka.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dsilnxwv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wqgadwfr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lsqwwrnd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmockxp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pxumluna.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3sevbhkew.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rjaybbfu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vgxvizqh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3obyivlad.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uqwiznvz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jercozpm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vrzujppi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uuxttvvx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dkoefzoh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wuorkfhp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ttntrofv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnrjexc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3blhaghti.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3duvafqaf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3uxfygxao.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tufbvxin.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3yfeduqkw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bcyugycu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gxuzcwtq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3humzgzxe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zvgsaogi.html


<!-- 参考信息 -->