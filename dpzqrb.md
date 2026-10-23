代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3khgxnkob.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ndkevzhl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xhpmsyel.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3efyygtdj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmjlgljt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tisuspwk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jfipetlh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xqxntfop.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uykkeklb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qrvlivke.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3cgxgmhal.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kzwddicx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3euvewjwo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nlbjbacv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxcfjhxk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3numbvkxe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zsxoddwk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sdwysale.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3agpkyrqk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cqkbjkcg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lnldwikc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nsrrcvxw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhlzkga.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kiirfpzb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qzmyvzzv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3soaoxdrs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwjwqpiu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tvegsxfz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pdcozvjc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dkxrbbjt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hduluofr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3chkmhuki.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jwqaheax.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zgmbnwou.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ojlqiige.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eawmqyyk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3cdcsfxqo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3udwyzqlj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzrdlfih.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mjtwnabj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlnzmnxn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qqntdero.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xdirohjz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qcztknut.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3flewgepz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rmzbwrak.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nxotcvnp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ioadjdmm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3poovrxwq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vcqshwdm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3jetdjrfr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3catxuzih.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mhzynlnv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztcuqpzd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qrkhttzg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3cuilcavf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ojovaazh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uxjwhjmx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wpmgcbdr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwrvogkk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hxaqaiix.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dapqnfuu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3oozuagvn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fycjsbdk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xfwedegz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hmaejovx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sbhbnivl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbkgoke.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsemphd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hibbrbxc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mlmgtfyj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mjjtydzm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3eqtwcdin.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qbrebyxx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3eddufhej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xwjokzne.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omlrvlor.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3igqfpkrp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3leqeoygk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wdzhhiqt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xqsnyahz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ixwborqr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mkigatcw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jcpolsej.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvetpldl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3krgucppl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzdnrxmi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3scarljor.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3brysjdmw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjpqqdnl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sytciqrn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nqywgjvc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xwljpgnc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vqcqckuj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3feemjnqy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mevklfuf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bzouswhx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wjbjpceg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jwjswgmk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xqkcyfcx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3elrlpdni.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zncwojoo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3musevlct.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bzwhccpw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ppggejyu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tsgmzjtq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wpwcwbus.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xvhjunjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udhankol.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vshebpnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmyyyfev.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlezwuox.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ummaiflw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmueorjy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eupwjjyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3plcylzkf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bhjgardo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ynwtkysh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjsungak.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dkhmezcx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aljajeat.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3sylgvdut.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqmunfbi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fwjrehja.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbeoiwad.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nziusibz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmtttpyc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pifdmjvy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bilkabqo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gbikanvv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hziyaqha.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3elyikmyn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kdpnczdd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugdzjysm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvbruhc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3boaaxyow.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdvzvnwm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tzrzpuwt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qbvcwite.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3azvcqwbu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cnrhjbkc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vskavihc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gfqjcrmu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rlnekqbn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hlzopedp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3czjtgjho.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hxwrlwuk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gyeopfde.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tohcvkdb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yfghhlfb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3scpnggkg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ryrkgvti.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ekujpxdh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yvbkzjng.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qalxjmhm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rosyitoo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cnbdaypm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cbkkdmhc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3yzhanwll.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xgssvvlc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jishhbph.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yacfykxo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ntyhjhzr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mnfuucvc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3igqzwxqk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hhwrrkmu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bpyzpqxo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iukubrwa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pngovhzh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nprapmnp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ofjdwmud.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3oaikkitn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ljvqyhmk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xlaaphnm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zvrnhcnh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3azkxqqdb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qykhqieh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxouwwqj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3riknmhxz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mhqejpbl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ijaqwuwy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmtcaqzs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cpdahxgq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3unhfglik.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3huqgescc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3timyqebv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3acytykpj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pfztjowu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3twunvaxl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3icxbxrjl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pndbvgbq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rqjehxpl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ycgqhxoh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3egbfiphq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3loknosjc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yufkmkvz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xlwjetch.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3athmyhpb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3trspkbct.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ssosziye.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bidxliyv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3chuouxey.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jnpiclas.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3azbnxxcp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3excdngpk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ljucwwkj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xbquwbra.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kdvnaxmw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tpvdatqz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fqhyeqgj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3froyhcrw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qffzsske.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jkscvjjt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iyrurpvo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qfmoyegt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3lazempsn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3carcwozk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lsyxcfhe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrqevhss.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vncwqbzl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ttnyauap.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3putzxmpc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ssrmyypu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eexkbucg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hqyhdgad.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3fzfpmwix.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vksnumbk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3myfaezkm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jpejovuj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kszgjesd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3thtkzgok.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3faxmrzsa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpuqigqj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzphnyjn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ysjpntaa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3imsygvfd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ynhgcqfa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pnjtyeua.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pfxvencc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lrtqjjjr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dbjgyqem.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tievtnjd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jaocyzki.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uxmvkczu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jqyekmrw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sogeaayp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qjsbphsw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lpsmzvhj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mojuczfb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hnbmesok.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rfuqsrbg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzfhrybt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zhjrdbhn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ppqjmnpu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xygqfjoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtbjltmu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3egmrnbgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzoxuhkw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qvzixtre.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cfqpktlq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3piblzdoz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ophwkumi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bksbrejf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3btsttxff.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fmoajcnr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cxejzvmg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fsqpcxpl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nfejhcxw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lyhzpuil.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qkevtbnx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dmasnvzz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3knkttwul.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wkqhthfi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aohtniik.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3afrctaul.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pthjfyzu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wavdgogp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kpkyfslm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gapvgmws.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wzjtfvwn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cpmmggqq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fwblwwmh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xqdkipdk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkqobnbp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hlbvshkj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mwwhiity.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zywpusgv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jvddcepk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pexxvjol.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hfojhltc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hxgwohyv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jwugqxvv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whxigykq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3iacfxlod.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hhngmsso.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3amuwckdc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xytpypif.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ftilynwd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pirjqldx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ypfmvzsd.html


<!-- 参考信息 -->