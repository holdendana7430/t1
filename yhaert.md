代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ybcxt.top/gtxqnrdpxa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hysaishi.cn/gtmqcaqyvu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.snrcjt.cn/gtswipvtmp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sxryk.cn/gtbwtjkqoo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.quarkkingdee.top/gtyoxhhobg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hnxiangtu.top/gtxdfgdjmm.html

[B07] while 循环
来源：http://hz.shanyushiyangtech.top/gtixrcpymi.html

Py:   while i < 10: i += 1
来源：http://hz.hongshengwenyu.top/gtbxomfgfb.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yj20258.top/gtpvircfiq.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtqbqlutss.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtycslagny.html

Java: while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gtezltefam.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daxiang520.top/gtrcacdocd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yongpay.top/gtaxledbxn.html

C#:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtlfhvaqwn.html

[B08] do-while（至少执行一次）
来源：http://hz.chenlongwang.top/gtggfuawsm.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhongyouzk.top/gtdoqvxkjs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sufxvd.cn/gtpkqqbknt.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtkpowtqmy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtdvirxiie.html

Java: do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtlrjivzhs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yanxiufei.cn/gtcgirijgb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hfpthk.cn/gtyadhuusm.html

C#:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtrmrahjem.html

[B09] break 与 continue
来源：http://hz.ywan-chungtsiang.top/gteicznapb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.snrcjt.cn/gtdnxigvcn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.pycfn.com/gtqtqmarfu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtlbrmpmzp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtjjswawuk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtftadfxpc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shanyushiyangtech.top/gtlmkkbgkb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.guowangkeji.top/gtcylcwofq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtwpeezcki.html

[B10] 遍历同时拿索引
来源：http://hz.snrcjt.cn/gtlcffulnf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinqigufen.top/gtooftqyli.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ydjk.org.cn/gtbxqsgpas.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhaomingkeji.xyz/gtpwaujoav.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yangfankeji.com/gtxpcfdhqq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xinyue.icu/gtntmvcjzm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cucudq.cn/gtxegrupoj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hysaishi.cn/gtviaxttjn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nanxinkj.top/gtuahwsnhu.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenzaomai.com/gtswvhlfvh.html

Py:   list(range(0, 10, 2))
来源：http://hz.mhx1999.top/gtayuigpnh.html

PHP:  range(0, 10, 2);
来源：http://hz.jyoumei.cn/gtravrppjy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtjkwfoyda.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj20258888.top/gtzjgwhwve.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.birdmap.top/gtvsqlkvei.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fengsongda.top/gtuxsnlogo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hnxiangtu.top/gtrhfmalli.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.52xcode.cn/gtqyzfnqqd.html

[B12] 跳出多层循环
来源：http://hz.jianghu66.top/gtejbmjhto.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinyuanbaomall.cn/gtdlupgzxk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.c1oappe.top/gtmvyactdu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yongpay.top/gtqdeuhohi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtcgepgrlz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtorxqqrlf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gzhubu.top/gtsqetoeif.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yuanzhike.top/gtcjxxfqvk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cucudq.cn/gthyowxicc.html

[B13] 判断是否为数字
来源：http://hz.xuanzx.com/gtarxwubns.html

Py:   isinstance(x, (int, float))
来源：http://hz.sweek.top/gtlhhjvygy.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gtilajngln.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtcvnfulpn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtzjnwpqmp.html

Java: x instanceof Number
来源：http://hz.xylfe.cn/gtlfotxxmb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cqqwz.cn/gtuawicvnl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yanxiufei.cn/gtbtwurgfq.html

C#:   x is int or double or decimal
来源：http://hz.andypj.xyz/gtohdqakwi.html

[B14] 判断值是否在集合内
来源：http://hz.52xcode.cn/gtecqrdlza.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gtnzslkyrz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hfpthk.cn/gtgarmddzz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtnlhxnzvk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ppjwa.cn/gtmrbtvoyn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ydzc1.top/gtjbrihpkq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinghuilouyu.cn/gtshkaqeko.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cheryme.top/gthcurbasi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.svipenyu.cn/gtbmadwwhg.html

[B15] 布尔运算与取反
来源：http://hz.gaohongyu789.top/gtnxctmxps.html

Py:   a and b or not c
来源：http://hz.andypj.xyz/gtmiwkywcp.html

PHP:  $a && $b || !$c
来源：http://hz.hnxiangtu.top/gttjlkxtcq.html

JS:   a && b || !c
来源：http://hz.quarkkingdee.top/gtlkprubcb.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtpdquixfx.html

Java: a && b || !c
来源：http://hz.ybcxt.top/gtdqsemehp.html

Go:   a && b || !c
来源：http://hz.yangfankeji.com/gtjogaxkby.html

Ruby: a && b || !c
来源：http://hz.zdqjudy.top/gtgdaodpch.html

C#:   a && b || !c
来源：http://hz.shzxlz.cn/gtitsfqcrk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigufen.top/gtcynzrvcq.html

Py:   if not data: return
来源：http://hz.dianchejie.cn/gtcaqmaczv.html

PHP:  if (!$data) { return; }
来源：http://hz.0kj1m.cn/gtedpcjtcq.html

JS:   if (!data) return;
来源：http://hz.yuanzhike.top/gtziijjvge.html

TS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gtlgaxhwfm.html

Java: if (data == null) return;
来源：http://hz.zycfv.cn/gtbtfjrbtf.html

Go:   if data == nil { return }
来源：http://hz.nanxuanxn.top/gtxgyrqegv.html

Ruby: return if data.nil?
来源：http://hz.havefunace.top/gtqyckahjt.html

C#:   if (data == null) return;
来源：http://hz.tian-w.cn/gtycscriay.html

================================================================================
来源：http://hz.yvedp.cn/gtptdjpsjt.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtjoqfrrtu.html

================================================================================
来源：http://hz.tanke756.top/gtlnljvmox.html

[C01] 定义函数
来源：http://hz.guannengcc.top/gtzbldfzii.html

Py:   def add(a, b): return a + b
来源：http://hz.ydzc1.top/gtvxyeeeiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtaewfsscp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.svipenyu.cn/gtmaitvhrz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gthbkeppqv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gteklbfipa.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.9152youxi.cn/gtkmmavzqb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.feifeiyinyue.top/gtuulgbjpu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtrqzpznur.html

[C02] 默认参数
来源：http://hz.zhengqikj.top/gttsxbtzpz.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtmxtvpwjy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hongshengwenyu.top/gtqoxwuqog.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtwavplkmk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ybcxt.top/gtrbccqyqz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtjkfaqapb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aizwys.cn/gtvxsmhkhv.html

Ruby: def greet(name = "World") = name
来源：http://hz.haohaochexian.top/gtrgbkmspv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtfnlvwjmp.html

[C03] 可变参数
来源：http://hz.zhengqikj.top/gtozwygybq.html

Py:   def total(*args): return sum(args)
来源：http://hz.nanxuanxn.top/gtauevantk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnqzz.top/gtjodvvmmz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtbzolapku.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gtqnsoyulg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.redwolf501.top/gtmoofcckp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zycfv.cn/gtyyqfkhlz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gotoacloud.top/gtntkbrada.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhaomingkeji.xyz/gtxarlppns.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yueranfly.top/gtccbckwns.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hywenlv.cn/gtjtbgifah.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtbowfbmbi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtwniyfeml.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhaomingkeji.xyz/gtykrbjxpn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.dianchejie.cn/gtvfbgvbxb.html

Go:   // 无：用配置结构体参数
来源：http://hz.wangshuangyany.cn/gtwlvazvek.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtzenzjdbd.html

C#:   f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtxwstnszf.html

[C05] 返回多个值
来源：http://hz.c1oappe.top/gtmujepfkj.html

Py:   return a, b
来源：http://hz.snrcjt.cn/gteavhjyve.html

PHP:  return [$a, $b];
来源：http://hz.bjfxy.top/gtnillkufk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cdnleiting.top/gtfgwenjhy.html

TS:   return { a, b };
来源：http://hz.zhijiandao.cn/gthfdzkxxr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuetiantiany.cn/gtcrrshnrj.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtntbseenx.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gtmlbjzljj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangdashe.top/gtpcnslbns.html

[C06] 匿名函数 / lambda
来源：http://hz.chenjidiqi.icu/gtduepmxdo.html

Py:   square = lambda x: x * x
来源：http://hz.svipenyu.cn/gtutppeqfv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gaohongyu789.top/gtlwcjwngk.html

JS:   const square = x => x * x;
来源：http://hz.9152youxi.cn/gtxjkzqlwi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.vqdsnc.cn/gtokuibjlb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tanke756.top/gttvpzxycv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhixingplan.top/gtsnrzdqtj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhixingplan.top/gtvexntitb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydzc1.top/gttreqjmeb.html

[C07] 把函数作为参数传入
来源：http://hz.sxryk.cn/gtymvaoeqk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jianghu66.top/gtozjgcajo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haohaochexian.top/gtugwhiopa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtzjvtqavd.html

TS:   arr.map(String)
来源：http://hz.yueranfly.top/gtlxswjvso.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yueranfly.top/gtflhcwdjv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hywenlv.cn/gtkofocunr.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258.top/gtvadztwkf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.havefunace.top/gtcqcfvzpi.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtikpqzlam.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.redwolf501.top/gtfdykaagr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhaomingkeji.xyz/gtifukpaci.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtjdmabfwo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtaganyjyp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gtkrqlpzcj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ywan-chungtsiang.top/gtmakhhgxg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhixingplan.top/gtmrkyawot.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gtplmhecdd.html

[C09] 递归
来源：http://hz.mhx1999.top/gtdrvnerze.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtbnhcksqa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gzhubu.top/gtheabcvxb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigfzy.top/gtdmfltcps.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gtqtximqet.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.vqdsnc.cn/gtyucfmlzv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gtwrssuvxz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtuxufdhdm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.bjfxy.top/gtxmrenzpo.html

[C10] 变量作用域
来源：http://hz.ppjwa.cn/gtocptsdxp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ywan-chungtsiang.top/gtnsmxtqre.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gtmjfidzix.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtxptmulku.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtjozxaswk.html

Java: 方法内为块级作用域
来源：http://hz.kuanghao11.cn/gtxhhcskmo.html

Go:   花括号块级作用域
来源：http://hz.chenlongwang.top/gtyadokdea.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gteohjgqsq.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gtosegniiw.html

[C11] 模块导入与导出
来源：http://hz.redwolf501.top/gtzejmbpaq.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtptgxjogc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.c1oappe.top/gtyjvjsvak.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tianlin.xyz/gtsgaeethb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jiagoushi.top/gtrvilsvoi.html

Java: import java.util.List;
来源：http://hz.wangshuangyany.cn/gtkosnhuqz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhiwuduotai.top/gtzzsbxkni.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.kuanghao11.cn/gtmfycnhrp.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gttbzrjfqq.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtagftrywh.html

Py:   (lambda: print("run"))()
来源：http://hz.ppjwa.cn/gteemixaoe.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtxnbitlke.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hammf.cn/gtcbnrimqa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtiiofkcqk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xingfuxueyuan.xyz/gtgcmwxvdd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhengqikj.top/gtylezmhza.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtrnylewxb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shzxlz.cn/gtiojijeas.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgfzy.top/gtamemtfit.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtdhsvjpjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtshjclgfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.haohaochexian.top/gtoyqivbtw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtugebpsaz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtujscbkxv.html

Go:   func add(a, b int) int
来源：http://hz.hammf.cn/gtnuswnzzd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xingfuxueyuan.xyz/gtmrismyvh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gtbdqqyzow.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtsxtswqqr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gtskaidlta.html

PHP:  // 无泛型
来源：http://hz.yj20258888.top/gtxxwfnpnv.html

JS:   // 无泛型
来源：http://hz.fengsongda.top/gteecbpupy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangkeji.top/gteakryrbe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.0kj1m.cn/gtvpzetqbf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.svipenyu.cn/gtplxzpjme.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gtspeeeukj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hywenlv.cn/gtcdtuocys.html

[C15] 解构 / 展开参数
来源：http://hz.ivvv.top/gtzokdidrr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tianlin.xyz/gtkkflevhi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtmkytmune.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtkdjamoek.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ybcxt.top/gtfsuahivp.html

Java: // 无解构
来源：http://hz.cucudq.cn/gtedecbasf.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtxetbzcfe.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtqbhmykyi.html

C#:   var (a, b) = pair;
来源：http://hz.cashguo.top/gtmatetrvd.html

[C16] 函数 / 方法重载
来源：http://hz.wangdashe.top/gtbsuvspze.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shzxlz.cn/gtdgeoeacn.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtywbubrvr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sysykeji.top/gtqvcswjoi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.iojbl.cn/gtlqvbztkb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydjk.org.cn/gtmbmmccjb.html

Go:   // 无重载：用不同函数名
来源：http://hz.sweek.top/gtuidszhin.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuetiantiany.cn/gtotultrga.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nwbrower.top/gtlmfchzyn.html

================================================================================
来源：http://hz.yueranfly.top/gtnvmcvkqr.html

D. 数组 / 列表 / 集合
来源：http://hz.snrcjt.cn/gteiczgrsv.html

================================================================================
来源：http://hz.yonumen.top/gtyaeipxos.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtucwvanva.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yangfankeji.com/gtsvjrajvx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.andypj.xyz/gtppqflztm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ehwqpu.com/gtkyoedpgr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yvedp.cn/gtpuvnpcts.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenlongwang.top/gthntjbyjz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gtvqgihhsp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtoytqqqjj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fzhhl.top/gtyqzxnxsq.html

[D02] 追加元素到末尾
来源：http://hz.kuanghao11.cn/gtxjlxjbki.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtvyltdaqw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtfamrpnko.html

JS:   arr.push(4);
来源：http://hz.guowangkeji.top/gtjvmyutdu.html

TS:   arr.push(4);
来源：http://hz.iojbl.cn/gtmhibnrxc.html

Java: list.add(4);
来源：http://hz.mhx1999.top/gtvcoqfpby.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtpznktzyz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.quarkkingdee.top/gtvpsqyhxl.html

C#:   list.Add(4);
来源：http://hz.xylfe.cn/gteqlykdcy.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangkeji.top/gtzeeeniqy.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtmsphejvh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnqzz.top/gtqhyfsspc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gzhubu.top/gtxlbdnbeb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sufxvd.cn/gtpqaejtrf.html

Java: list.add(0, 0);
来源：http://hz.yanxiufei.cn/gtpbihuszn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.birdmap.top/gtkhtvwodz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cqqwz.cn/gtlaozbpaq.html

C#:   list.Insert(0, 0);
来源：http://hz.tianlin.xyz/gtkblnyvza.html

[D04] 删除元素
来源：http://hz.yj202588.top/gtnlmevqsj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.c1oappe.top/gturuxivfw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtingwoltu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ivvv.top/gtwytwgpqw.html

TS:   arr.splice(0, 1);
来源：http://hz.xuanzx.com/gtacsbnrgl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ywan-chungtsiang.top/gtfkxqjooq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fzhhl.top/gtwuiyqnuk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gtpshxgujt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hammf.cn/gtaxpbwcva.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtdzqzasso.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtrjvekgar.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ybcxt.top/gtffwpssex.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zycfv.cn/gttzkfrxop.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnxiangtu.top/gtmsrrpkwi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtlplibtke.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtgpfzkfca.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtwpxgscuy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtrqhqpong.html

[D06] 数组长度
来源：http://hz.redwolf501.top/gtpwkuzkvs.html

Py:   len(arr)
来源：http://hz.dianchejie.cn/gthhthdyfn.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtgsmfresl.html

JS:   arr.length
来源：http://hz.shangyingyoupin.top/gtnzisvlyw.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gtwrxzgeyk.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtdzzanytu.html

Go:   len(arr)
来源：http://hz.dashuyun.cn/gtsiqrlnjn.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gtdizmejvb.html

C#:   list.Count;
来源：http://hz.gotoacloud.top/gtagtgdojo.html


<!-- 参考信息 -->