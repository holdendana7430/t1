代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.smart0.xyz/gtsayaiogi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhaomingkeji.xyz/gtfifqalbs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cheryme.top/gtvjzzwtxn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nanxinkj.top/gtqmnwwqlq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangshuangyany.cn/gtkxfpnskg.html

[B06] 遍历字典 / 对象
来源：http://hz.birdmap.top/gtctbdxrbw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.dianchejie.cn/gtuiowzera.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gzhubu.top/gtcexggowo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gtswycdnps.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shanyushiyangkeji.top/gtgzjgbjwx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tanke756.top/gtgxhecukc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.svipenyu.cn/gtdulizqco.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zdqjudy.top/gtlsymytvu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jqgfzy.top/gtcjzgrton.html

[B07] while 循环
来源：http://hz.jinghuilouyu.cn/gtfsvbfbxc.html

Py:   while i < 10: i += 1
来源：http://hz.daria6918.cn/gtziwsfuhp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.wangshuangyany.cn/gtihxsbdux.html

JS:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtslvsrxvo.html

TS:   while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtkmmfnhdg.html

Java: while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtmtkpilzk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tian-w.cn/gtnawfivkm.html

Ruby: while i < 10; i += 1; end
来源：http://hz.redwolf501.top/gtxlxukfye.html

C#:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtvewvsidn.html

[B08] do-while（至少执行一次）
来源：http://hz.xinyue.icu/gtrhmwiyca.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenlongwang.top/gttivvwwuh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.andypj.xyz/gtnqhpwswz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gtzoycocgi.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtjanwcfib.html

Java: do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtcjtvilfy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhixingplan.top/gtwihzvxtc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenjidiqi.icu/gtxkosblhj.html

C#:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtrizskhiv.html

[B09] break 与 continue
来源：http://hz.bjfxy.top/gtudzjeykf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ybcxt.top/gtyfkygohd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gotoacloud.top/gtkfunugvm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtiaqzlwlc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.birdmap.top/gtqvuibkaf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtzhijqfwu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.sxryk.cn/gtvbfgmvvs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ehwqpu.com/gtyokekreh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtzmkhpqjv.html

[B10] 遍历同时拿索引
来源：http://hz.sysykeji.top/gtjniarwcx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yangfankeji.com/gtuxtbyymc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daxiang520.top/gtfestahqn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtzrmesknc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xuanzx.com/gtoxnlqfgw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hysaishi.cn/gtvehkkzmk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinqigufen.top/gtrmlkjubg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xinyue.icu/gttoukgshr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hammf.cn/gtbutclxgl.html

[B11] 生成数字序列 / 区间
来源：http://hz.gotoacloud.top/gtyupzfklv.html

Py:   list(range(0, 10, 2))
来源：http://hz.hnqzz.top/gtqmlzpsya.html

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtawqplkfp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtbadwzqwp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yangfankeji.com/gtqvbkvivt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtzunmyucj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.316326.xyz/gtrbfdjycf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gtgxldwaba.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shanyushiyangtech.top/gtdxkhrfqx.html

[B12] 跳出多层循环
来源：http://hz.sxryk.cn/gtawlqkqwc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hongshengwenyu.top/gtzhnfosln.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gzhubu.top/gtegmrxrdw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtyccczsro.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtxvbofgxe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtmcsqqsoa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tanke756.top/gtvduvdmla.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnxiangtu.top/gtffarvrpv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yanxiufei.cn/gtqnhlluga.html

[B13] 判断是否为数字
来源：http://hz.zhixingplan.top/gtlqgzrqex.html

Py:   isinstance(x, (int, float))
来源：http://hz.jianghu66.top/gtlyrayhmv.html

PHP:  is_numeric($x)
来源：http://hz.316326.xyz/gttiluqhbu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gtflamzeoi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtbirwsvza.html

Java: x instanceof Number
来源：http://hz.shuidangran.top/gtsthpjmjg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xingfuxueyuan.xyz/gtqoptlbre.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hysaishi.cn/gtnhmqsqrk.html

C#:   x is int or double or decimal
来源：http://hz.fengsongda.top/gtelwceewm.html

[B14] 判断值是否在集合内
来源：http://hz.52xcode.cn/gtdzithtpy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yonumen.top/gtworjqgsr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.c1oappe.top/gtmjkaxnig.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtasifxnvi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hammf.cn/gtfoewssos.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtdrzimerk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daria6918.cn/gtjxynkeeq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.wangdashe.top/gtwieatgkd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhijiandao.cn/gtsqibzkep.html

[B15] 布尔运算与取反
来源：http://hz.chenzaomai.com/gtypcdlgwx.html

Py:   a and b or not c
来源：http://hz.yj20258.top/gtpvyorumz.html

PHP:  $a && $b || !$c
来源：http://hz.guannengcc.top/gtzddibbex.html

JS:   a && b || !c
来源：http://hz.ivvv.top/gtzbzvpapc.html

TS:   a && b || !c
来源：http://hz.iojbl.cn/gtnueyshxl.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtizkeqrye.html

Go:   a && b || !c
来源：http://hz.0kj1m.cn/gtlujgkaza.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gtnoblwyzz.html

C#:   a && b || !c
来源：http://hz.jiagoushi.top/gtaleptyha.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.meibo888.top/gtaprawsoy.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtvvlmbgqu.html

PHP:  if (!$data) { return; }
来源：http://hz.vqdsnc.cn/gtmlxbnbgt.html

JS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtpkgbcukh.html

TS:   if (!data) return;
来源：http://hz.pycfn.com/gthnmyfwvl.html

Java: if (data == null) return;
来源：http://hz.xuanzx.com/gtjhvieqjj.html

Go:   if data == nil { return }
来源：http://hz.daria6918.cn/gtokdmmcto.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangtech.top/gtgkuasooa.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtvkklmmkt.html

================================================================================
来源：http://hz.jyoumei.cn/gtbjerixis.html

C. 函数与作用域
来源：http://hz.yanxiufei.cn/gtdyezemqt.html

================================================================================
来源：http://hz.ybcxt.top/gtmfibjcgp.html

[C01] 定义函数
来源：http://hz.yj202588.top/gtfwmisllb.html

Py:   def add(a, b): return a + b
来源：http://hz.yvedp.cn/gtsbithtth.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtxxyeghmi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtjvkvyyif.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtasbjsgeu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtsnkmnvzp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.c1oappe.top/gtoxiuaara.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinqigfzy.top/gtriybsbhb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtqmmijwkv.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gttshwecyq.html

Py:   def greet(name="World"): return name
来源：http://hz.yangfankeji.com/gtpxfblyyt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gttfotxvib.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtymemgfqj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenlongwang.top/gtryzxytds.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigufen.top/gttgtdqigo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtbeuacopk.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhiwuduotai.top/gtmwiunsbx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhoulong.xyz/gtxqbwwfmd.html

[C03] 可变参数
来源：http://hz.jqgufenzy.top/gtdqzmmvls.html

Py:   def total(*args): return sum(args)
来源：http://hz.cucudq.cn/gtjtcxxwlo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ydjk.org.cn/gtfapycusw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtqlbzmvrs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gtqvkzidqn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gaohongyu789.top/gttmwhikbr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shzxlz.cn/gtuvmoarpn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gtxxztiedp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guowangkeji.top/gtrcppwjnw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtwfisqmsd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gzhubu.top/gtmmgihufb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gtagwcdkjg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtpzuubjbj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jiagoushi.top/gthnztggvz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aibaodan.cn/gteoxafzux.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhiwuduotai.top/gtspdfpwbo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtlgeacowj.html

C#:   f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtwmcczwmh.html

[C05] 返回多个值
来源：http://hz.yonumen.top/gtbhrdoomt.html

Py:   return a, b
来源：http://hz.yangfankeji.com/gtmnwluiir.html

PHP:  return [$a, $b];
来源：http://hz.shuidangran.top/gtncblufcf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj20258888.top/gtijwzozxk.html

TS:   return { a, b };
来源：http://hz.fengsongda.top/gthxxynoio.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtazczuxlv.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtqlqbdxxb.html

Ruby: return a, b
来源：http://hz.andypj.xyz/gtjvloisei.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinyuanbaomall.cn/gtpqakgewv.html

[C06] 匿名函数 / lambda
来源：http://hz.yongpay.top/gthicgthxt.html

Py:   square = lambda x: x * x
来源：http://hz.havefunace.top/gtfddjbzcp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.quarkkingdee.top/gtjixhweeb.html

JS:   const square = x => x * x;
来源：http://hz.c1oappe.top/gthefzqzxb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jiagoushi.top/gtzodseath.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhijiandao.cn/gtahirlwsu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhengqikj.top/gtdfafzgwf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinghuilouyu.cn/gtigpdsxpx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj202588.top/gtwswjrlwi.html

[C07] 把函数作为参数传入
来源：http://hz.nwbrower.top/gtpxtggikw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinghuilouyu.cn/gtavtigpqc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj20258888.top/gtwkjfqxji.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yvedp.cn/gtdbonwuur.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtaaanxtzg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fzhhl.top/gtmyrykaih.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nanxuanxn.top/gtasmpfkun.html

Ruby: arr.map(&:upcase)
来源：http://hz.daxiang520.top/gtziodrmbd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gogol.net.cn/gtqoxbclgm.html

[C08] 闭包
来源：http://hz.ppjwa.cn/gtetesslzr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenjidiqi.icu/gtctfvhsjv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gticuzatdu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtazidjvjc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtqawbuluw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dianchejie.cn/gtmofkjjac.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xinyue.icu/gtrnadwdeh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.birdmap.top/gtygtyzxqm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtcxhrfqxg.html

[C09] 递归
来源：http://hz.hysaishi.cn/gttsbmkucd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.meibo888.top/gtbcakgenq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigufen.top/gtoibautep.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtwfxlgafd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtjugjubll.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dashuyun.cn/gtncnxvmrb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinyuanbaomall.cn/gtaxkbjqvv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.mhx1999.top/gtqfngiure.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sysykeji.top/gttybqzoxx.html

[C10] 变量作用域
来源：http://hz.hnxiangtu.top/gtxpglsdha.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhengqikj.top/gtwjhzeouk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydjk.org.cn/gtltfnbttu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yanxiufei.cn/gtvttbxpar.html

TS:   同 JS
来源：http://hz.zycfv.cn/gtleiztwmg.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtoqrbuahv.html

Go:   花括号块级作用域
来源：http://hz.xuanzx.com/gtpqqbqzrn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hywenlv.cn/gtxserwpuf.html

C#:   块级作用域
来源：http://hz.pycfn.com/gtoeixduns.html

[C11] 模块导入与导出
来源：http://hz.birdmap.top/gtpvfnrpll.html

Py:   from module import func
来源：http://hz.jqgufenzy.top/gtpcxnbntl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.svipenyu.cn/gtnvvccepj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hysaishi.cn/gtvoriukqf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigufen.top/gtynqclnzr.html

Java: import java.util.List;
来源：http://hz.ehwqpu.com/gtvwjzhoyj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sxryk.cn/gtajopttsu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aibaodan.cn/gtcyyobakd.html

C#:   using System.Text;
来源：http://hz.9152youxi.cn/gtdcyjmytq.html

[C12] 立即执行函数 IIFE
来源：http://hz.yongpay.top/gttrwzamor.html

Py:   (lambda: print("run"))()
来源：http://hz.jlsjyb.cn/gtxgowluhf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fzhhl.top/gtkubkbpds.html

JS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gttigzzdkh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtqrtklcmv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guannengcc.top/gtdbijvhnc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtjpoeruna.html

Ruby: -> { puts "run" }.call
来源：http://hz.zdqjudy.top/gtoxongbyq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ybcxt.top/gtisdtpphy.html

[C13] 类型声明 / 类型注解
来源：http://hz.dianchejie.cn/gthubkpeuc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gotoacloud.top/gtjnsnmhia.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtcyebcpnm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtgyaooywz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtgvagmgpq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtbsoxggrp.html

Go:   func add(a, b int) int
来源：http://hz.cdnleiting.top/gtqabzxear.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gteiiwznkf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydjk.org.cn/gtvpgiyvhq.html

[C14] 泛型函数
来源：http://hz.jqgfzy.top/gtwrxiavie.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nwbrower.top/gtykklomym.html

PHP:  // 无泛型
来源：http://hz.zhiwuduotai.top/gtejmvhizm.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtubozbugk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtojbdjtdj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.redwolf501.top/gtzupzgqqc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gtxeishvib.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtctcombif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gtbzpjkowd.html

[C15] 解构 / 展开参数
来源：http://hz.0kj1m.cn/gtlwimlsus.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yueranfly.top/gtwofilkdk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.c1oappe.top/gtjzisluuz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xingfuxueyuan.xyz/gtwdijgobd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtopsieaao.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtxicmmkli.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gtpetuvdlg.html

Ruby: a, b = pair
来源：http://hz.gotoacloud.top/gtropikozc.html

C#:   var (a, b) = pair;
来源：http://hz.zhixingplan.top/gtklalvurf.html

[C16] 函数 / 方法重载
来源：http://hz.aibaodan.cn/gtzrivcejf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tianlin.xyz/gtddbsocbq.html

PHP:  // 无重载
来源：http://hz.iojbl.cn/gtqthotfcb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fzhhl.top/gtqcwsybbh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtauyladpf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dashuyun.cn/gttzttsrip.html

Go:   // 无重载：用不同函数名
来源：http://hz.tian-w.cn/gtladulncy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigfzy.top/gtlmcmolss.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xingfuxueyuan.xyz/gthszejwct.html

================================================================================
来源：http://hz.havefunace.top/gtaysornnt.html

D. 数组 / 列表 / 集合
来源：http://hz.zhixingplan.top/gteiwvrurn.html

================================================================================
来源：http://hz.yongpay.top/gtsrlquxag.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtkcduzuxc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtobwgbdkk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinghuilouyu.cn/gtyzdotziq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtoexufndj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinqigufen.top/gtyqoxibqz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gttpwbrymw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhoulong.xyz/gtazmhronq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtxinzqkbc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.9152youxi.cn/gtnlnihsec.html

[D02] 追加元素到末尾
来源：http://hz.ivvv.top/gtnkhpiucd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.mhx1999.top/gthkeekyih.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtcyeoqjgs.html

JS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtegvxaaho.html

TS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gteihpjllb.html

Java: list.add(4);
来源：http://hz.jqgufenzy.top/gtoufknlvk.html

Go:   arr = append(arr, 4)
来源：http://hz.haohaochexian.top/gtgjvfdihl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jyoumei.cn/gtqtrrzsnj.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gthuadgmgf.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtgdpxatnx.html

Py:   arr.insert(0, 0)
来源：http://hz.chenjidiqi.icu/gtvjdyswbc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtbqpnimkj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sweek.top/gtqjlgjmyz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj202588.top/gtozxoqpxy.html

Java: list.add(0, 0);
来源：http://hz.yonumen.top/gtpeuttsmz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.9152youxi.cn/gtwvsekjjx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jyoumei.cn/gtgupmtyxe.html

C#:   list.Insert(0, 0);
来源：http://hz.cheryme.top/gtewmdhsmq.html

[D04] 删除元素
来源：http://hz.yj20258888.top/gtkmsmdugc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.bjfxy.top/gtawieqrzh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtbgerkuov.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuetiantiany.cn/gtzobamvdc.html

TS:   arr.splice(0, 1);
来源：http://hz.daxiang520.top/gtykpdkguq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shanyushiyangkeji.top/gtimoipiaz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gtsxqhfogd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhoulong.xyz/gtxiixzoyz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtbohkhsrm.html

[D05] 访问与修改元素
来源：http://hz.chenzaomai.com/gtdkklfrxe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtndmfjimq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtuhwmnxgg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtaeymgftk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yuanzhike.top/gtalwhhutp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgfzy.top/gtpwfjeohf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtuprejmnz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtbsecxdou.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ppjwa.cn/gthhdzmavd.html

[D06] 数组长度
来源：http://hz.9152youxi.cn/gtkrcpkjae.html


<!-- 参考信息 -->