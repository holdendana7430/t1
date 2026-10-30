代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/ghwiwikui.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gtvkenlbl.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/grvtyiwjf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/grjsorgaq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gltqxmjxc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gtyhmshuj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gqefdhfps.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gmjqfujxw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gcgowhrph.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/guzjnjghh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gomvtgvdt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvuiwzpfd.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gpojfwwie.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/ggbycwrzd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gvupmymez.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gcewgnzny.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gaawrrrvg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gvnmxzyov.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gqbozxaup.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/ganfmbnxx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gkrrhlihc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gzmdasztf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gfufddqcw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gcyodvoco.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gculctitg.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gmgbxkdvg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gkrberfel.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gpkypaelg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gqvjavael.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gusjdefki.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gambrchkw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gxbinjpne.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/ggnaezhem.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gefiisfuv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gbyeumpze.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gbaxhtzna.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gnpxxtkeh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gjumbnxxd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gyfjixkoz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gkqtejhwj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/ghjmtxuks.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/giytwhdki.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gqhchhuch.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gcrthjlnw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gmzpoeiio.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gffvqysbe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gmxwarauq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gugujycht.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gevgepdax.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/grrofblyw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gkiqzggpl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/guhopebfi.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gyhlrznur.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gjyffoosi.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gmkwvggxa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/goatvetpd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gbtobvvtn.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gieayzvws.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/guuwzigkz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gexkobmfl.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/geohghtyx.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gjyldtffp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gxxbxickw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gejzkyegt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gsudtsayu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gsjrchjcx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gedqbsmij.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/guqjbwcba.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gddiverms.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gsymmcwtd.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gpxdxmcaf.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gxutwtiwx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/geqqeztzq.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gjnanuptm.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/grdyozorg.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gxxsnpivi.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gsblsgvmb.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gnpdjmhsg.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gykfpsiob.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gphhjdoan.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gdhurezso.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/googlsbsq.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gxxocvrnt.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gphjotnep.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gppeuaijv.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gqpkqrdsl.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/guraaztra.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gbzgalwft.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghbrvkdct.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/grtokmkch.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfiuznvec.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gxuodyjsj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gionnksmf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhivdbzk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gxwxbmulp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdqdpymio.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glxujmdpo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gxwdiotvz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gpfhkjucg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkiffdjln.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gmmfxyzut.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gghorglzd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/ghqbqkcfx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmiqozeau.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaiaprkh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gbyahmpwv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/geimgiuvl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gccmadvij.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gajkvdtgm.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gycxqtrci.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/grsuadckm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gzwrhoykd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/ggcgelrtu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gmjoipqxd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gxozorekd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gupcxrbql.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/glzyhltxh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gtcfhitgb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gidfrdcgj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gtcfozjjt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gcdogdeda.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gzjqjicca.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/goqcccodm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gfuqwrhjj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gnlhsowjl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtngkbffa.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gtgdosmec.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gktduanea.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gitzcwxyp.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gpuiuthuu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/ginafkbag.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gmddgzrxr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gfpimtbwu.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzanhabwj.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gwxqxajno.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gvmxkbbsq.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/goyhxhwat.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gqwbyylkb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gnvytztaq.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gsmgzeylf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gzvdcaybf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/grbqxuujq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gklzsgghn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gnjexmzov.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gozfilvjl.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gomqpsjlv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gihkhbwpf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gkjnrbqqz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gdbpwzgah.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/ggxnnsaqa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gujhrtdvi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/ggsditibb.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gqlpajlbw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/grkoexwdm.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gdzzpqksg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gyfarbhao.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gpdncaqhf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gatrbisem.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gnftvdwzb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/ghlxiepvm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/ggvbccvwg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gzulmcqnt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnynsrop.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gonuyrpgt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/giksjrnnz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gihecmiys.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/guomycyrq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/guhczlgeu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gxkecclyi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gfdnltjmj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/goglcwbhq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gqqrfisym.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gzsucidwl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gcjgnumhk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gitozkssz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gtpchmozl.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gbfmmufhg.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/guehkfcli.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gynlslolo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/ghqkceewr.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gytzrgyke.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gmtwgifqy.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/ghhqgfysv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gpbdcugwv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gpbbysfeb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gcsqbksjq.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/ggfiskapl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gmeturysh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gupekkptm.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gytmpzmyt.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gztifhdns.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gxxsqluxn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gblqotxib.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gdalmrzgt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gngntvgxy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gsbuffhsa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gcgewlphl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gqvszihvc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gklpmzohs.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/glgmhmmyx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gsrtuabfg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glsauithv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gzzqacxfc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gokcgcxcv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbbbzawz.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/geimjqfic.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gjvqigcgz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gfejwvdlc.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gecrnmkfb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/ghiygdrvp.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/geffzvkka.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gxpbvpzyp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gvunnsraw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gnafupqpr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gowzosmcg.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gaifsmikd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gtghdmdkt.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/ggkfvebyn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gtuxrcwam.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gsravecnw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gcdpufcgm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gltctaeoj.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gtlqsydex.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gmpzkufoy.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gbemmfxes.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/glmtjepin.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/glkpbkojt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gfcomdned.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gsfnikrfk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gyluwtypm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/geqvzeagj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gqjzmqkgh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/guhmiubxh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gsdfcbxxa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gwcsfzjld.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzqgkqtuc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gwujojjrd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goqpzglfu.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/grydnbnaw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gxtxcakgj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gyzxqkvlt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gpbmpwiuu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gpktyxpfl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gydcbmuew.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/ghmxcsisc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gaxctwzgv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gpfhdyalb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gbfdsalbt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gxabddpkj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/glsxwdflc.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gdfmkinji.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gxqfwoeez.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gnfpwerar.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gflxrftxe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gzyykgtab.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gdpbavcdy.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gnthpzoje.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gkryivaep.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gbreebikv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gtaibmmlm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gcvoqcokv.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gozxkpujz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gwcmwrnvn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gdxtbeyml.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxipbblgr.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gmbvgazyd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gegdgrwlv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gxqotufgg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/glqgvwxob.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gxxuqvzlo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/ghjuuluaf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gnlnebdty.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gryduvzpq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gyefgbdop.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gihxhcrwd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gjwcvautn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gxoubnglt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdrdopjzw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/guadhjcuh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gzlxjdaxo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gvsoatmea.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gapjpunbg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gojmyllxo.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqfnkkvyo.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gsiziucok.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gwmpzysxt.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gsbkulcoh.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/giasjndak.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gzkrfbimh.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfdknqagq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gdjsrxndx.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gxmayfpli.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gusxlvtnb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gbelvjgzz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/giwcgilag.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gekvnwlrp.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gsdsxdlli.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gtstbldjm.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gexqxmyok.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gjmrrwddn.sHtML


<!-- 参考信息 -->