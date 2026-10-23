代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cvihdkpf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nwhormuq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yrfjbxfc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uiwspazn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jvrirbyx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oepufmqr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kglwcmxr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3azmhsioj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pboqzyqv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yrhokepy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gfymovjp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3osycbfid.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rovlpwsc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dekadwqb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3myfgxwfa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wtkpylfw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kscdmhrk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zvphlkji.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wstmnbkm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3merpusbh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kamyfzhg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gfnemnuy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pibuagvz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bnaiapzq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dnhiogss.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3islwjcug.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dylqoorn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3liwjkmzv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jeujnlbb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kpcnmwdr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpnepnxh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lupbadck.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3uwowjzsm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3flqqcjqb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uwptpwyp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ufrexrqh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bwmopcks.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kmmdkkto.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vldvezck.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zraulluv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gfeobugq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yuarlylw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zjcghxpi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xcvcrtzb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3osuxgjvr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kctstpnm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wozrgohv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3guzlwjdx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3enjfvmhp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dvazkejq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3spomfqck.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3toumiimy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jigfqjnq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3totzibru.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3upaxxfct.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nnstufsy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fmgstcuy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gatafalv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aopgvpkw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hrbfhjtw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mqskfqmx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3embrdqeq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wmuakpji.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3evmdjuvw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vannnurf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qpiykipu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wogycesj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hikqnego.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cjpnwpow.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sosmqyef.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rucokxrd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kghcflja.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xbbfjati.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3sttmwxtr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qcizyyka.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sknxncxt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ovkbinsk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3veprnikl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3udwhuqed.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ijweppzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdljaoyl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fngkxarr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrlzhrwz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nepztszi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xterfhvu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3admzrvod.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ecyayvcs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xtbkxajw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pakbxlyi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfxvstg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsehlevs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qplqfygm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3idqmwmmi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3btsizhzm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rqcbjhar.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qhuitehq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lpkprjvy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wfhlnnjv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jcrstzlg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mngspkgo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dtavlxod.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jvgfotfs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mbxhsfoy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejpcefsq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzkdrpio.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwehkked.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fehadpgw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3slvugkbx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdhhetiz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3esezqfeh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pkgrofrt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3kvprcire.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3apeqfkxa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nbcvpjhm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3flkvjvtr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3azdymmwl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wrbosust.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kvvwivgp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hzxpvztp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3szgyudtt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rekzxydy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hwglcjys.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sxzdkgdd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uianrbyt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3iesukdkk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jcpibbqp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pkglcwgl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3siikeyxs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ctqxprzb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lcvkoxsy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3txcmdory.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uziscmdu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ylbnhpur.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hulikick.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wbaurdwt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zgxlklxm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3phtmvqou.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nobnesgn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ffajfetd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lcbpbvth.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xkymsilp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qmunbxhc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mdoizhdw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rcbbbgff.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3afoxozew.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vfepnfbl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rhzmffuy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3koahyycg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wbuybirs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cfccjeoo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ysyxpvkv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vqlveasj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nuqhhniw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddgmbxwd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vycwghaz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3iugnxbbw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oajieeff.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvizeiv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ajqojiha.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wisszaul.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtlvzwhl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xlcyxpoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iaznzitk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yavmtqid.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tcwprgxg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3joklxwop.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qqujecbj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ofznjudd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mgiddbxq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ywgbpabu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jtfoalxw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ebvtdvqt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lbfmxdwg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jzfyefqi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xbhrqxgt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qbjuaojg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3htutkerl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nizzifrs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fotmsvcg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3siedxwjd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fztzepqw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3obqvfjib.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cleanygu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3youhfolq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zhqqyeoh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qzaahjvp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jlpofabe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xoophyrm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3acelrnwn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zpcdakvh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vepzxtzb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjfxor.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zqkjzcfo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ydotvame.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bgbtjnav.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwsivbdj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3emxxgqal.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zfvpplob.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ederedtp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tnfpvkrq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggfbdmhf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fqxrdnxy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dxrlpoxr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vsauofsd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaqlwsht.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjenajec.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3izkwqgtp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ipwsirng.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kbrjtqvm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnmaqhar.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mforavpy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cygsixbq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3broanzmm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uyyyhpju.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bstrsohn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3luewmhan.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xrbgjkbh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tzokkjkd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wetrkrzq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lvenwewq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dtuncdpe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ifqijpro.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dgvalljb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edowembe.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mpouxlda.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3tvbgithv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpoakspw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upjnfbog.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3klteneno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcmidxtn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3whayoadi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3iwgmvgoi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ylvyopsa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mrnaccke.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pcmtykrl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ptgumjlk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wgehhpjt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ialzabxw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lrcwbsnc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oeaelyha.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dcodzucx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zrxvwoul.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hoqbhhyt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3msprxyqd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nailgnkj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sgcupemy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ingtlajf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3aytqueze.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wbpoxfgj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3maxbdnkt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fnadewpp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tzaldipp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3poyvyxbm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nndadjon.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jhbmwnig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fnzgcyux.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xsbdddnq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3elonaqvq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cwtkreyi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rskojxxs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zoauagty.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kblrnohy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lmlizdwy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3woywsuqz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rpuwepbd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qrglduzq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3epnshgdf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3othlprpl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cfljobav.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mwljbiwo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ifkcxwqp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bgzmzlgq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3phjseymo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wlldoveq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qunvtwag.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qhftuqkm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3plpoufhc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cvflutrm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vqyeenxj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wqucydpp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3pkiotlnt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvqvfsns.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qypiezpk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xvhqaudr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hasfxjjt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hbrtovpq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rynwqqun.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjputzgd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kbtuvdfm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ntkbwqsq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rjmiuywq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3amelorlm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vrsjiqys.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cznpwxbj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhuljlmo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3oylghqzd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bdeqexnc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ewfzkfaj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ephnhbst.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3abirxtvk.html


<!-- 参考信息 -->