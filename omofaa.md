代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydzc1.top/gtqsnoilat.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gtptcvuajc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hnqzz.top/gtzqbrptld.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.fengsongda.top/gtwebmmzfx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinyuanbaomall.cn/gtohfzdcrh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cdnleiting.top/gterzbziuk.html

[B07] while 循环
来源：http://hz.wangshuangyany.cn/gtpkinbfjp.html

Py:   while i < 10: i += 1
来源：http://hz.9152youxi.cn/gtewuitmch.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.guowangkeji.top/gthpxhrujn.html

JS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtbkosszgx.html

TS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtmeqvyirz.html

Java: while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gthgengqrx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangdashe.top/gtdghycofi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zycfv.cn/gtnmcwqjvp.html

C#:   while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gtuacmwtsw.html

[B08] do-while（至少执行一次）
来源：http://hz.haohaochexian.top/gtgukhxfuo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gogol.net.cn/gtgiuxmubi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pengpengdd.cyou/gtrujnniuu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yongpay.top/gteghlrhvm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtdbodqpsl.html

Java: do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtvsicwdil.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tanke756.top/gtudbsubje.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cdnleiting.top/gtwjxoilvc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtgexqotlm.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gthzdgkoyl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydzc1.top/gtqwlfmvpr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.vqdsnc.cn/gtrjzbesba.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtzspgkmst.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtojyxcyze.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtlskuhlew.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.guannengcc.top/gtptujzcjh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shangyingyoupin.top/gtdwcfgomj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtgpwftfgl.html

[B10] 遍历同时拿索引
来源：http://hz.ybcxt.top/gtdqmanjtc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guowangkeji.top/gtvktrninq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.guannengcc.top/gtkxgtvyvz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.wangshuangyany.cn/gtvdhdicjl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ppjwa.cn/gtvezfxkzi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ydjk.org.cn/gtgcfjcroi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yongpay.top/gtdrbosonc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.daxiang520.top/gtdhvnloko.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yuxming.cn/gtuwhgxsal.html

[B11] 生成数字序列 / 区间
来源：http://hz.xziqi.cn/gtbocoiaiu.html

Py:   list(range(0, 10, 2))
来源：http://hz.gaohongyu789.top/gtczhtwpds.html

PHP:  range(0, 10, 2);
来源：http://hz.redwolf501.top/gtwttxylns.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtcjiyigzv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtulzofvkn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinyuanbaomall.cn/gtlojkucrk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtlvwlnhor.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sxryk.cn/gtlxiflras.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj20258.top/gtgrhpyapx.html

[B12] 跳出多层循环
来源：http://hz.ydzc1.top/gthvjcsugd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jianghu66.top/gtijxdneho.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shzxlz.cn/gtotrdqwcd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtpzlwkmib.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtulbhmzvd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtcbuimclw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sufxvd.cn/gtxvpsmzms.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guowangkeji.top/gtqpyaqspn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.aibaodan.cn/gtnsebsead.html

[B13] 判断是否为数字
来源：http://hz.hywenlv.cn/gtxfaltvhk.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhijiandao.cn/gtmffnogfc.html

PHP:  is_numeric($x)
来源：http://hz.ppjwa.cn/gtobyzjxwx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtpydfddpr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtxzkujchh.html

Java: x instanceof Number
来源：http://hz.guannengcc.top/gtrydswizb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xziqi.cn/gtjzmmcycb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgfzy.top/gtwxdluwzm.html

C#:   x is int or double or decimal
来源：http://hz.pycfn.com/gtfkxxoupb.html

[B14] 判断值是否在集合内
来源：http://hz.daria6918.cn/gthqqylzpd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xziqi.cn/gtbwecerag.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aibaodan.cn/gtggizbedy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtdekodiyn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.316326.xyz/gtpvvfsxwo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cashguo.top/gtdfqoyqcb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nwbrower.top/gtfwwjhmeb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.birdmap.top/gtimpfuzkq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dashuyun.cn/gtjinvikxr.html

[B15] 布尔运算与取反
来源：http://hz.shzxlz.cn/gtweiuaabl.html

Py:   a and b or not c
来源：http://hz.ivvv.top/gtpyxbaqvg.html

PHP:  $a && $b || !$c
来源：http://hz.vqdsnc.cn/gtoycclylq.html

JS:   a && b || !c
来源：http://hz.smart0.xyz/gtfpqpommh.html

TS:   a && b || !c
来源：http://hz.yj20258.top/gtceglwaqv.html

Java: a && b || !c
来源：http://hz.jinqigufen.top/gtpnwntxxt.html

Go:   a && b || !c
来源：http://hz.yvedp.cn/gtypechkpb.html

Ruby: a && b || !c
来源：http://hz.dashuyun.cn/gtarjgbwjk.html

C#:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtzyxlxvbh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jianghu66.top/gthwsrpncb.html

Py:   if not data: return
来源：http://hz.chenlongwang.top/gtbhlcypgo.html

PHP:  if (!$data) { return; }
来源：http://hz.hongshengwenyu.top/gtqkyjdras.html

JS:   if (!data) return;
来源：http://hz.hammf.cn/gtrqghvqmc.html

TS:   if (!data) return;
来源：http://hz.birdmap.top/gtwhbxwxwp.html

Java: if (data == null) return;
来源：http://hz.9152youxi.cn/gtnonnpyyz.html

Go:   if data == nil { return }
来源：http://hz.hnxiangtu.top/gtqcgorgly.html

Ruby: return if data.nil?
来源：http://hz.sysykeji.top/gtcdifajdd.html

C#:   if (data == null) return;
来源：http://hz.guannengcc.top/gtzqfdioax.html

================================================================================
来源：http://hz.yanxiufei.cn/gtsfbcehsm.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtcpigwksa.html

================================================================================
来源：http://hz.svipenyu.cn/gtxzkltjjx.html

[C01] 定义函数
来源：http://hz.hongshengwenyu.top/gtmzdhmfvl.html

Py:   def add(a, b): return a + b
来源：http://hz.zhongyouzk.top/gtvwlbfenv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gaohongyu789.top/gtguledtum.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cucudq.cn/gtjjxalhdi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtjerdtnhq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gtmlurbuem.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ppjwa.cn/gtrkbhjsmb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.bjfxy.top/gtophesuau.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtmnwflmgz.html

[C02] 默认参数
来源：http://hz.yj202588.top/gtxlqwjqza.html

Py:   def greet(name="World"): return name
来源：http://hz.zhaomingkeji.xyz/gtqdibfvxg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zdqjudy.top/gtduetrfmk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.svipenyu.cn/gtupcmncgs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gtmwhgigvg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tanke756.top/gtfmhefcuf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.daxiang520.top/gtlveufdmi.html

Ruby: def greet(name = "World") = name
来源：http://hz.daxiang520.top/gtcfuvezyt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jianghu66.top/gtwynffnoj.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtnqaaroqt.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtljhyylhp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hongshengwenyu.top/gtrlawgiex.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtbvdnhmgi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtmtugufqx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xinyue.icu/gtdhybyaxl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ydzc1.top/gtfibseisd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cqqwz.cn/gtlyszdebp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pengpengdd.cyou/gttveltfwk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shangyingyoupin.top/gtsntxkcld.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nwbrower.top/gtdsufklxr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xuetiantiany.cn/gtragjjyah.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtxtesgmpy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tian-w.cn/gtwwqgndfd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuetiantiany.cn/gtqhbjubsj.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigufen.top/gtszqiuzjv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtlysqinep.html

C#:   f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gthwvlshfu.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gtyhxppkaw.html

Py:   return a, b
来源：http://hz.hongshengwenyu.top/gtucvtrwyk.html

PHP:  return [$a, $b];
来源：http://hz.jinyuanbaomall.cn/gtgydwaigk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ehwqpu.com/gtrskaxftg.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtiqqhjueb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sufxvd.cn/gtigiitvmx.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtaovbzmha.html

Ruby: return a, b
来源：http://hz.birdmap.top/gtdqbqypzw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gtzwcfasts.html

[C06] 匿名函数 / lambda
来源：http://hz.nanxinkj.top/gtvmcdklmt.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtkoazhetl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hongshengwenyu.top/gtxmssuker.html

JS:   const square = x => x * x;
来源：http://hz.cheryme.top/gtbzgithgc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yongpay.top/gtkcmmlage.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinghuilouyu.cn/gtedmsjzej.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ybcxt.top/gtspxaxpkr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinghuilouyu.cn/gtazhxhrja.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yueranfly.top/gtxjmpvwea.html

[C07] 把函数作为参数传入
来源：http://hz.wangshuangyany.cn/gtxesllncy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cashguo.top/gtvdqyqisy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yvedp.cn/gtdfunduqo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daria6918.cn/gtbfukwmje.html

TS:   arr.map(String)
来源：http://hz.yj202588.top/gtpqzlpnvj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgfzy.top/gtjhsxfiqz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xinyue.icu/gtinydbyfa.html

Ruby: arr.map(&:upcase)
来源：http://hz.hywenlv.cn/gtyldjusje.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258.top/gtbqhuppul.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtihuymbam.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.meibo888.top/gtnizreciy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guannengcc.top/gtdzzxbxcl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gttktkqgyj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtbvogeqqf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xingfuxueyuan.xyz/gtsjrhmxcm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gttbqqxdlq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuxming.cn/gtqpdcicca.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtcnorlqug.html

[C09] 递归
来源：http://hz.ivvv.top/gtdbhkrtbl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuxming.cn/gtylmujsfi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fengsongda.top/gtlqsfnxbu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tianlin.xyz/gtzhdqydxn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.9152youxi.cn/gtdmufdqhs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yangfankeji.com/gtthkaukag.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cdnleiting.top/gtkfgsudgi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtchaquvet.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jlsjyb.cn/gtfeephmvf.html

[C10] 变量作用域
来源：http://hz.kuanghao11.cn/gthqubuepw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pycfn.com/gteawyclxq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cqqwz.cn/gtkbpwoagw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hfpthk.cn/gtgbeqthlh.html

TS:   同 JS
来源：http://hz.zhoulong.xyz/gtoymepubx.html

Java: 方法内为块级作用域
来源：http://hz.zdqjudy.top/gtvfnxnkts.html

Go:   花括号块级作用域
来源：http://hz.zhiwuduotai.top/gtrzvbbvko.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pycfn.com/gtgkouhdck.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gtkbgtvefp.html

[C11] 模块导入与导出
来源：http://hz.zhijiandao.cn/gtdoxniwsr.html

Py:   from module import func
来源：http://hz.chenjidiqi.icu/gtbepjseho.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.svipenyu.cn/gtwygaukgz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jyoumei.cn/gtemgifaze.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.birdmap.top/gtlmzmfius.html

Java: import java.util.List;
来源：http://hz.shanyushiyangtech.top/gtbxxaoyvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxuanxn.top/gtwyuidbrq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.feifeiyinyue.top/gtnxbnsrvm.html

C#:   using System.Text;
来源：http://hz.tanke756.top/gtxvenjcsc.html

[C12] 立即执行函数 IIFE
来源：http://hz.ehwqpu.com/gtlsvhcfgd.html

Py:   (lambda: print("run"))()
来源：http://hz.svipenyu.cn/gtmaggmbpu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tanke756.top/gtfrguljbl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.feifeiyinyue.top/gtaigfjyln.html

TS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtdccmekkg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinghuilouyu.cn/gtpubhtevv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenzaomai.com/gtniimdaph.html

Ruby: -> { puts "run" }.call
来源：http://hz.shzxlz.cn/gtsvwfkvlp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtxjuebdro.html

[C13] 类型声明 / 类型注解
来源：http://hz.pengpengdd.cyou/gtsrhjssia.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhengqikj.top/gtmlvcfyft.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtfrmupvnk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yonumen.top/gtxwjicdvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtqzonrzkn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gttzeokwdh.html

Go:   func add(a, b int) int
来源：http://hz.hywenlv.cn/gtgazgmjcw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhixingplan.top/gthqsrnkyp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sufxvd.cn/gtwzloarvh.html

[C14] 泛型函数
来源：http://hz.shangyingyoupin.top/gtgcbbuqnz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.fengsongda.top/gtvkodwbdv.html

PHP:  // 无泛型
来源：http://hz.yj20258.top/gttgoutgkb.html

JS:   // 无泛型
来源：http://hz.zycfv.cn/gtzkssprnj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenlongwang.top/gtjqkfduel.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtfcaygkmm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gthmcpdesd.html

Ruby: # 无泛型
来源：http://hz.snrcjt.cn/gtipzchxlx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yonumen.top/gtzoxuauiv.html

[C15] 解构 / 展开参数
来源：http://hz.zhongyouzk.top/gtvttpwora.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtjxenzkku.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guannengcc.top/gtkkjqwygk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtecpshbbf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtwpntyfov.html

Java: // 无解构
来源：http://hz.guowangkeji.top/gtjxienzcx.html

Go:   // 无解构
来源：http://hz.birdmap.top/gtgbkavryl.html

Ruby: a, b = pair
来源：http://hz.xziqi.cn/gtfidgzmbz.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gtcyypboic.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtxmolmmsw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ehwqpu.com/gthaybqmmk.html

PHP:  // 无重载
来源：http://hz.xuanzx.com/gtpbbicynl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yangfankeji.com/gtfkaxnaxb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxinkj.top/gtsfgdbtzu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yangfankeji.com/gtdtsqvqys.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhongyouzk.top/gtfhlcctbd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinyuanbaomall.cn/gtpsbpjvbc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aizwys.cn/gtucxqohfm.html

================================================================================
来源：http://hz.daxiang520.top/gtjcqrkkor.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gtcdjonpip.html

================================================================================
来源：http://hz.yongpay.top/gtzyivyqla.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtpfcdslpx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhongyouzk.top/gtdgymxzvv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenjidiqi.icu/gtkhqeenhf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dashuyun.cn/gtntwevqrn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yuanzhike.top/gttkfrwmyz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gthnncrpal.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtjvwlgjvu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtseenvcfr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jlsjyb.cn/gtzhvtyhgf.html

[D02] 追加元素到末尾
来源：http://hz.chenlongwang.top/gtphydlwyr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.9152youxi.cn/gtmmtfjyku.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yueranfly.top/gtneuabasj.html

JS:   arr.push(4);
来源：http://hz.mhx1999.top/gtyhzrqcsw.html

TS:   arr.push(4);
来源：http://hz.zhaomingkeji.xyz/gtcyhrgfta.html

Java: list.add(4);
来源：http://hz.mhx1999.top/gtycqcpjrz.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gtvqdllpnc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guannengcc.top/gtwygmxuyj.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtcnxvhcfx.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigufen.top/gtszblfgfd.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtlydrqzll.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sysykeji.top/gtcpaqjthp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ehwqpu.com/gtulkboetx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hammf.cn/gtcyovplkc.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gtwawcejua.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangkeji.top/gtdadwxdwc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gtqjnlccle.html

C#:   list.Insert(0, 0);
来源：http://hz.feifeiyinyue.top/gtvaarqkkb.html

[D04] 删除元素
来源：http://hz.pengpengdd.cyou/gtmheieopg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenjidiqi.icu/gtvuwltvnq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtpgkdbcdi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydzc1.top/gtahdnjzdi.html

TS:   arr.splice(0, 1);
来源：http://hz.shzxlz.cn/gtgynhpspl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jianghu66.top/gtivnmifqd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj20258888.top/gtufpgctrj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtzfzutsen.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtvfhbxbmf.html

[D05] 访问与修改元素
来源：http://hz.zhengqikj.top/gtbksfjdha.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtvaforhoc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.mhx1999.top/gtmzognwmj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydzc1.top/gtohmzwqes.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xziqi.cn/gtmocljwyx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtyhhbosmz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtbtnejjuf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gttpedtxtb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtqnfdxjqt.html

[D06] 数组长度
来源：http://hz.svipenyu.cn/gtxbzqmjpf.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtioiffdgr.html

PHP:  count($arr);
来源：http://hz.iojbl.cn/gthifjixvg.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtkkwxougu.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtsyvgvqwd.html

Java: list.size();
来源：http://hz.wangshuangyany.cn/gthmvkgjmc.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtqpxytpsk.html

Ruby: arr.length; arr.size
来源：http://hz.c1oappe.top/gthzqilbqd.html

C#:   list.Count;
来源：http://hz.xingfuxueyuan.xyz/gtbtcimpys.html


<!-- 参考信息 -->