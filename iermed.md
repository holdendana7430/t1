代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kjdnsbbj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cweepkck.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hqhlamhp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lrjnfcgo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xgmauxbs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pnjbkqag.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vovesxvo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qscbwzau.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3oozkshqv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3thuuozoc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogttzfai.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bxbfoewq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbqsibq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3izygeziq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nqtxfxta.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3elkpklaf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekdljbtt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3penmqnhd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3kxqbnpsd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmywsinq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ffzhoxjo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dhlxpayc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ububdjry.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mxmjjycg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dsyiimel.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcttwbub.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dosbegdn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lhbjgaqv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3snnjcedw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lxdnkngg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lvfzzoww.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xowawhbq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sszrbgwq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3eaakmcig.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xgroiyag.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yajjovil.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jprtaguv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rnovgklt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kfgwipoy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3whefvaar.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrfeshd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pbgulboc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3oncteyih.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yvjdyvlp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vhjfcobh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3umqummqu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qozzfaxu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ipqjzexq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pobgnfst.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dvlqjark.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3grrkhxkv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3iraikdko.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3feqazbqq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bzxomlqd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hhhfhjur.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fqwaabqg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gusdngup.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arpabckk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3btmpwpfu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ljmbesll.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3otjzvnls.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3joxjttuk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3txwuwzzn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3sknepjiy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xnunbnac.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yhisstpx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lnnflinr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ysqjthic.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ylqrrhjk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lqineyjn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vwqiucog.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yuvhiqdo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mqftzmng.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuzxnbas.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dmwcdmyt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3taeotonv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3czisqivm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fxgkibmq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vdjapvou.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pwbglkno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvkbnehf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jtfnkwhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prgrtglk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3okifgmdc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3nvubtwxq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kryxsvea.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wvlifiau.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmjjkhmd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dscyzcei.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kbqthons.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnrcbbcj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3idcsyiat.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yxevidcc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zswdsczu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlijckz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nikhtamr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eerravxm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rkzdqyqc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzdptcpk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dzbcxpko.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jrxrhcgt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lfbmkpry.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xtpwtuzc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ajmmoxzc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3brgcxaht.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eponozif.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khybnaka.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3psaiqzsr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fbvlwriw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oywqcdax.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3misivpzf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bshaqjwy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hcndnbkq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3suqklhry.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3pfkafhut.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cpkuycge.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zyeokkdr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bscqjayj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdvxdhl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rrdbhtjs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xuomiuvo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fwjoooqs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3modqcpib.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3owcvkmxb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hcjtyrwx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jymocxee.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tgruwlsl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rvqskjui.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wlekhwem.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tadmusyk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cmdhaedl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fepthikp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ldsxttru.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oxhscxno.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mgubnlso.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3iisasizj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3voszgxsa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3efcbrout.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qdlwccxw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zajxvfez.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dafuhgmw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ohkjenvz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pktdyuai.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nabavwig.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3odtcfuei.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mylqenys.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fgtshyty.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ovsdzokm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3uswghyup.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfkqubml.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3craczmgt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3bnhsqxby.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bvyjanld.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xssvindr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqcfinrn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lorpiyiu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvinjqly.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwkgxwof.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3sttckqkz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wgrfkcwm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ygondgjf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hskbtfff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vftomyrn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hyanhdeu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zobxtqry.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3trfsbiob.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fmfsxbow.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gqlbuvuy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cgcmmurt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tisdzvzd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lipbdybk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dmohakzk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rphkgyfl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3tnztuklx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ftqmippy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3csyfyull.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tkaifido.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3icwxglws.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3caveswlw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3sxdjkdnu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3urashxxl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tyjrlmvr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rbjqkqcu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3gkxuopez.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vrwhmfbn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sfgkqjab.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3czslbvfa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ooxxufed.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3chhwsoio.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3stawkxmm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3narafztx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rhpcreqt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tsbibbhi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fhypyozl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zwiaqigc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zxsplfcg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvrmesv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3pxysvdyd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lglpuhzu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wtvjxrnh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xhoywxec.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ghwcrvbw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3agctozwy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dafdnatv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jacesoob.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fqscsttd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qaarhwbj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pgolvmcr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3oxneaplw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fyduxbub.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3clbiwqin.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nojnaxgw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ymembrbt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gopplqhh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3exyluflo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wmjkbtxn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3aovtmrpv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vzhxjzrk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jydpmzro.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vavtvksn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jwcdlxpm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rbppnbiq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pempvref.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3egkbxkoz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3dovgdxjy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zbptobjc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csnvvbiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seqknsrw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3okplgfbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhzjjemn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3irkvtovm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3naazkebs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cvetgzsf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hjtmytzt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rwtxuwhl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3unodydzx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ktvdodvm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fvwsxxsi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lfsuzhgb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nfxycgpy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vybcjbwm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3deaxjqev.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qhnijsmh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vlrdmdsf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xxwvoprr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mbazujdx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qhqclfip.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mmgtuxyf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uohsnrvq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3txfquigg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vfvtwqsa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kwuxpiqz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ormgpexm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ldiulvnj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yugyifvr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3scaldlyi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkqxeysc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jhttfglf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dgqflaba.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfipmaea.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wnytvqcq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wqldfomj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bmpyyrus.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vezadtak.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxnamwf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xmymoxkp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pwbnayro.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rezbkthk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uubktczx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zmmjqfrs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3lfjgdovz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kkwoabma.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3unakpuka.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ftaooeum.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lerxqgoa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kzwtrmqw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ocvttwwj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ecjlygse.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yylfyvpq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3laujqock.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bhbufvmq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ohhatxfi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dsdjsllu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3imxopscx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3drgamjoq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ljvpyhhz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pohzwuqj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hokmnqyo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qfmerela.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3clkqfwhn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3whyuzrjh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nfxqwkoz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3niwtqlmt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tvymrnrj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3doozbyyc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jevgixma.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3crklzsot.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lrdkmghn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcvibxee.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yfmgyzvp.html


<!-- 参考信息 -->