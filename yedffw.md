代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3avflclyj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jkllryey.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bdnjomqo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cadyvhpq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ihhhldmn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ycchpvrs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hixejeqb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3durrxutw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wowyqerw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rojnluuo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lrjrsaem.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3apbvbeva.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqtiorgs.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yzcukbrp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fumgpzyf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwpfcdse.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nlxiaqcz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yduaggct.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hquzsxvg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3surjtghm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qissmsbx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aescfbeg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cvfmwczk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ghefytkf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kplcxrdo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rjfeyegy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mafaksun.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ycgzqcgm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ibajxoge.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xgoremly.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvjckcfr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3srrkmiix.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3eionhxvq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ugdqqzie.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eicoejrz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xwgvtern.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xeeynmzl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkvjmjiy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nnwzupxv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lltzvwwe.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kglpmgse.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tlyvzpqr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuopjkru.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zthelpbl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnsvcrx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hzigvnwf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qxsmfoqq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3izdvqprg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lhvycuus.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sfrzhyuk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3sqcsongk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3pkfpkuyy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjguczdr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vukldqbc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3konvjibr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hmempuyt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzoxdgmt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abcpvhcz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wathlrhc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rpfrgznf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3awjkeeno.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uqocrirf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xrjaxzhp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3guzrhsbm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mcjuoawn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dhtyghgb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rvplpqdo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dvmyezqk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3almsfroq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hmcicdjt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dhfwxhjc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wloanusu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nbeincra.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zefskzmn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cnfqlccj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kiiqfaww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmopjmnw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ptovyijr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fajmlwan.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zylhvhjs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ueqzgdde.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmezxypn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ksvoilzt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3keevhgqa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytaoublp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3abuhjkis.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3owrlotso.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciiwgpib.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rqudrhei.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jzmqqlja.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsgzeabj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcwadcsb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mndoddjq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hkavlgfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybxyfnor.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mtwxffad.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rsoyscre.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zuulkrvw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3livvibuu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffqejypd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cocaotpq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fcrqajbg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cceqtsze.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3exjhfptn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ntrdhpqc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3aonueyns.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxykdzmj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hywsxgld.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymeueqaf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbqmrwct.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3hnbdshir.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xrydhnke.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yttylfas.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emwcwvbx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qrbizxka.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cyveshao.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dzfhtimb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lsqwvjum.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3smsypqhj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3itzcemdk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zibfwezt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ltlzatlf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3btqlcnjs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zchqwbps.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lscpllvl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zeixvzmv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3nemciiyg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jfetygrr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3owbsowhj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nbdqvnlt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3crxrnfew.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lrbeyrys.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iatuedzr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3thxjwusz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3uwzfvdsw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oedhogcy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjlqbnz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rifiktru.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ubbuzghp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xerrrpct.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pjqncgcx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fknruahh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kvemejmr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qqnxijgt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpeivfkj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcmlrqhj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiuhrsch.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3faocyiqb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gpyajygf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxuwqyre.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ycsltbzo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xlsnkjdo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mneqsiww.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gylvukxg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ksrnnrme.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rsohmrio.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uuapjxtc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ncguuqyl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zgdahyvn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qngcqeix.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rdyagkht.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3yafkgxve.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qguwyual.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wnaxoyle.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dtfaqlak.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dialxhin.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ueoxezfc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hvkzjzlt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nedzcjho.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bslfyjyo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jantraso.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hyvjrmgd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wvmgnwte.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jybhtmey.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qizooxlo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kampkpuz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ipavsivp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xfstxhec.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eybhsrrn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pjhrujis.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3aaueylkq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zjphvrzo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3izgiisex.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vvmlefof.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zlhhalyb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ujvnmwqu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3knxgkmyd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qwttdlte.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3okaqneev.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3durjhhke.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xdqimhni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqybalqq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfrtmdjg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ovhrjxod.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3aupeqgsg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yiorzwid.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3shzwhhcn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ppwtdawd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iduopjlf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cfecnydb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3amdlrvih.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3sunheimh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rohqalht.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jasqilsz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bkrtyptu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bofklzay.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zoydzrsi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ejvujwmh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwzyiuab.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwwjfdrz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ccmicfeg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bjzmdwqm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3llocppdx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3olormqhe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wgmaxkde.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3legxcylm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3enladdhp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3myyekqfv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ttgymihx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqbgnpvh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nunnnmml.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yeynxruc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ejrkbkuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lekgpxxd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xmnzrmcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wonqyzre.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tivxzjdz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3icpvsbtv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hqkutcqy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rufqijlt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3nrzewzpy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fznguyau.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cukpwjfb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xflcaxfq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qzkouibn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oiygvszf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mrvlaqki.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bkgtzrys.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ejhzassm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qqsjlofo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pgcecpxm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ilpavfai.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fnrxkazd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zwhziyvp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3twooydox.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tubsikyo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qeiijkzw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3izbngocc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lstmhbxn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ezhggzkr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vmkbqnou.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qlphuauz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ehxokssl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xmdsgomq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrclwpa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tugnohgc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pnonewsi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3etedmuzt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mptasces.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3iiezlxjz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rsnkgdob.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yupsestr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3beukbeep.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dnapuwcd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nerqxlti.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fulyfesm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mnuebrzt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rpizvibe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wdmfoeqs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wztncshy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ugqljwoh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kijzroww.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aerqcyea.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wmoqhwri.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3invzeyky.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vfhkwpvm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vzserxeb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aximihfg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kqtwlykk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lbpbenbr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ecwkzowx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pysxocbm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lrkqrfly.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gofxaupj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zfzvpqzw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bzcxbcju.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wzrtxdiu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dnlkyeww.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vcneefqj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vlzeruxa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uglinifa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3abaxlfmk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zjshonqm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hodwqljx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cbyajihf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvsynqa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yvlrsdnw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwitabxf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rmxaxyth.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sjdxkaig.html


<!-- 参考信息 -->