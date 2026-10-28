代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.zycfv.cn/gtqjzdjjav.html

Py:   for item in arr: print(item)
来源：http://hz.yangfankeji.com/gtnoxjspkl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.wangdashe.top/gtnuypwjbn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.vqdsnc.cn/gtstljcsdl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhoulong.xyz/gtbyewveqo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shzxlz.cn/gtmnatvziu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.dashuyun.cn/gtsmlarcsm.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj20258.top/gtlygkrbcm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.snrcjt.cn/gtdqdhkxdy.html

[B06] 遍历字典 / 对象
来源：http://hz.cucudq.cn/gtokxbnfxa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ppjwa.cn/gtmxsbdovx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.havefunace.top/gtfxnxyobt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gzhubu.top/gtqmdgzecn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhaomingkeji.xyz/gtirzuemde.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.birdmap.top/gtfrbzkluj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ybcxt.top/gtqrhojgru.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yangfankeji.com/gtuhwjmujv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yvedp.cn/gtvxpetvro.html

[B07] while 循环
来源：http://hz.andypj.xyz/gthijmfraw.html

Py:   while i < 10: i += 1
来源：http://hz.ivvv.top/gtqjtegpwr.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zdqjudy.top/gtxzlzsque.html

JS:   while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gtedymdkvq.html

TS:   while (i < 10) { i++; }
来源：http://hz.shzxlz.cn/gtghkgmamg.html

Java: while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtzycfpkyx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.havefunace.top/gtsvzgxtxc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shuidangran.top/gtffalmryf.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtcljwutgp.html

[B08] do-while（至少执行一次）
来源：http://hz.zhiwuduotai.top/gtvsexiyzs.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.wangshuangyany.cn/gtwvlhqlhb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pengpengdd.cyou/gtqyinflek.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtwcjhgmtn.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gtpjifhefe.html

Java: do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtftqzntkv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.0kj1m.cn/gtsdubrenw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yj20258.top/gtvovtsgyr.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtcagxdjts.html

[B09] break 与 continue
来源：http://hz.chenjidiqi.icu/gtngjxdbcg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cqqwz.cn/gtfayyberp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ivvv.top/gtolkawpzc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtudvnzkgt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtrlvggaqh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gteoebjmxt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.guannengcc.top/gtcmfddydn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gotoacloud.top/gtiusdzaxg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtbeexvroz.html

[B10] 遍历同时拿索引
来源：http://hz.jqgufenzy.top/gtneyinlnw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sweek.top/gtygnpafwm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yangfankeji.com/gtjtibbejw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daria6918.cn/gtwdwpcmho.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hammf.cn/gtrxkeirxl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gtxodplqzp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.andypj.xyz/gtnvhzccgh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shanyushiyangkeji.top/gtyylumhxm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.daria6918.cn/gtzwcwccer.html

[B11] 生成数字序列 / 区间
来源：http://hz.pengpengdd.cyou/gtgmuisemj.html

Py:   list(range(0, 10, 2))
来源：http://hz.cashguo.top/gtylxsplrx.html

PHP:  range(0, 10, 2);
来源：http://hz.zhongyouzk.top/gtrmthoqrv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtxitzvsta.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtzqyswjto.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.52xcode.cn/gtholruhcd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.0kj1m.cn/gtaimpdcvh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtpgjikluy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenjidiqi.icu/gtlqqsfllk.html

[B12] 跳出多层循环
来源：http://hz.daria6918.cn/gtlzyhpmcn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhiwuduotai.top/gtdmdjwocm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.kuanghao11.cn/gtnufjxzns.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtbewtfjbl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtrhdvyfrk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtjbywhcbv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zdqjudy.top/gtviiqeemn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnqzz.top/gttfjphibo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangdashe.top/gtljjimedf.html

[B13] 判断是否为数字
来源：http://hz.vqdsnc.cn/gtyivfepta.html

Py:   isinstance(x, (int, float))
来源：http://hz.yonumen.top/gtnuxrrpyh.html

PHP:  is_numeric($x)
来源：http://hz.ydzc1.top/gtoirkygox.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shzxlz.cn/gtwqcdkubm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cheryme.top/gtwxdtafqz.html

Java: x instanceof Number
来源：http://hz.yuanzhike.top/gthcseksab.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.smart0.xyz/gtzdspzpys.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hammf.cn/gthodhmksf.html

C#:   x is int or double or decimal
来源：http://hz.jinghuilouyu.cn/gtbhmnfkte.html

[B14] 判断值是否在集合内
来源：http://hz.yonumen.top/gtiwkfyjlb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.c1oappe.top/gtcejscdou.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yvedp.cn/gtefwxxtax.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shangyingyoupin.top/gtylvlzzcj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtlszlpssk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhaomingkeji.xyz/gtfjjtqrjj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jlsjyb.cn/gtbjdpakam.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.mhx1999.top/gtwtwroqec.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgfzy.top/gtvtzewezx.html

[B15] 布尔运算与取反
来源：http://hz.kuanghao11.cn/gtwmytxhcs.html

Py:   a and b or not c
来源：http://hz.feifeiyinyue.top/gtexcfthfs.html

PHP:  $a && $b || !$c
来源：http://hz.bjfxy.top/gtgxoqljce.html

JS:   a && b || !c
来源：http://hz.yvedp.cn/gtlgvtkdbj.html

TS:   a && b || !c
来源：http://hz.ppjwa.cn/gtftpsfefd.html

Java: a && b || !c
来源：http://hz.guowangkeji.top/gtclgswmgc.html

Go:   a && b || !c
来源：http://hz.svipenyu.cn/gtonekhffu.html

Ruby: a && b || !c
来源：http://hz.0kj1m.cn/gtlumparvo.html

C#:   a && b || !c
来源：http://hz.gotoacloud.top/gtepsprnkp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cucudq.cn/gtmanwfeqw.html

Py:   if not data: return
来源：http://hz.daxiang520.top/gturbbusck.html

PHP:  if (!$data) { return; }
来源：http://hz.shanyushiyangtech.top/gtqcnvkuer.html

JS:   if (!data) return;
来源：http://hz.aizwys.cn/gtmzublejt.html

TS:   if (!data) return;
来源：http://hz.ydjk.org.cn/gtpmldgakz.html

Java: if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtbkjfcutq.html

Go:   if data == nil { return }
来源：http://hz.cheryme.top/gtosukwbik.html

Ruby: return if data.nil?
来源：http://hz.xziqi.cn/gtxityarby.html

C#:   if (data == null) return;
来源：http://hz.hysaishi.cn/gtqrnbytzv.html

================================================================================
来源：http://hz.havefunace.top/gtpxzojatj.html

C. 函数与作用域
来源：http://hz.jyoumei.cn/gtwsjzmnxa.html

================================================================================
来源：http://hz.xziqi.cn/gtziitujpe.html

[C01] 定义函数
来源：http://hz.yangfankeji.com/gtwkxyilnb.html

Py:   def add(a, b): return a + b
来源：http://hz.zhaomingkeji.xyz/gtvavazsew.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtmhtzxzjg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gttiezfbsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gthbkkwvzp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtjahcxumw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shangyingyoupin.top/gtadlwhldq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinghuilouyu.cn/gtjwfsuwgh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtndsuwdcc.html

[C02] 默认参数
来源：http://hz.guannengcc.top/gtaxywmdjt.html

Py:   def greet(name="World"): return name
来源：http://hz.cheryme.top/gthuiewsio.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pengpengdd.cyou/gtugbiewli.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.havefunace.top/gtcknlhtnc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pycfn.com/gtpxjejqxo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cashguo.top/gtjyobmdkl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgufenzy.top/gtufabhtxq.html

Ruby: def greet(name = "World") = name
来源：http://hz.cheryme.top/gtwodiieor.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yvedp.cn/gtkfbjqdhg.html

[C03] 可变参数
来源：http://hz.jinghuilouyu.cn/gtsxqtndzn.html

Py:   def total(*args): return sum(args)
来源：http://hz.tianlin.xyz/gtypitbbpz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cdnleiting.top/gtjzethnii.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtkcunswdm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtkdppiixc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.birdmap.top/gtyrrgwcoz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhijiandao.cn/gtazgrombd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tianlin.xyz/gtolavvtqo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydjk.org.cn/gttnepzywq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhijiandao.cn/gtnpncktzu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.vqdsnc.cn/gtyckoxlqn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigufen.top/gtixnjwdml.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtdibicejw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hongshengwenyu.top/gtmaethlgi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yvedp.cn/gtpywfwris.html

Go:   // 无：用配置结构体参数
来源：http://hz.sufxvd.cn/gtfwiurfex.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtegdcsflr.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtwpootlje.html

[C05] 返回多个值
来源：http://hz.jinqigufen.top/gtwvatjkhx.html

Py:   return a, b
来源：http://hz.jiagoushi.top/gtitxqmmoe.html

PHP:  return [$a, $b];
来源：http://hz.tian-w.cn/gtcwltwepk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtvjaolfzy.html

TS:   return { a, b };
来源：http://hz.xylfe.cn/gtqkckfguz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangkeji.top/gtzmnatpfv.html

Go:   return a, b
来源：http://hz.havefunace.top/gtkdhjaozb.html

Ruby: return a, b
来源：http://hz.chenlongwang.top/gtwuzbvenr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtrwciquvz.html

[C06] 匿名函数 / lambda
来源：http://hz.guowangkeji.top/gtntzqtpgr.html

Py:   square = lambda x: x * x
来源：http://hz.fengsongda.top/gtnhxlafop.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenlongwang.top/gtzicyxdhr.html

JS:   const square = x => x * x;
来源：http://hz.xuetiantiany.cn/gthnntoloj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gteqpdevsi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhaomingkeji.xyz/gtpwdkyumy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xingfuxueyuan.xyz/gtoabcbhuv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangkeji.top/gterpebrfb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.redwolf501.top/gtwihhctyu.html

[C07] 把函数作为参数传入
来源：http://hz.sysykeji.top/gtiscnbbmm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxinkj.top/gtfwfssqzm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tian-w.cn/gtfitrpvdz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gtemhfzobt.html

TS:   arr.map(String)
来源：http://hz.hongshengwenyu.top/gtwrrkijyd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cdnleiting.top/gteeroyjzb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtjqwihqxm.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhiwuduotai.top/gtxlfboizb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yvedp.cn/gtbvuffugq.html

[C08] 闭包
来源：http://hz.snrcjt.cn/gtufmybowm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cheryme.top/gteevuieri.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.redwolf501.top/gtwamqzulq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtselgjtxz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtmovhgnfr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhaomingkeji.xyz/gtoswsjhfr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangshuangyany.cn/gtwrnhwuaq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jiagoushi.top/gtezcdrpux.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtdswhjqsr.html

[C09] 递归
来源：http://hz.guannengcc.top/gtvgbxexup.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuxming.cn/gtdglnrsgn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.birdmap.top/gtdijkprxt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gttalnyucn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtfiwzevrn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtoaayxdew.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtbibvbhzq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtutzvkmgl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xziqi.cn/gtfjgzhrpw.html

[C10] 变量作用域
来源：http://hz.tian-w.cn/gthfynroze.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xinyue.icu/gtdketcvdn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xylfe.cn/gtubpqjbxx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtewpzcxws.html

TS:   同 JS
来源：http://hz.316326.xyz/gtcvfjoork.html

Java: 方法内为块级作用域
来源：http://hz.andypj.xyz/gtnkmhndcl.html

Go:   花括号块级作用域
来源：http://hz.hongshengwenyu.top/gtvwvjrhhd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tian-w.cn/gtuwfusofc.html

C#:   块级作用域
来源：http://hz.snrcjt.cn/gtebrtpvwb.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtsvijkwuj.html

Py:   from module import func
来源：http://hz.shuidangran.top/gtyqdmdgoz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhoulong.xyz/gtpvgexcjg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tanke756.top/gtgrpnwnko.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.svipenyu.cn/gtbgwmeepi.html

Java: import java.util.List;
来源：http://hz.sufxvd.cn/gtxmbehuku.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ehwqpu.com/gtjdhxtxii.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sxryk.cn/gtjnngpoli.html

C#:   using System.Text;
来源：http://hz.zhoulong.xyz/gtwjoutiay.html

[C12] 立即执行函数 IIFE
来源：http://hz.hammf.cn/gthuryklzx.html

Py:   (lambda: print("run"))()
来源：http://hz.bjfxy.top/gtfgsncvxq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xingfuxueyuan.xyz/gtzntmcjfj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtdkkqjqyi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtavnfrblh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.meibo888.top/gtgtdkhdmy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hongshengwenyu.top/gtawrdtcnl.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gtsgcwigvh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtoysvoour.html

[C13] 类型声明 / 类型注解
来源：http://hz.daxiang520.top/gtcptbkgnp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.snrcjt.cn/gtiueajlfc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtswrodacv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.316326.xyz/gtbntlplfq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtmwazcqrk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtgtczauor.html

Go:   func add(a, b int) int
来源：http://hz.sxryk.cn/gtdczsnxjp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gtdqonvtod.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gtloviamhs.html

[C14] 泛型函数
来源：http://hz.dianchejie.cn/gtjmfdnere.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.vqdsnc.cn/gtotzjwktw.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gteyemlpps.html

JS:   // 无泛型
来源：http://hz.chenzaomai.com/gtnngjkfhr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinyuanbaomall.cn/gteysairyq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtgmehvnon.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhoulong.xyz/gtdduvrcap.html

Ruby: # 无泛型
来源：http://hz.zdqjudy.top/gtednvjvdv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhiwuduotai.top/gtjcedvsqf.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtmioanmzy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.vqdsnc.cn/gtauhyfvpf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yanxiufei.cn/gtxzttqubf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtrxvpqczv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hysaishi.cn/gtxcbiqqnk.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtfpnduebo.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtiohbkcpp.html

Ruby: a, b = pair
来源：http://hz.kuanghao11.cn/gtmigfocvi.html

C#:   var (a, b) = pair;
来源：http://hz.guowangkeji.top/gtejcegrio.html

[C16] 函数 / 方法重载
来源：http://hz.hongshengwenyu.top/gtcxrojnqv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhongyouzk.top/gtacaqjzda.html

PHP:  // 无重载
来源：http://hz.wangshuangyany.cn/gtzzgqqipn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daria6918.cn/gtgesxdblt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigufen.top/gtpmkzntro.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ybcxt.top/gtqwppjdoo.html

Go:   // 无重载：用不同函数名
来源：http://hz.hysaishi.cn/gtuunsleca.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guannengcc.top/gtjbtgklwt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zdqjudy.top/gtuggjmklz.html

================================================================================
来源：http://hz.xinyue.icu/gtfnxjhuvn.html

D. 数组 / 列表 / 集合
来源：http://hz.cqqwz.cn/gtqfgbnevr.html

================================================================================
来源：http://hz.sweek.top/gtksthvivu.html

[D01] 创建数组 / 列表
来源：http://hz.zhoulong.xyz/gtoqwggftf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gogol.net.cn/gtcyledvdd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.iojbl.cn/gtxzmpernn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hysaishi.cn/gttmwkpere.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gthlpzxasw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yueranfly.top/gtxovhjvuz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgfzy.top/gtkcvethhn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtjihkhbso.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shanyushiyangtech.top/gtkvbspdnb.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtondlvmew.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sysykeji.top/gtqlpmofff.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnxiangtu.top/gtpujvgxrg.html

JS:   arr.push(4);
来源：http://hz.fzhhl.top/gtzmsnjgxy.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtgowdakfv.html

Java: list.add(4);
来源：http://hz.zhoulong.xyz/gtccubwfwy.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtvuvdrkio.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.bjfxy.top/gtfcmpyjiq.html

C#:   list.Add(4);
来源：http://hz.dianchejie.cn/gtcvkupegm.html

[D03] 在指定位置插入元素
来源：http://hz.jqgfzy.top/gttgscqugl.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtrukhdnzh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtshukxitj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shzxlz.cn/gtbwfyypol.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydzc1.top/gtskjngjez.html

Java: list.add(0, 0);
来源：http://hz.zdqjudy.top/gtbwonfxox.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.birdmap.top/gtmtcqsmxs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gteypezbac.html

C#:   list.Insert(0, 0);
来源：http://hz.gotoacloud.top/gtaweklowa.html

[D04] 删除元素
来源：http://hz.yj202588.top/gtxgcrauck.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.vqdsnc.cn/gthtkyrvej.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtqypsutyb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hywenlv.cn/gtmptqwurs.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtyswxcqec.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cheryme.top/gtwyjblkxj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ppjwa.cn/gtadtwbmnw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtcprihcpa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fzhhl.top/gtvmdcixex.html

[D05] 访问与修改元素
来源：http://hz.jqgfzy.top/gtakrxzczt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtmjrncqvg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gthnztgace.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.316326.xyz/gtdtztrqst.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daxiang520.top/gttvvhwycq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuanzx.com/gtkejpawtn.html


<!-- 参考信息 -->