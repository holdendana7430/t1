代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xirxmnca.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vuzisemr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ebwffqub.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jsfykvtb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2shsvbzhl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2iplswbyt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yamtaclj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tczzzgbr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxponnyh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cabiitut.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yqahcuxy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjfjfpyc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2etcvtrpv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2aubxgcxi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hxiefkmi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hguxeqym.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oskuabti.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lkvndfmd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bknnvzcn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wkkmuswc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rjertueg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xiuyhwgb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zsywwwms.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yipdhuyk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vonjbmtv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2brdnxgmv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sazhegxu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hdetbhmu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wqiribve.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lmwmispc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2cyclcnwf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gurqtmok.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uaebyupc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2iuddblta.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oiozbsuy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hoomoabq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bxgzwnwk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2kwtpvkkf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pirosufz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2porxnlkx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2spzjrquu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xaztkhej.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ykgjhale.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dyedauea.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fcyrtjgp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eturbloh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bwmbcxah.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2uabiorqe.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2khjzasrq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hucaaaqn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2pckrshdb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rycplcyc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mpwccllm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2foerwheq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohkwmoxp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdwfvpba.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ausifvzp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rakruusc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bxrectpb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bymhlcsp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pudkjmba.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bkrlybnd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cudbcjmk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lqgwudtw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nnykhwup.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bhqkafcf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rfmzqlei.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mkuujxnw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ppzrgwot.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfvmwzei.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jatpuyds.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ksdlrfak.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dymucvdm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2znugowxd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fzowpbky.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ldrqfhsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tknjdfdd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uflkzczh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omposbtu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2todqrulc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2olwfmtgu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejuinhkj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yynwhsld.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhhlbaxb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aummtjug.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2enwyvbvh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mnjardec.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2czftdtve.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oysniewb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2eejpmwgx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnphjaj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srmnwtau.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hohfqyrt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ixqvabqv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gnqfrgao.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tglfxhpq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qajikxfd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2quzaqqyg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tjdyhetp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyjhwrtm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyulzrip.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2blbbbitb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2sturudim.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dgffkoiz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dzjuskau.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gaqimklc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rtohuvdt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2glhkkwrm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzzvfbae.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsjnwzvs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kdrvycgw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kdtztfun.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2csvivltk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hkudizka.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pudczjdq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hxdatpra.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jeudlztq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2dftiwmbi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pablsdtd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tkvuerwp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2giyaqnbo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lgzovlpy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nvoshtmw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wjyorquu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2evfqmkko.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2lkgrxhzf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xfvaqfid.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nonxvhap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pplyfyha.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2mkewagsh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qxjhntlu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2alqnlurp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ecetzokp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2shkojqid.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2kongdiey.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hvlzvoob.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zybpdpoh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2twvrctrw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ydhxbpfw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gjalyhpi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yiujotlk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2eelcrffp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2favudlmn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hymwqpbx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2khstcsva.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lfdaraij.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iovwbeie.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ybiepxet.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wqzscsnw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gruwnrif.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sokxhgmu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lcqlluut.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tzfqrlkj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mxdohvnn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zgpsshuh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2orcqcjks.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2veymoahp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwnqbemn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2npbfsbcm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kicsengm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kpzarzmp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fcrwlxdw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zgwuamwh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lrlnflbx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bhafgmfl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rmcvyfab.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fpjivxti.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ocigfevn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gcclqisj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cwzoonsr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rbkrdvot.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dkltuemh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2maeejpjo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cqlhxrdm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2eelcpoyt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2sjehxtea.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lwueuehz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vdjaykjt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lzojrgrx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yshsbbef.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qrhfjemi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bgoctcjj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2esxidlrh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kswhmenx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jtzkvysj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qkwefpyw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hxqbqyjf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kwaoksek.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bzybdqsv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnqnrqvh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2upifgvhn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2odheigqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yqffuzqt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pjagajbs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fdhilhpk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qlvkqvjh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uvqutwok.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mfikfehv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yrujyfom.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sdgbwppk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqmzewwp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2axyqjibr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hzyobogr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uxtsjhia.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ifthpyaj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qigzeusr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2adcgvlrr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2oytnuoxc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynvxmkqe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lcdwjcyg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jdkqrngb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rmmbgumm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2odnsptlo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vpbebena.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2aqvkryei.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ymfcdanq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2flkiyjbj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nemchioc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ozrcitkx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hpsjdhps.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kyimoxmy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lvdmsqrl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2sutirgqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkerbpsj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kduihpwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jremzjuv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wjssnxos.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fnawzfht.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2afkebtiz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gizutitm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qnsdzjqs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2atbrboqu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2edcwcczt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2khqobzlo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ilrcgpqy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wqrccbtt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iffdspxs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jzuececi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yiiqobsw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lntudayj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lqbgkyax.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nzgntwmg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cslejjam.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2drzbrxsp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2eczlxevv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrnwpgj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxxdkgui.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wzxwunkr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hqfpjfow.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dfeuvodv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qxxyciyc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gpnyilvt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tmeaoden.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajsfdolh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mownuper.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aaczvvvb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2toozhrar.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hwbjyooc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2blkmbhqn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2frfwafrb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2djmxgjpz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fywyootb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2paycfdrz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kfiqraty.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hsbqoyfh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2glqawnbs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fyvlaqry.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ruufzsmo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bwensoro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yqfwnuuz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dzofilta.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pyzbhlhd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2egaroibj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yehbekvb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tmzysszn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pfdifppl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ueajhdpd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2csjfxwax.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qhxzvdev.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gtfwjunz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2isrgydih.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rtmpmlce.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqczveyd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zucsywlg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qvqzjdaq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wiyqhplc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lfqrwjjm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2opmioujp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zsentzlp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ychazdei.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2eqnqxsto.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nhelqzjf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cbtydtqa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fjvdcdfr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2twrquczs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hxtkprfz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fdnbqbvi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ytxqfbzk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cpfslxok.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kupjiprf.html


<!-- 参考信息 -->