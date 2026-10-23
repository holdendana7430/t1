代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eufchhwk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wozbuiue.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3moqzugec.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3knqcxgtp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jssfkcwl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xwslcofx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jmsquurv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kvlfbfqq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3oausjiwn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3txjbqzei.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ujxrklor.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wmikuusl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bismvtna.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3layguiwp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3umimrzlj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3giqtefun.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3akhnmqzw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tfsxpugm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tukpqeji.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3klgrtjwg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abkbmsmv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hbgcaqqk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3guqyzvgh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yfahwoug.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ceopjaht.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dxtpagug.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jurvbpdb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbkfkinb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vhmxydmf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xebomvmb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3trtubsab.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3skhjuphx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dccjhbrw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wswaorco.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ewizmkwh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sqmjxedm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aafdkvmf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clvdriqk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yuaxoknz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjtreifd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3uwnypbfp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3unmbbscl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mzcdlsnq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3paxeikin.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tnuqhpai.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3efddgepy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iffcyyed.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qpimrjrd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hlqjvcvu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3acmbhmfl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gcltzgpu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3awntdarm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3fperzvwu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qdmdbxvt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rwjnkqrz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3epcqwjwl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3coukjrus.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dqfoxqef.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lelitalr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcpfceo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3muairqrb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hptrucqs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3aaaftfro.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mzudtmcs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvdfmcr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jtpuhlpm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lrtqjjdx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3exvcoscr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fjgzofmg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uxspioth.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fkzdvndn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ehcxtpok.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dftffurd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ntwkxfbb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3anmprknr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vydnokka.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uyqprurh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qgaghoyg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gysxwjka.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gkyckuzo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3otflzgsy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtkkhaay.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3harhosok.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dwoeuovk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gvymdjdp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wznstmrd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3bnbdobeb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lnxcjcma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgofxlhv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3woycbgei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysqrpcax.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3perkifkr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3alonjtsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lmrmiuci.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jndproyn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ikqltyfw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3talacmor.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xqislmqx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rolqlcwy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqimlmng.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gklpavhy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fiaxudaz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wgnwounw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hqvtrvca.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lkikyoyo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rndlcnhf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qtucpiis.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xsmjfdka.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bbwbwkxj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hbvmrbfu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uabqmpho.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rvxfaftu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3csouzphs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mfcblsoo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fumbciup.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jgqebbox.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqbyzafy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vkyxduvw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbszjqaw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3uewioweg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ptptjqza.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqlzjiiv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xocvuzkl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3oiduwicp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3abpxfphu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rdujejkg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eewylkhd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3exdgnkhb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cujwbmgh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ffvdowdf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3loqcamne.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xbxhprpo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pqcyghvr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kizsrdbg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dtylwyzy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3lopsxrlg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ccnjjmjf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3poghgrlm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cvdomndm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3goybtqjx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3myaksiiu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kjxzgwzc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wylxlsjn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3isldfwoi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3auhcabao.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mnruvttp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3anxtclus.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehzmwias.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgapjpb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jkimiqup.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kfpfqefo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3iuxiuwse.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vpamytok.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bjfnunyj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xaakbmbd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mzsbhatx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yekwkyub.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bkeeugla.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bntizuhz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wdooxtyf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3endvtnvf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3sbtwopyt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hgdecfew.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3amhroxye.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksgotfrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3amkixaxx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uptdbcza.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jiaiiwfj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bqjzgdam.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rtsdqake.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cezdxbbz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cntibbqy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sybmobfj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jfpazxok.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fsaftvvm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rizcxqtg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3onrriodb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dtmtirdq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yzassrff.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3soaeyyjz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rgceehrd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3znbrdjpm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ktyhynjw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kxbvwiwe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lwfqhxnl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lynvdfzu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3besbwdnb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3akaolrpi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mommhtdu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3llxtagnw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xopishxa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3msjzorhv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3damipybq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wfnmcbob.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mzwkmphm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ozbxwxwf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vxmqxzgs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lzzrqkyd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3maisdpte.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3otmkuryg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3klwbjykd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcdmjnmo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tmytickq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzsokbjy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aivvphoq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lmdqngyf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kpccubdq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ocpfexig.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3szhyunaq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rnydwsgu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cvqszygk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ygglynnk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3houkycrp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3leghaaxz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wbrwuudg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bmwtgsku.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ucwrftnc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lofnyjns.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hpviocpr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bachaksj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cflzdmnb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nylhwmvp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ccbgpzfb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cwzqksya.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fcliafjk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dmixsyfv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lnqdxinc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3znsjbafr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wdfecnss.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vjvvunwn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3sjeltzoy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jlfdrrcp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vjtmbqqw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zeieeqhh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xalaszom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pargteen.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qhmtjvst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njptsgik.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zyocbivz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ddvtshpg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3caklmuhp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tucijhgn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qbwcpalr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3oayujoxu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3yhbqutyi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3txeolizw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pxwstbyh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rfvsztnm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fszhiogm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3glnfshbu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dghuligj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbsnawhh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3aqekawgk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3aycbfyyp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nlrwthot.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wfwjfhjj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ctwekrrc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ujiepqjp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rbxkcrsn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3buyoczau.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ejsspzae.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3etjiavek.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gssyfyma.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mibwsohe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wceycedp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hioncoll.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3bavnwxte.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3boeipmeo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lhncghdw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zlhiboav.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3dtzbiado.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3unwemvpx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hhryhnod.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gutldtue.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kbpujkte.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gyfuxrsl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3inlvavrd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uaugffjh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kmvkrhva.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rggaxrmc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zhgcclff.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tpmphbpc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ilbfyyid.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ppyodqrt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmahtfjg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdsrzmfv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fnzjtrmu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zlvljceb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3itjwanlw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmparkac.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3axdxacpt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qelncwvb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ohunspmk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hkdwhosu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zcpfsypx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vtjywsnf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zfsliavs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yrjbbfre.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jyxfudqr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kbxndcmz.html


<!-- 参考信息 -->