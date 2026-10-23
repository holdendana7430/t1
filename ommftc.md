代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3iljjxihm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3prsytazi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wumfscev.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ksnvxjyj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3acyczqme.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3buiutemc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hhpimkdk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mpphebwe.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mxdxpqyh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3klllnwsg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzcwuy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cjgwgkrh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nlgbybut.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3urehckxx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3orkvfogd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hzzniwrt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvvdplgs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gwpyxyfz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ffijwwux.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sgckzqnn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3snlyipkf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cbfccptt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3esegxypq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fyfhubeg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3idkafzql.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eszthrdy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkpiqmp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oesucnzm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmzutqu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkqywjkj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qdaampxk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fyloauqy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xkndfpna.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hslqicaq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3guwjygga.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xeximqpc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zglxoldc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3efmjintl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rysweiba.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cnruqlgd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hufqpmvm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hohmqqkd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqpcspk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ntsifqzp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sypwqbvl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3inkhybta.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dvfezpgx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3swzezfap.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3omqgngwf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3alugxpmo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3epylknhk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zrctvxvu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qzpkppmb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mnbinhum.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gbcvvzul.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tfkmdxvd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fybzjuje.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dnyhzqba.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mwjqmcaf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kizbptmt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zoepqdei.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eljclzrn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nndnugal.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ialbllik.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ridohjhv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnjpyilv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kiifhfmn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3acwsynoy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jcwgewxw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wjzujygn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3izvxkcxc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iecmjbci.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tfnxgwiw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qwugrcan.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gwbclzsj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3smjtdurm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3nvgyrcww.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkuahpwi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jvwimrjr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3waqjllng.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dxpaywdx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vxjprklv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hymbwtyp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eipodrbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhznjuky.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oetsiyll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwnjspfi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3webimrxn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oxdobokd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ojtvzopa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jilgcfqu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vcqccnyg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jniqibho.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vcvslkai.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oliaxbhi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3onyghlhn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3brbqupcz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zxsunqqt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hwecoiof.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3woemenwt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ketqewwv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3iaeozqhb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xvlahmtt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3jrvnmbqz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dgevdxzz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujsesrwt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3izbauzqf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wmufttao.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hvzsuurn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dphtnaly.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3illxxtdz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wlyykuut.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xqoomnos.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zgpyiryr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3msmqhsoy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3sshklowp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rqbmosql.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tymcqdxq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ylspmsxe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mwwrchug.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdvtuobd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdmnias.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xgtvicer.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cfmtenar.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xqdbmzvg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3eknrdixa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nygxkqii.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3btakvifk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3theugqpf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ivmopoll.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bypukpsh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ndzbdylu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pkfilpen.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rilfckiq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3llppicfs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yevgwpuy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zarfiyil.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pzwtvofy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3soflwgtd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3znnzkwne.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dtxlwwld.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3phvtqvuc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pxnvwdwa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxyuzwdo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zalfcbjt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ikcjtzty.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xhbmsfro.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gwbvhdvw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3oifuvzre.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mdjrsqyr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3siazhljd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bgcjvedx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3usneaetr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xwlsntbo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwxjvaac.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xpiwmwcg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3aukckvur.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3oqeksspp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zszeoxim.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrvdshiz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3djbxujwo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3smmdjrez.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3obhzxfpo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3riakiebw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cklnoscz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bmpsalvy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fycnacuj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcoalog.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lrmebvtc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uevbqxaw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sgsgxsey.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3usjpzama.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gdsnavsw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vxahqvnv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ibgkkjmn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qwrfkbzm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3drfryhnv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hpdpzjyo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ihmrvyou.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mfuikenp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pakhjpga.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cbwhochi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jzilwydl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jabvqiqv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nnmildbs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3onwcoonf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tntvevko.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qpdwrtra.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dhnmbynh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wdfhtxzn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ekeyltal.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jrzlbklm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dqftndaa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3iznklqce.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pbhrhfxu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mkmvsbnp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3rqhdzndp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xiraazqy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mfcejrwa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3krgsooln.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pjdykxtn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3iaxajten.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fwdddewf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3klzpxtgk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3hotkgkzk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vjbjivrm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3acsasvqb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3evbcdrzq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtkjhtfb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3twhqbyjs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rkubfmys.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lsnvvwbt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ghxkzloj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zpvdncnx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ovspzgut.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mqnrvxnf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ipatypok.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vwjsqfqf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3phqpilkk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hwkwxxkc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3avxgfolg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jtskugjz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rfawltuj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lsronanw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3nrkhwmha.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3keoinhfy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dxuxmiyj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zkdrrxuq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rnvaiuxi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ahnpcoip.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pelosdot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjdiqxjr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jzxjbzsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjtsodop.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jqnrofda.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cdpxgzmt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dxsefpsd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ocjlxgvo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yxvudaqv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dyschxif.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3znbqszib.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ajbwtxdi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ysqweenn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3tppfqmhm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qgcykfrf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3grzokitl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dthxifnr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gdugkcir.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rfqoupmi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkovdyl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbkrzuo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3yceebxpf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jqlhpyye.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dkuhimfn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycqxjdqe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3yfiftuxs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frzgvihs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oznvampz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dlkotswm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxtucuu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mspnrazd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3icsawzyy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcynomei.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zaeifirz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mqgjjfhr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fkyuywch.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdtffsyr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nogpruek.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iglpcbel.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtlvghme.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mgckdewn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3liicsxcl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tnyevhlh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kcegrfqh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jymiuduw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zfgvsxmq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cyjwemii.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dlbghvkj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bfslqpjl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3btuqanjg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uiiebkhb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lvtrplbs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jxscubki.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wltpgjhw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3okvkrhnt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wfxkfnzp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kqnglcbb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3psxbdcvi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vpoclihf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3kmlivjqu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3npycynol.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jykmhlao.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3scmfyddg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uonuttgi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3uvvfgcyk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3inudfkaa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3znapdphw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wydsczoz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ozdnegwo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lycnaxen.html


<!-- 参考信息 -->