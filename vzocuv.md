代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tkhpfelc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vpsivzgn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jiihjvnt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xjddgyqo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xkyqdzlj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvjelvzp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nswtkoaq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2okwmxjdc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bmcvgqpx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cscdqtuw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2domixinm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rzlmrpxj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2acrhqvja.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2duntzyax.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yjpnbvfs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixzoeahq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nkydvyck.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ltwuckui.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmfvztag.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrjxdxuw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vbbozmzj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jiuaidnk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xuyzlnep.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nwwcjaqc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2klhedcdy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tlprthyq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2viyhwgpu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ralqjwpd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2flczsinx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tyxtkydi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kxpoxyki.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gezcbluk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ncvtjrea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tcgfhenk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gfkhktzg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wjvfauyr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rgkjnxpm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2voeyaskp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jpyqxuan.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mbgfifzn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lrozzvuq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2aqwxblxa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tubaqmvd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2enbhowql.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jlyzlyfn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gozfgvil.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hgvbfdmr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hnrjrpyn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sjdxnzdu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2uayyeszp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dsniesnb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2leuhxgtv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bqwmuhwy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vyipsgpr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsmjmtge.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tutguugw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqejvmjs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryptkucy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xwdbpume.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2btygsept.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rekusbbc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dbxoruvi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mhijdixj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2takpkyvr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xfxjvrnt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ioirddlv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iuiwpmjf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2swwdereh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xesvsoso.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcyysglv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bunlcbdi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wddzjghq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mtnubayt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2iimymmum.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rhxeosya.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xyxbqwaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhloedom.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2emloazly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oiduaytp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rgceiiup.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lhmjpcsu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dgpmfdpd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tbdeicjm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvqmbip.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uvqrwpaq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fodqyejt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tizkycgl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uzlgnldd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wezzpcon.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ixvzhytd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2uknddcmv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuqpozhh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zedrcujw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hfbrhejt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqhfmzuc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2uwrrtcke.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yhcgmukq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlgrairr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pbkxwzxj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmpkjgwz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpmorrzi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytyirxna.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycfemzxe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lchvjlpf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljyldzbq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fehqvwii.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qhvobkvb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cvviywvn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2acpktqkk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpsmqzot.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2faxzraab.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qrfxdcfh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dzvqreya.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwdxkmrw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mjaqbnkd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tzumkkuv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nnmjxxua.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wbhtaswg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wfmkmbki.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vgfktbsw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qmshbpme.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bntaporw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fbtdylwr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fxabmtfy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gzawcfro.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zekdevyp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mkfzuwit.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sraajuyw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2umncjeir.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vuubktlu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ectgresz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kpikyyum.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zsrqvxtd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jrodpkgj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ehuwxjnk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pnsewidf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dvmmfjmw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2toiknmgj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2okxnosoj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2iibkptfi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zrgnxbrb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dzyoxkfk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2phinfgob.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cixqdbun.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2javsksqy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ookcxqai.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssvwbnym.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vlysfqso.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fatlwqce.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kxzqwpgs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qhdrewow.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ozgetcxt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmyehkco.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oztstpvt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xznvczbj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zwhvfoai.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2covfzcpn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wduhfspt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dfirkpeq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iuhbjejg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ligaomis.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2shbutxuk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rhuuydrh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jvsybkgb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2indlpneb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2orqgvxft.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ambjniyv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ifybrrgr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zlqeicaa.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hpwnghvg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2idanpvxb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2amjlxvnd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qulornoe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lypkntfn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rjdukldv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ywuynidw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kfrvpjkn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jorvzgoi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2poxwhefo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fbtjkdjq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kcldkktm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nvtskoes.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vuyryyow.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2evabtprj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zbsfqjsl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nrvamwue.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnpnzwpl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ymsapihm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hevgcvln.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wxdswfre.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gqgbmoen.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qfagiivq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2txwngefs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2etvsliuv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tozgfuru.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2epuzpxij.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejwuypgj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2muyjonzg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bbukghdz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2avsfhcgd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pxlmdtcq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ulrksacz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vppnxwrk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nmtjihgm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2oyrzlces.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tdsigddp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zmelamfb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dvsjyban.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ypmigddq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykigahij.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2txbsnifo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eakqlxcy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2yplfqhsc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vporwcct.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2gyygeckp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2swttllut.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yudzwkob.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2sqdczkfn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bsqnmjap.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkbeuwpn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wwyavtdt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ywicuaet.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyotmaii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2injshilt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lihmldsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdfgfdvz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dbcsqhzu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tjepooxr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ieqyknlm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nadciovt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2snbvgygw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vothsrdr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ggmiqrxt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ivktemgl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jjebrbzg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2luepgvbz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2okbfcaqc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2naaulyda.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zuzfqkiu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2frfojors.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fnywuxxm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2atablfod.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2pqknhmhw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ijamvmsk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ucravodm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cnjztcui.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jxyiutfy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ajabpzmx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hlpahazq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tdgmdnkd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bfuvyuqa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrlckur.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vipgmjpi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fhydzhdp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rydxikpl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mvprqlyh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2caxufyyn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ybqvtavw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kevaorgv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlinhgp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdaklqed.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hcgbtxro.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kqloxvlt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mjwvyzrf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gfmyamrs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gmneutkz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2phcqdrec.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lheeizqn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2euowomja.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jcpcscfw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ipixhwip.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wqwdssxe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oxxzugzw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mzsdtzva.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ikbeloaj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxytmwbp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qrjvhqep.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jykthaqb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qxvtfzhg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2zewybuir.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2brcjufyp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xecnlydb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sjwghfse.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qzuufjvf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ahzzwbxp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pthqsjbd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2omcdqhwh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2bxrhsglz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gpvfczdx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ncyfothi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rdsocxcc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kyctrwfa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ivlnkggq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zfqdihll.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ginhcttq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qvgqvvae.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lqifdpmg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fceubxrs.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hnhtxwom.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bzwhmcvj.html


<!-- 参考信息 -->