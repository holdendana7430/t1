代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dugxwxcm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2slxaotbt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bgdlphsk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwlvuymo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dypfmcas.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzfmefjj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ebviadqe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwczvscv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lujrpglo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rjrfxegt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qrvxtlmi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mzvlcoli.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ofdjowho.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eflrmxsa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uuhkewbu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zumanbkz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hirevady.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zxszekro.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2veqdttim.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fzyuxxvi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2enjnspru.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pntiozpr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xsgpikoy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbzeplrg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsyqggdi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtlyuzbk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ubntgaqd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rxuvhnpv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwmoljdw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nfxqsfwe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yxomrdax.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2awbkzjou.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jejofsvm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nnxmzous.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kueoqvke.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mylumjoc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wiqidvbn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckjcsytn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bejsrrtd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2icmetuxe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2swgufnfe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2evctrswt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tdkkmwmn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wubljhqh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jfdsairb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wwmljegs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kteynucd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vkezmdle.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2abozkajp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2begcwagg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hgyhycqs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pecabskq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2prpojmqb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2junaemvm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tdsiarhd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2mxgnvkrv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ycatuvud.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hfgcsrqk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ayntlqii.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lurzngwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dtopwauy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xhpveqol.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2swljfkre.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zoxzgnav.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dlycmwdk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2omrfccwy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hclbbvzc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2iqbppjws.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmgkjcsd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wioxskdt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2empdedeo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzdowyyn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jvfhvpcm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ytmrgxsg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fswuagtk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rkloquun.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jphvrnqx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xgkksvlq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zkhyjona.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yhpuoevr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2akywcphi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2izaimqna.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rwdsjjto.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kekkjfxh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jcwsurwq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwhlfqms.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mvinyiem.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2afzemwge.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sunngtht.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zizjwzzm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pyixlopf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kesczzvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryuphtwx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wytnemjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnzpjrfq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vhluxjfg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2suczqwtq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcqphjgn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwosoivi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yjxbaowy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghqngebs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwjzrdw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2znpleznn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2soitjgux.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mdapttte.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vbiqawhu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pmeehgke.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgtzdczr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnfiiwzo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kyqvhsmo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2lyewybzi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qgyzqcss.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rvudptpd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nnwvzdzh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xkvtaaac.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnjiwuwo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aghwigpt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cnrldufh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2isynxuqt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rtqyyigf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2eslfoayf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xvbvlzfz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mhdxoovg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2helntzti.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yykldnms.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2arpskhek.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hrkelpqw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2axwmsrfm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rlgzgczp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqnatcm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2myxwhvee.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2osdqhrsv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2clfdomrp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ufqnlolz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2scswgjvx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ufmxzoai.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2unaaxdam.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ujjfrppo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gdevdawj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pmshesiz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jpogjyce.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hmgbmzdu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lbmvwbgd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ytwxhccd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cvcihtag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fljtohvf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kggeqcit.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vbfjujks.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yvfskgoh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2eiyvcmqs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2kkmentmj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pmaehztz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2iocsqgri.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ivfuuqhm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yekkvwtn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ypioinpf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wluyerem.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vlmtinat.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zvfvdudr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ebhpssly.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nssafadz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2szrpvqek.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iuqeueha.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cfeipzyo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgntzkmu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2upbbphao.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgrxpinw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2drnkzwhn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fulpyvhp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbdjaomz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2klxipkzt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fsvcjiom.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dpjsbaaw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cfmsnbsa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2auofozfa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vlrbodeh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mwkrociu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jgvfqlll.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cxubmgax.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cuyysxzw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2etawyhid.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mbmnlblv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zywosife.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2cumtqzqt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sptwmmdm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ksmhpjah.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2htyiqqpo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2exdrrwqy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uckyfcpt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qkbemvmh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2flisvnsb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2scqeyqey.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ryirfoxf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfozpyl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rdsbonkg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jrqrxgnl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fzkaxwih.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ragjnghf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tstquhwq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yukgckuc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gvxlulqv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kmrntgzr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbdltste.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2djudpuaf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yqehxzlz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bhcknlti.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wpvasejm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhtyanch.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pqkwjzyt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lcawzbqk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2yvdeaqrm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2trtozezp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dstmzqjj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pqgfmmzm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jwujctew.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ntiwtvtf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjawhsdx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzlgdnmy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rfuwqhpw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wcbaczsx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qnjextdr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wrllrwkg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mqypjtoq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2doonumtc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tznnmvvt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gofcguee.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zmrhruev.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jhjbdmpz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jdoycaxr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2swbbsulv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2brsfwzbf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nlpimcyc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2llomecxd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jtdatwzv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ibauftod.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kmctxbif.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2npcodmja.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2smvchgjh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cexdchbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mouulvev.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tmghxnth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njjmqptr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uqtzegzd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dfoeghwl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jxedbvoy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2miiebwde.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qfxqfegs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2agxvphhf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2poaplvhx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iaghtjio.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cwtmemff.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dxmdwrcr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iucvbadf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oscxrcpe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jslmdnoz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rypahjnr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2uqtzzvmy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2agjmxgol.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nzxtcedq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wwqmqpdp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2irbusrji.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qngpvjqg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bugfosdp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ojythitc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sadzxpxg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2awuakids.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ioqgjaxy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gvczzvij.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gqqreuzv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ygockvqy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2givwhmno.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hvhoppky.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pudlfdkq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vlzvtedu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ssybgcoy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2arrbmxmr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdrxnkp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ntoxbxvm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mhvizyvv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ilkzciog.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sqgeboop.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dhixhqsa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vjvksisc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gvnbcpcg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yjsnhbuv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dimltoso.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lvlbqcll.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zcbjgxdu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbwbqlzo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hlpohpgx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2icehnumw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wthqnvzx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2gbqmyhfl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mqytgwlo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lhlctlif.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2grroaylp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2mbqhgobq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wyasgfbv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2earonkyo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ooetgpfo.html


<!-- 参考信息 -->