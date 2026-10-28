代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sxryk.cn/gtwblkmkxb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.daxiang520.top/gtpzgevren.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhijiandao.cn/gtkbtzllch.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangdashe.top/gtseniqyxk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenlongwang.top/gtggqduedq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shangyingyoupin.top/gtnlcrzvtu.html

[B07] while 循环
来源：http://hz.daxiang520.top/gtyvrztbbf.html

Py:   while i < 10: i += 1
来源：http://hz.ppjwa.cn/gtwjytbggy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yj20258.top/gtxevsvckm.html

JS:   while (i < 10) { i++; }
来源：http://hz.havefunace.top/gtetcflkhx.html

TS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtwwilmsbw.html

Java: while (i < 10) { i++; }
来源：http://hz.havefunace.top/gtouxifwoi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenlongwang.top/gtrjdqojyk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.52xcode.cn/gtoywyabmr.html

C#:   while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtdqsnxukk.html

[B08] do-while（至少执行一次）
来源：http://hz.hnqzz.top/gtkrfqlvpq.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.9152youxi.cn/gtskujvoop.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenlongwang.top/gtsdxmhvev.html

JS:   do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtefncqzan.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtjqsvyyfs.html

Java: do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtfqohkgmi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.9152youxi.cn/gtwaohawfp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhongyouzk.top/gtaykgdvxz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtexjdbsoz.html

[B09] break 与 continue
来源：http://hz.zhixingplan.top/gtjonzbemp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daria6918.cn/gtiqsnaydn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hammf.cn/gteyqqfmvq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtzrsirnpm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtxmnltxfk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtwfvjvehk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shangyingyoupin.top/gtbisguevf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtaymsmxgl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtpcuufzhw.html

[B10] 遍历同时拿索引
来源：http://hz.zhongyouzk.top/gteneonsps.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tianlin.xyz/gtdrlzxqdg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.snrcjt.cn/gtgrovphqr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj20258.top/gtyroiqtys.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhoulong.xyz/gtpetjates.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tanke756.top/gtthmrpktu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yonumen.top/gtnssajpoh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtpscgwmpp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.9152youxi.cn/gtbsfwldko.html

[B11] 生成数字序列 / 区间
来源：http://hz.cqqwz.cn/gtxtxvktyg.html

Py:   list(range(0, 10, 2))
来源：http://hz.wangdashe.top/gtrjktoioc.html

PHP:  range(0, 10, 2);
来源：http://hz.zhiwuduotai.top/gtyeylnyeg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtejnxmanw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cucudq.cn/gtqnhrunpd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shangyingyoupin.top/gtgomugtmu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gtjdcdpgpk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.birdmap.top/gtjzlarsec.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yangfankeji.com/gtztxytjap.html

[B12] 跳出多层循环
来源：http://hz.cdnleiting.top/gttbfuhysi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xziqi.cn/gtnkyainwt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dianchejie.cn/gtzvnssjqg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtilndbhdn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtlakkkjfc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cqqwz.cn/gtsqslcacd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sweek.top/gtdtwjozqv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cdnleiting.top/gtddkdhfdb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhengqikj.top/gtnsdjpfnh.html

[B13] 判断是否为数字
来源：http://hz.cdnleiting.top/gtlopsmnzk.html

Py:   isinstance(x, (int, float))
来源：http://hz.xingfuxueyuan.xyz/gtetddzsnt.html

PHP:  is_numeric($x)
来源：http://hz.yvedp.cn/gthkwjiopq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gtvxmgumuc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtddemimej.html

Java: x instanceof Number
来源：http://hz.dianchejie.cn/gtjcbofdas.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gteezaedro.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hywenlv.cn/gtdzghzxad.html

C#:   x is int or double or decimal
来源：http://hz.ppjwa.cn/gtlgqbdmdm.html

[B14] 判断值是否在集合内
来源：http://hz.redwolf501.top/gtknyiwuno.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sufxvd.cn/gtuyouvtjr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sxryk.cn/gtprgrlwjv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jqgfzy.top/gtfnwydwiz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xuanzx.com/gtyebgeqwg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gthiilrvbg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xinyue.icu/gtobbixkbn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinyuanbaomall.cn/gtppbdubcl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hnqzz.top/gtvhguqqhy.html

[B15] 布尔运算与取反
来源：http://hz.yueranfly.top/gtomfgmasx.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtqwjcgpxe.html

PHP:  $a && $b || !$c
来源：http://hz.yanxiufei.cn/gtxlvajala.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gtfurqrbkn.html

TS:   a && b || !c
来源：http://hz.zycfv.cn/gtdlxgaskg.html

Java: a && b || !c
来源：http://hz.feifeiyinyue.top/gtjxprovzv.html

Go:   a && b || !c
来源：http://hz.aizwys.cn/gtfsuzmozp.html

Ruby: a && b || !c
来源：http://hz.zhongyouzk.top/gtgcjqukcw.html

C#:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtnoxulskg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtusektmfs.html

Py:   if not data: return
来源：http://hz.shangyingyoupin.top/gtwtkfvzkg.html

PHP:  if (!$data) { return; }
来源：http://hz.chenlongwang.top/gtcoawwmfi.html

JS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtojxeqibj.html

TS:   if (!data) return;
来源：http://hz.hysaishi.cn/gtljwjubli.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtkqrwfxat.html

Go:   if data == nil { return }
来源：http://hz.jianghu66.top/gtfyigjdks.html

Ruby: return if data.nil?
来源：http://hz.pengpengdd.cyou/gtxjdeciyj.html

C#:   if (data == null) return;
来源：http://hz.fzhhl.top/gtegpmzvek.html

================================================================================
来源：http://hz.yonumen.top/gttqqempot.html

C. 函数与作用域
来源：http://hz.zhaomingkeji.xyz/gthxtqgrua.html

================================================================================
来源：http://hz.jlsjyb.cn/gtnyqdupyg.html

[C01] 定义函数
来源：http://hz.tian-w.cn/gtpbuahrze.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxuanxn.top/gtnpekrcbt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtnsocluot.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.bjfxy.top/gtfsdubaew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gtykjstmzj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtqcvvjzil.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258.top/gtdnvmlmxt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ydzc1.top/gtvvlovxqi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtrpglkfkp.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtpmrzpvkj.html

Py:   def greet(name="World"): return name
来源：http://hz.yj202588.top/gtcghyjbcc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.9152youxi.cn/gttfmvyulo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xylfe.cn/gtbpjrdwqi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dashuyun.cn/gtntrsbeyu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sufxvd.cn/gthvpsuusy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenlongwang.top/gtlyydibmm.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangshuangyany.cn/gteyomfqvn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.andypj.xyz/gtrqajnfmt.html

[C03] 可变参数
来源：http://hz.dianchejie.cn/gteofoczza.html

Py:   def total(*args): return sum(args)
来源：http://hz.hammf.cn/gthzlltitd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.redwolf501.top/gtotwvvmcw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gttxxohtpt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtlcxkbjzc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yuxming.cn/gtsypyolcc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhengqikj.top/gtjzkqmoez.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigufen.top/gtozjofyct.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.meibo888.top/gtmgaahslo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cashguo.top/gtjfyaiqqc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sxryk.cn/gtklaoyedd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtbutitpks.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtpeakzoap.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gtikmxipib.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuanzx.com/gtrlcbhgfd.html

Go:   // 无：用配置结构体参数
来源：http://hz.feifeiyinyue.top/gtznhfgfbi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtdxhlqinv.html

C#:   f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtepiqhqmq.html

[C05] 返回多个值
来源：http://hz.pycfn.com/gtqxrkzqlc.html

Py:   return a, b
来源：http://hz.iojbl.cn/gtcfygdxlh.html

PHP:  return [$a, $b];
来源：http://hz.yj20258.top/gttisgbgqn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daxiang520.top/gtcskihobs.html

TS:   return { a, b };
来源：http://hz.fengsongda.top/gtatarlfax.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtawfouile.html

Go:   return a, b
来源：http://hz.chenzaomai.com/gtldeefkzj.html

Ruby: return a, b
来源：http://hz.52xcode.cn/gtkunvfxoj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sxryk.cn/gtmnlvchpf.html

[C06] 匿名函数 / lambda
来源：http://hz.gzhubu.top/gtcgatppvv.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtxlryibas.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xylfe.cn/gtfhmjfzhc.html

JS:   const square = x => x * x;
来源：http://hz.jinqigfzy.top/gtespzdkef.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gtqeiidkbf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ppjwa.cn/gtnyznzjpx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hywenlv.cn/gtdupgutes.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yongpay.top/gtguzkgjoc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pycfn.com/gtlcfygtrs.html

[C07] 把函数作为参数传入
来源：http://hz.cheryme.top/gtetgekzft.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgufenzy.top/gtvfwdeeea.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yanxiufei.cn/gtdgrjluat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxuanxn.top/gtwgcoiipa.html

TS:   arr.map(String)
来源：http://hz.nanxinkj.top/gtkkfprrcb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nwbrower.top/gtgwrcijgq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jiagoushi.top/gtvawgzwrq.html

Ruby: arr.map(&:upcase)
来源：http://hz.feifeiyinyue.top/gthjowrdnt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.svipenyu.cn/gtdpmrpyya.html

[C08] 闭包
来源：http://hz.sufxvd.cn/gtmxoghqie.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tianlin.xyz/gtetilibcm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aizwys.cn/gtmnzioshe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtwazayekb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtbzmdgrmd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtvycrcfct.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yueranfly.top/gtmrghpgen.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hongshengwenyu.top/gtugejbcuf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gttflkrfhg.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtsgrhuuhn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtawyhklhx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guannengcc.top/gtvnlgemqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtiyxecbof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtoqxabgcd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtmtnlomfa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hfpthk.cn/gtimturhjo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtxbdqmupc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.9152youxi.cn/gtalqcavxp.html

[C10] 变量作用域
来源：http://hz.hammf.cn/gtksqtymek.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenjidiqi.icu/gtrkthziav.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gtwtkecnkm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtundfzxzt.html

TS:   同 JS
来源：http://hz.meibo888.top/gtzuxzjfvg.html

Java: 方法内为块级作用域
来源：http://hz.snrcjt.cn/gtvwsondxd.html

Go:   花括号块级作用域
来源：http://hz.yj20258.top/gtdqygvinz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gtkgutxjfd.html

C#:   块级作用域
来源：http://hz.ydzc1.top/gthfesvjpq.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtolarfsbv.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtszcxzkur.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jqgufenzy.top/gtokuqmaon.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shangyingyoupin.top/gtirsbxvgj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinghuilouyu.cn/gtldmyvwef.html

Java: import java.util.List;
来源：http://hz.cdnleiting.top/gtiktpmhqr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnxiangtu.top/gtaxfetdvs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nwbrower.top/gttaxlstng.html

C#:   using System.Text;
来源：http://hz.hammf.cn/gtldhzjavf.html

[C12] 立即执行函数 IIFE
来源：http://hz.xylfe.cn/gtekmftqvc.html

Py:   (lambda: print("run"))()
来源：http://hz.fzhhl.top/gtbcolcyjt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tanke756.top/gthsjwnuat.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtrnqcbltt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtitmnurfo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xingfuxueyuan.xyz/gtyelmczgh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.kuanghao11.cn/gtgskhwvvk.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuetiantiany.cn/gthvenzebt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gteolnjpsz.html

[C13] 类型声明 / 类型注解
来源：http://hz.daxiang520.top/gtkodapian.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yvedp.cn/gtdeneqyrn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtgdlgkdzw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhixingplan.top/gturixhvgk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtmpblmsje.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtbkmnepae.html

Go:   func add(a, b int) int
来源：http://hz.fengsongda.top/gtwectcrib.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.haohaochexian.top/gtvhnohmap.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gtpcwkykup.html

[C14] 泛型函数
来源：http://hz.hysaishi.cn/gtfyaqpjrd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenzaomai.com/gtjfvbuihn.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtdypthcvk.html

JS:   // 无泛型
来源：http://hz.sweek.top/gtszgjkrfd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gtanqihgxd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.smart0.xyz/gtsieeyemv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtvancibkt.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtpyccqijc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jlsjyb.cn/gtstcpbapm.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtwawunvlj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuanzhike.top/gtnumoqyna.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtwbebwvol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtodnfqtei.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhijiandao.cn/gteogspaoq.html

Java: // 无解构
来源：http://hz.jinyuanbaomall.cn/gtjijtdgro.html

Go:   // 无解构
来源：http://hz.ywan-chungtsiang.top/gtlsrfobim.html

Ruby: a, b = pair
来源：http://hz.zhaomingkeji.xyz/gtorrdvlrx.html

C#:   var (a, b) = pair;
来源：http://hz.ehwqpu.com/gtpexzetgd.html

[C16] 函数 / 方法重载
来源：http://hz.pengpengdd.cyou/gtmtcyudam.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.andypj.xyz/gthejkxhsd.html

PHP:  // 无重载
来源：http://hz.daria6918.cn/gthooozaew.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.feifeiyinyue.top/gtlxttlipb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yonumen.top/gtqjmpeawr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinqigfzy.top/gtobmwpzdp.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtwvfqbwlc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtixqsmypj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yonumen.top/gtjmwzfnzp.html

================================================================================
来源：http://hz.svipenyu.cn/gtmlpqfxqh.html

D. 数组 / 列表 / 集合
来源：http://hz.hysaishi.cn/gtijriimnd.html

================================================================================
来源：http://hz.yangfankeji.com/gtpdjdwmko.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtpkblmaro.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hywenlv.cn/gttryisyfe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangkeji.top/gtrlnhkedp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtwqzjuwhs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jiagoushi.top/gtdauohlnd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gtvtiuxupe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtsugiqmio.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guowangkeji.top/gthlzmqwdv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gttohuvmqy.html

[D02] 追加元素到末尾
来源：http://hz.haohaochexian.top/gttcubqlqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtlgourwkw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gtrweqfpkg.html

JS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtjuqjtwyc.html

TS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtahotlkgy.html

Java: list.add(4);
来源：http://hz.kuanghao11.cn/gtbjxwskpa.html

Go:   arr = append(arr, 4)
来源：http://hz.aizwys.cn/gtdocqfahg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.mhx1999.top/gtqwdnqgyb.html

C#:   list.Add(4);
来源：http://hz.ydjk.org.cn/gtonqxwtgj.html

[D03] 在指定位置插入元素
来源：http://hz.gogol.net.cn/gtbkedzyej.html

Py:   arr.insert(0, 0)
来源：http://hz.dashuyun.cn/gtmdarxkqk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gtgzvdyndn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hongshengwenyu.top/gtwczcnrmu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtdjkwmgxl.html

Java: list.add(0, 0);
来源：http://hz.shuidangran.top/gthfhfprvz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtofxnprsd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gotoacloud.top/gtlnfgpqmx.html

C#:   list.Insert(0, 0);
来源：http://hz.gzhubu.top/gtjbavhqby.html

[D04] 删除元素
来源：http://hz.ywan-chungtsiang.top/gtilamqhkl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cheryme.top/gtviygiznp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtmrbrbnav.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtlsvestrn.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258888.top/gtgzwkxffl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.bjfxy.top/gtwymncpdc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtefiiwsqq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhiwuduotai.top/gtbyemtgjk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtroteazex.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gtfdeoyndr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gttiictutf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sysykeji.top/gtmcnioczp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtopmjfrse.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinghuilouyu.cn/gttefqhbbl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhoulong.xyz/gtlaoksmyt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtzklzollv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtxzzmthnv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yangfankeji.com/gtrnqahush.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtikvwbmyz.html

Py:   len(arr)
来源：http://hz.havefunace.top/gtxwkzgzat.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtnswljoit.html

JS:   arr.length
来源：http://hz.meibo888.top/gtwrngdzzv.html

TS:   arr.length
来源：http://hz.quarkkingdee.top/gtlunhegdi.html

Java: list.size();
来源：http://hz.aizwys.cn/gtnvvmyilj.html

Go:   len(arr)
来源：http://hz.dashuyun.cn/gtabzhxujw.html

Ruby: arr.length; arr.size
来源：http://hz.nanxinkj.top/gtzogwtbio.html

C#:   list.Count;
来源：http://hz.yj20258.top/gtbcurygnc.html


<!-- 参考信息 -->