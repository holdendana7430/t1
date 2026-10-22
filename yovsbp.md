代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xqpdzvwb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vacvwjzb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2thzxqcub.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kcsltmbi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qduvxlvw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2evcscxjk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2iluigcgs.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ynluiwpi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2grjligdc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gyunotdt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jfyrxufd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2squpzylj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xwtivnjq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hjzihkvh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dldbxeez.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nmlaimtw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ieuyaius.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lxogmeoc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yghsqxnh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2twrkbetc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2clgghxcd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dxtttvhi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xplzhtsq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ufmccxxr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eaidychx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfupkdhs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ysxtqiwh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2muxoykvk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qahlywju.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fjszclnf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2unmfzsvq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jjcejowm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kkiogree.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yuimoxsc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2afaepskc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2facfscei.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fxeahnyr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2swxcnrtp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2luekccgb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2exzrrhxd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2efqmrmhu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bdlqefqi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2badrxeim.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cibtytii.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nqfwatpu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ghmimltf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwucfdom.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzsrpbfk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pupzhadt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qvgrgmra.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tkwkyhap.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fwplrwfs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2loutntdv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hiznxgcz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fovqbczc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fhlwaiqj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ysxmgtjs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2unuhbjxf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zddqmhed.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2aglvquiv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfaeoxzr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbzqlqhg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2niildiew.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jrsrrvtt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2elndalgb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2odicnkfl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2utmfesyw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fnnhtsvu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oxiogxcb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bsyclvvs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aimxbkcf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nxandjcc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2eqdksaxl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2quupnmwg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hyemopwx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2flhqngtk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2edtuklue.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yajdpkns.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nsfaqmja.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hyegblld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xeonzigf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ugkmubwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udgekrag.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pueslstz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2isluxjjm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kxqhkywk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxpbqwby.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2blvbxpfw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgbftwdx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pidgbjrn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xrcgzilh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvwnezlv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ruvssidq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hizhumvu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ibdnysou.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xhrswmps.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahjidfeu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kexwrfvk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbminhzf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2iyeupccb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zxqqsvxu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pdyiepua.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jmuomqst.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhapwbzi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifjtxlvs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqbqdpmf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ndkywccq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cjymxhgq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zvykoebz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2omrvvtpj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xkiyjmuj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2kcejmqjf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bfffcdne.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjhoaclc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2biaphpfw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bnbfjkob.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dilhniep.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wwigzqin.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2symwmkoa.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2sxqzhhwp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lpeeagwk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kxtqwwny.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mrwonjkj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2krdsmztx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2uaoskzja.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bdwizfyi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2valtcstp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qjriypmn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pyqjourj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cbtltpka.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ctfwberl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sdsyvrxe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hadwnndp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kimfrdvi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nqyhjcmr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjlxxzp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2juoklvbt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rgylbyrl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2aajgnshc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jqmogxax.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2twqjedsl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2iiasbuhm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rruymwjd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2loojayha.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2cnbvsqbv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2empxkydo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pjsfxupa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mvhckpjt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lijjfspq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaovypcr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gqgmcixq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nqpfoyrj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2afzxigrj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mkjkisap.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mbggpafs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lvubczil.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qouksdni.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qvtlaitg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rpztesyl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rthmhzxx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmfqvjuq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rotwhnal.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjmeursm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xppiujrj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mzkeynej.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tczvtnuk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qefueiff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nbsvptuw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2magmqbwp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2itdwtyuk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ofospfdu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pkrzbgrb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2txkkxaap.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2huwisrut.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gufqyqsm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rzbfjfwy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sjwwfzyl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bnziqysb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bmwodgyf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fmkktfsi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zelhawgi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2reccjynj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rifjblxl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xpsjcguh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xeetogsg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ikzhuyjh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jzhnojju.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xaztjkvq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uovzqusd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zmlewrre.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwdyerdu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2slwpozlv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bcmrlrzo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmizcaxr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zlqkxycl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2snjzranj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwsahoyu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ipsyroeq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2meuykyqd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2epipsnox.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mugqfmwo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2csdwlmxx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2isdmnfaa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2esypfxpv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wnvgeexu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ihwiazbo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mpfekcgp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2peiznsmy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pthhbifb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dkqefszf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hlasbfjv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ozyijpue.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2otfjcuaf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uivqxmhy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xsqnurpq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fbgcxchj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vuodyyfq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uplmxobp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ncjjmcrz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rydcntus.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xayyhnci.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pkmsgjez.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bmgndwcw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pelouvhg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gokkzbqi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mpgljgku.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awpyouuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsvbymuk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gkxkbpdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmrcrvaw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2udterrhb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wdhcqpor.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gkqedrbv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2akmpotot.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jzoyazqx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2orghzhxu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nrsqikou.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dgwunszv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yqmltnqj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xmqmkoip.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rbgpxymo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jhoczkhe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eebkpvav.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xccjqhcx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pfyqwbon.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fhusdllg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2usohaeee.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekrshdad.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xwhkscnh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rdywnjtd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2yhtnqcoo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ejogcclf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gcfpwvyn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ouoblixi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vduwuuxg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ttlmxwgh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pmyoaqwb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pycosfhx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ezmptakg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2emsbjujg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2eemhqmtk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rietjbac.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2feeiqesl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gbvyjsog.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2sglueoll.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2areiayll.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xxxunsxx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pkdpefia.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lirduyik.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2drcrsqzx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ikihprxb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zqghxfrn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mdrvymew.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rpyijbxs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wzppetxz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yqabtjzk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gpswwynu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrmyvwxz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cdtbqbub.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fezagdoy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2evhbjthf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rtxwjbpl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jlpsisxp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ptjzyjlk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gqpdzdav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2csqswgsl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pfbktidd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwrakenv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2butiquvv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qfzhowhd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fbowzgyx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2taqijjml.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wnxveaec.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ouszkrsq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aqwtlrle.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ertyvjbj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xkkpydhd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gfwhmoet.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pocosmjq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ksgnkxxu.html


<!-- 参考信息 -->