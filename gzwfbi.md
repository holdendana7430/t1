代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dvdpugng.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3pmdikfxc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wrnershb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3chslvofd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dxpsczkx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhctqufn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aujtvtqv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hakinlkx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3cckgawhz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kgicwtra.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pflkonnx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3idfrkver.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qrnlkrgr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ftoywmeb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vscdiqum.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbmjqwqq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmyrlrcw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3olfgdxal.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ccasmrko.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3sgrgoxvx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nwuoxslw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rzsafpbd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gtxewqwr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqrkdjia.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffeoyrcp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsregnmy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kgmqzbkh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wmjviofp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rinvtqaf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnvwdwur.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hpjbfgrv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3athmpxsy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eftyecoj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cngiiivf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jndrwhyj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxjpudf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3opmsnxqi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3uppnnufy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eagimhvr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wiorzrvs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rwcnhmbf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3odephsoz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ugccjetn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pgnikzhe.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vzjlzxjr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jacqtcos.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3byezxske.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3faaxzzdj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3rgncqhwl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zvqnakcj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqtafulc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3paniczmy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnnksdn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ycjabera.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3exdpfpef.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3epkfszeq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdoqtjex.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3frycsmof.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uoivkztn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvgtzjmn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lckrpdiq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iqaylkqr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyfifpz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdduegxg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3sqgevgaq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jgigatap.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zzbcfxfq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3oalvjjzj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fvaatyso.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rpjwzyfe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uxtyzssp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3weemybmp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3roxtajzw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bbcldyos.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wihgnoyi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3teybepgo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jmzitaxr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3uvbsioxj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cscsgoue.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qmwuukuw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gorryuok.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yjvzugwc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3izyjuhde.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bpbhmkbd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qvakreuc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tzjmlnoi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ziihzhne.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdoqrlac.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nenthnjp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3judbplva.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hxhwqmze.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3iaanaolh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hzytirqt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrmuxo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zezmqkuf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ntumuifu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cigflwff.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qscbaocb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nsagsjab.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gbomxrsy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvvflta.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cubbtaer.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lusdkyya.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qokopggf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3axtevujr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tyyjwpou.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zwjwowgx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3whmantfc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gnvfclns.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xmwsiodg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jiwyarpq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hozllkkg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bmotphen.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppzxioyd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vskmgtnm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wvpropmt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3idsmwjcd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gyrhkjkd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pftlnqme.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wcehlrcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdpxeiia.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pikywaqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnnmvasq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qwzzihvt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kkwptigw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kyzsdcup.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mcvrdlgw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rcwhusku.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3afqtityx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gwbzwoip.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ahxvoyzc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ivncxbov.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ozbhhavb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ofouitye.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxagfhho.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dbyaftiq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhvrubnu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hetajgej.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jndcbnyk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kmcqdkfv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3eqqsztvi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3oksexzau.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3malusdzu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfwoldjv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ghidmxrc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tszrbkzw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3efyuirpf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xkrxcsmk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3axnrhkno.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zqwmfxfa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3iyghksnm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxoraxl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3twxbuuds.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3basqvzyo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oxwlzhlu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bykemily.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3djwxramo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bhpkbdro.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qiwlvuvd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3scrbcfns.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zkvgffxh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kagpjyol.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gdydfysy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qnvmcrri.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3panlzizk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qhztyaoj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bojgwnbh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qrsrxhfw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3aricasec.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3zvzxxqac.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zmmytvbb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gsrcrfua.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wlyrsqwt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ckcopfrw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nbkljdid.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dtmxgfup.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oucekjia.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vxomnqki.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nculrilo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kgzkhzym.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hriswage.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xrkttmpf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3peebcoxb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ynprmgtl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ojfjanri.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tlbyybae.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3douzrjhx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wgnbwcmb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkpejelo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnlfrfg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gcauelzz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zcfvswab.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3umuppblw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nypassfb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqzcjfne.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3leysxqcm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vbcghsri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3azgdqbyh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gsohjfyp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yviijvvi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nutttakg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3buxasmzb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmzctach.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3lxijblpi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mfiqaond.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xxwnozua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cohmdmvt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3virlvloa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3farwbwvp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3julzurky.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ztpfermu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3asqeouxs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hxoairbq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3trsvjlza.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ctbkxmra.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gkwtalsh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cgdqfken.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qvjwztlb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3daqipwcf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3efkzkeke.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3etvbedqo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3pubgpbyi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3veozwvgb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sjupblbt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ijfgkkbw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3drirrqag.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3weoqnnzx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pxeglrnj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bfvevfqv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vgcfxenr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3johfdcum.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oufcezth.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jsqsenyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwjggzvn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uosksfve.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmpbbiah.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqajler.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cegpbpnf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3blrwbkcs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hrsptqrm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xhuxbfso.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tjpmybai.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wnyldznk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tjmajjde.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cvyazdqr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ovhhmlud.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wineutjt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jmwhrpks.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3zyxqmggg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fukaypwk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kycofgpd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3htzeylrl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lfeynhzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jieurssn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pvrpzspq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ykdnktqh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pabcjdle.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gtdracml.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qqgofbua.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hzuxyxto.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ealarpcc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cguwqzzx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zftatuta.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkqagohy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3iqznewou.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3thizvcbo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dzattddc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzplvdop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dzzhqorq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eydyguge.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hwrgenej.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3laktthlx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3guimfgqq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hecjbthw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3koilecen.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3opubnmgr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wsbmuucu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xsvmdpni.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yozmsxfn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3twgchqrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ljhyfblp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3udqefgcd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kjpysces.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lrhiuqgh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3emeaqeqr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nbcjdizl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzdzgcp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gqdcuxjf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ahpadmix.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fvtanevu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqqugewf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3iliheaes.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rzpzctka.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nvxxzlwu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gapwpodf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ndwsqbve.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ipptmnch.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ihdcmqqv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iowsmfdd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ngwrbgnh.html


<!-- 参考信息 -->