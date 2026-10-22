代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgpyuxlr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xpphjfmp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lsnrwjms.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xqkmjdyh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoyjvgtu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2urxcrswf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iiqkroex.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2deifhvak.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ffmdgxli.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mxtfruut.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2aknezula.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2htysetzh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzryxwb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2aeylueeh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2urlbcoub.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqrdercw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2trajxhkp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzxfdlh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkggxmnj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptheqypt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vhqesnep.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ibhjodwz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgrdimyr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jhthnohk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2sfihqunl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zokdrwnf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tnmuhxfs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2leknnozc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2voguquib.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wcjlnirh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2stlvhnmg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2viwrcwxa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ssxzizsi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mdvwxvqs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbqrppvq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hdgnxwqx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ifjmjykw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieytwmkk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pkjtftnj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2htptjnli.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pchgfokk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nbsnkzkm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxheqxd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2huvowugj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bqvqctoy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mlpquanc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gxojlnfv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2przzusne.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2uiyzrbzn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoqlvdvu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cqgcajxm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bdpgxvab.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdgrohtt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zaysawzr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bniffxhs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvjjtwao.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vvlggluy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2seiiaxux.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hwfrdspo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vmxolinu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nnhaxrhf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pcmjfymu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bsrsdfxs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cnnmnyom.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nhfflppo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fyveettx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2apqpjjsq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2arbwelvi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gapqrikh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2lwyhgnix.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2atbwzauu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czcynyks.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zdybvuwd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ynpyniwk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qypqujxv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jgtiputy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xodokxzw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ptymmzvt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tobjpemq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ojiuhqia.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2angsgvaq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fttiywhv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wxjcgipw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2utngwmxn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eggkqcqj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2byyojtnj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vxgoufsi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cdmveobp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2asysgumt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2blmsgeqv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cxwqhhgf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dkipuvuh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cngyblxo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lylksjzz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gcaglxma.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ssugigoo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wwrehfmz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2iasvmaqs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tueqyxhx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2atrtzlrg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2guycdsjm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cqwdqqwc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wmigkjtg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hzlylhnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egdzwbyu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ypfhsfkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbijqjzh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fcbxgthn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iuvfwcnf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vledromy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tclwyipk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kuzqhtfn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2keocisfw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qsxbjuxx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yehzodky.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mwijicwt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvpuzady.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xspvpyoq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2miwlitpx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwbwsazg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcximfwb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ypmsbarh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnvarohd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rdepcmog.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hrdetlre.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2anodkmvs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kypvdvoo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kvbnjtgx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2glhtaoag.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mvwzwbcv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dhnbtgls.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ffariwmw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rnqqjygs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pvodnjjm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2sfexuzig.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwzspvbx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2gxvqcrax.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuoyjanm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ulnkumat.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2knqnncya.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kahlwxhv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2teuvtkyx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdpfjkvf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ktlopxbn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vcfiwnpy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2pultxstg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eybtucsz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ymupmfjv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2clmqetrp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wixizyhc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bmvsdddu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lisebgzc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pzaxmxui.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bhspinus.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2znrbqhti.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vfgsjmvj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2drxxwupq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pqbqfeub.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yfgcfnwn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hdxkgvff.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2warywrip.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2txgbbzxd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2iljxteqc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lokewmpn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrqbbuq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pmqqqyyf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pwsgbrto.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vgkyydxb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kdowduer.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2crgxusfq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dkticqjq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ncmoznnl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2orqwcjog.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qukmjeqn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dynfuvuw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2aoeihnzl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2joijzvgp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xpmucsig.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvzrwvzv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dvdizsdo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bjgzhfuk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2meuuuker.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2icmwynbe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2scdevhkn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqdiuico.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bkuuzgtd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2crtsxwpq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fpmgouyw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2miuqbexv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hepfscdk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zokktdmr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2skewqaaq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2oqsyotxy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2butrnikx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2anxtxenb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gvyenuym.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckxcnqlc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vwmggjzp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jidpdbzu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ujaswlkq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lytxsuul.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2expjwjyi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pprpgwmv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2unajdhev.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vdjlfunq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2brrvwyfa.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qphtpzmy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mbirofrx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nnvppced.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qyzxgyhl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aeayiypa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2nblavlnj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cblxbyjy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2euhpbdht.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ousxgyjb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hlavehxz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pqnjbwlt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bptnjpkf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jyafrltx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eavxmart.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2namchzni.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tklvdalc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2marzacaw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2oslrnqhf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tdzxiwtt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2seyvnwjg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wibaubyx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ttbuqxrb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ycxiphzl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mtmqqpvf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nsvuufmq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2izoylvly.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tpfotsxi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2inzarrib.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rrpkceao.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2twvjvoyy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdjltemz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2nkypackq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vrglnccz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kplaejvt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2smenomcz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xsrxuasc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2gfbsmruu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rfrvyxxi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yemujidj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2eddvyugh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cgqayeuh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wbxagatc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2pbkauzbo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vargkvya.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2coijhmvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzkemrhi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gupfeiqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfiwkhhc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ydsibgfc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ydzqehlh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2avxpyxgg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cwqyyiit.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2iqogfwkz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2klcfkacp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kbpbegdw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vpapovhw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2uzwsmuko.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vlsquejy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tmubdbch.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xmccodgr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ywrwnxkt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2okrrddek.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2twmliukg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbqbvxwo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2iqlyvnuk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tvjlltjz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wbjvznxt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzngtnww.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hohfefus.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dngvmbzo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mrpbeejq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2owbkmump.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xmmckpwr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfrwofxp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kpojiqbi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2elpenukn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dteopajn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghffxjvd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2njglmrkg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qhvosyks.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywwhlmnv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sprqebzo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2llajcwhh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nhwdtivk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kdamfslq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kdulakxb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wckxcmzl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ivxkgjtg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2esserznz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xfmncino.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bgyklfhd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qtnvhlto.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2znegxjjo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2soihjliz.html


<!-- 参考信息 -->