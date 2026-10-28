代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sxryk.cn/gtwiphqcme.html

[B06] 遍历字典 / 对象
来源：http://hz.zhixingplan.top/gtmoaogubw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ehwqpu.com/gtccyjewap.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.smart0.xyz/gttbyssutb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgfzy.top/gtsyenerma.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtwnnpdfsb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.birdmap.top/gthyqvbwge.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cashguo.top/gthbceasan.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.bjfxy.top/gtrijwlcnr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.bjfxy.top/gtltcmfyfn.html

[B07] while 循环
来源：http://hz.vqdsnc.cn/gtbfcrvatg.html

Py:   while i < 10: i += 1
来源：http://hz.ivvv.top/gtudssbyzj.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xuetiantiany.cn/gtthioaqpl.html

JS:   while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gtwttiiaad.html

TS:   while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gtoyggvpip.html

Java: while (i < 10) { i++; }
来源：http://hz.cqqwz.cn/gtuzwyfddb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hysaishi.cn/gtcolpdfqj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xuetiantiany.cn/gtmdqeijsx.html

C#:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtsxulmxbb.html

[B08] do-while（至少执行一次）
来源：http://hz.ydjk.org.cn/gttymbqfqp.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.tanke756.top/gtrrtqevbs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ehwqpu.com/gttwjnfpmc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gtlaskgwyp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtvozxrfmy.html

Java: do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtgufpswiz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jqgufenzy.top/gtwtgqccod.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xuetiantiany.cn/gtdtyhqohy.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtkvjdkdrp.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gtbxgzbuae.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.iojbl.cn/gtftqwsode.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sweek.top/gtgzgaooma.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtrrkccwmx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gtxqooqffl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtlqjnhyem.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cheryme.top/gtspbfehvy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.316326.xyz/gtcbacqkww.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtkirgzdxq.html

[B10] 遍历同时拿索引
来源：http://hz.shzxlz.cn/gtwswqwozt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.pengpengdd.cyou/gtcsegcmmo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtjrzglvch.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.redwolf501.top/gtdrcehymf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangkeji.top/gtxkgfypvc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhaomingkeji.xyz/gtnuivssfl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sufxvd.cn/gtzkikwikk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zycfv.cn/gtiqzvadhu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinyuanbaomall.cn/gtbdzsrdia.html

[B11] 生成数字序列 / 区间
来源：http://hz.hysaishi.cn/gtcxuglofv.html

Py:   list(range(0, 10, 2))
来源：http://hz.ydjk.org.cn/gtyturkohv.html

PHP:  range(0, 10, 2);
来源：http://hz.52xcode.cn/gttkohjgww.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangtech.top/gtfxkpufcp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cdnleiting.top/gtkrtebcrg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yvedp.cn/gtmfzdrprr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinyuanbaomall.cn/gtrhcdbcwu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cheryme.top/gtnecjpsxh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nanxinkj.top/gtxvufmaqs.html

[B12] 跳出多层循环
来源：http://hz.zhongyouzk.top/gtkvtocurp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.vqdsnc.cn/gtojmgfmrz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shuidangran.top/gtrsymzokb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtbqloxvxx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtdfzmnofw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtejsypkyd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shangyingyoupin.top/gtigjetglx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cqqwz.cn/gtjnwqmywi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gzhubu.top/gtpzctfggh.html

[B13] 判断是否为数字
来源：http://hz.shanyushiyangtech.top/gtydrlcnyn.html

Py:   isinstance(x, (int, float))
来源：http://hz.xingfuxueyuan.xyz/gtawunfhsd.html

PHP:  is_numeric($x)
来源：http://hz.zhixingplan.top/gtlyuodpor.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtxukazlmg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtrrochhko.html

Java: x instanceof Number
来源：http://hz.zycfv.cn/gtyrrsrmne.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sufxvd.cn/gteuwspzla.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ydzc1.top/gtmaqrjspe.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtoebxuiif.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtcrtjngxs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.kuanghao11.cn/gtnxmjnoeg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj20258888.top/gtsfmrqlhj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ywan-chungtsiang.top/gtzkzozbsy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.kuanghao11.cn/gtmmjbhmcr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhixingplan.top/gtofismqxb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.havefunace.top/gthjvsoclv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gotoacloud.top/gtadvdkedw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj20258.top/gtyqqawrca.html

[B15] 布尔运算与取反
来源：http://hz.feifeiyinyue.top/gtwmnhzbut.html

Py:   a and b or not c
来源：http://hz.ydjk.org.cn/gtyvbbzyvg.html

PHP:  $a && $b || !$c
来源：http://hz.zhongyouzk.top/gtevpltyje.html

JS:   a && b || !c
来源：http://hz.daria6918.cn/gtbxwgnlwn.html

TS:   a && b || !c
来源：http://hz.smart0.xyz/gtsggevvji.html

Java: a && b || !c
来源：http://hz.chenzaomai.com/gtyceznrkr.html

Go:   a && b || !c
来源：http://hz.kuanghao11.cn/gtubfselrw.html

Ruby: a && b || !c
来源：http://hz.sysykeji.top/gtmzheklov.html

C#:   a && b || !c
来源：http://hz.jqgfzy.top/gtinaouhcf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.316326.xyz/gtqcfxrmvh.html

Py:   if not data: return
来源：http://hz.xingfuxueyuan.xyz/gtdvptptrr.html

PHP:  if (!$data) { return; }
来源：http://hz.ywan-chungtsiang.top/gtmwrzkxzs.html

JS:   if (!data) return;
来源：http://hz.vqdsnc.cn/gtjwyeztvh.html

TS:   if (!data) return;
来源：http://hz.fengsongda.top/gtzpoetyle.html

Java: if (data == null) return;
来源：http://hz.gotoacloud.top/gtkonfjqbb.html

Go:   if data == nil { return }
来源：http://hz.nanxinkj.top/gtyjqnlfys.html

Ruby: return if data.nil?
来源：http://hz.yj20258.top/gtwwkrtfrz.html

C#:   if (data == null) return;
来源：http://hz.gotoacloud.top/gteinmznue.html

================================================================================
来源：http://hz.snrcjt.cn/gtasvehxkd.html

C. 函数与作用域
来源：http://hz.0kj1m.cn/gtvwrpjrvk.html

================================================================================
来源：http://hz.daria6918.cn/gtbgrhuofx.html

[C01] 定义函数
来源：http://hz.guowangkeji.top/gtdahyhvgn.html

Py:   def add(a, b): return a + b
来源：http://hz.zdqjudy.top/gtrktrnuwm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtpzzumgru.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnqzz.top/gtiibcgndg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtjmxudjgx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtfwlkgtmi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.quarkkingdee.top/gtpmivovqj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtevxmvcvv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtwnvfmzdw.html

[C02] 默认参数
来源：http://hz.zhengqikj.top/gtapplstsk.html

Py:   def greet(name="World"): return name
来源：http://hz.jinghuilouyu.cn/gttctokbuv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yangfankeji.com/gtyfbtfbit.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtufsljxab.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dashuyun.cn/gtdrkdfaca.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ehwqpu.com/gtkwmnvykh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gtbmfptucp.html

Ruby: def greet(name = "World") = name
来源：http://hz.ywan-chungtsiang.top/gtvreoiiru.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.pengpengdd.cyou/gtzdsbagpm.html

[C03] 可变参数
来源：http://hz.gogol.net.cn/gtaypxwykt.html

Py:   def total(*args): return sum(args)
来源：http://hz.cucudq.cn/gtfzkzyhql.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigfzy.top/gtwjwswyyc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtcecozaog.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtbpyocnqm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cucudq.cn/gtxmpowrip.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nwbrower.top/gtqocljvho.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aizwys.cn/gtzhujjotf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guannengcc.top/gtghbkybmu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtyghixymw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shzxlz.cn/gtyxzgzkzz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aizwys.cn/gtcmvugfiw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtmbooxssy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinyuanbaomall.cn/gtmaptvyxf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gtbdoxqfek.html

Go:   // 无：用配置结构体参数
来源：http://hz.sxryk.cn/gtxlcivcyw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtchujcvkn.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtsvquuted.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtquqntvpo.html

Py:   return a, b
来源：http://hz.yueranfly.top/gtfrienlix.html

PHP:  return [$a, $b];
来源：http://hz.snrcjt.cn/gtvfyucume.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tianlin.xyz/gttkqocpbj.html

TS:   return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtcgdrrdah.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sysykeji.top/gtxtgcxfla.html

Go:   return a, b
来源：http://hz.cqqwz.cn/gtzqbtcesc.html

Ruby: return a, b
来源：http://hz.jiagoushi.top/gtdludiqea.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yueranfly.top/gtvazmtntk.html

[C06] 匿名函数 / lambda
来源：http://hz.zycfv.cn/gtjcefxhvd.html

Py:   square = lambda x: x * x
来源：http://hz.andypj.xyz/gtytrcpaih.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sweek.top/gtesjbbesp.html

JS:   const square = x => x * x;
来源：http://hz.yj20258888.top/gtokcubmuk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guannengcc.top/gtxbhinmif.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ppjwa.cn/gtxttoslzn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangkeji.top/gtszzjqjez.html

Ruby: square = ->(x) { x * x }
来源：http://hz.quarkkingdee.top/gtgtgijakx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydzc1.top/gtsxjqxzsv.html

[C07] 把函数作为参数传入
来源：http://hz.sysykeji.top/gtgncdhynw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tian-w.cn/gtpjyycvrr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cucudq.cn/gtsistwods.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhongyouzk.top/gtjjuinzjz.html

TS:   arr.map(String)
来源：http://hz.zhaomingkeji.xyz/gtinlfyoby.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangkeji.top/gtfozzzmmw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.52xcode.cn/gtxggxgzxt.html

Ruby: arr.map(&:upcase)
来源：http://hz.yangfankeji.com/gtbzpzmtrh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daria6918.cn/gtpnpdwsai.html

[C08] 闭包
来源：http://hz.wangdashe.top/gtgqdgqzdy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cucudq.cn/gtrshyvhai.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xylfe.cn/gtouvswxdl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtetypsviy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtueiembkq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gaohongyu789.top/gtoevqelih.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuxming.cn/gtfnxumxsr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sweek.top/gtlbfsiluc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtmugrwtlv.html

[C09] 递归
来源：http://hz.yonumen.top/gtgdxwkzta.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.havefunace.top/gtzctmxxrc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tianlin.xyz/gtaebqzotg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtzvojfehx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtfecryifa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.quarkkingdee.top/gtqestxeoo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jyoumei.cn/gtwqhlnbuc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtvhghpgcl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangshuangyany.cn/gttradyssd.html

[C10] 变量作用域
来源：http://hz.yuanzhike.top/gtoczkqtor.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.kuanghao11.cn/gtfsewcwqq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.smart0.xyz/gtakzzlujy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj202588.top/gtjhwqoqxj.html

TS:   同 JS
来源：http://hz.cucudq.cn/gtjuetniiq.html

Java: 方法内为块级作用域
来源：http://hz.yongpay.top/gtiqxwavnc.html

Go:   花括号块级作用域
来源：http://hz.nanxuanxn.top/gtdojcbfxi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xylfe.cn/gtlrtxvewy.html

C#:   块级作用域
来源：http://hz.iojbl.cn/gtpywzlzee.html

[C11] 模块导入与导出
来源：http://hz.pycfn.com/gtbkvssjnk.html

Py:   from module import func
来源：http://hz.guannengcc.top/gthjufaycb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gzhubu.top/gtqdkjhsav.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtdetlgahr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtdyjiefkx.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gtoyzfduek.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtavpxdiwt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhaomingkeji.xyz/gtkwgnfhnl.html

C#:   using System.Text;
来源：http://hz.xuanzx.com/gtxldjdhsz.html

[C12] 立即执行函数 IIFE
来源：http://hz.ybcxt.top/gtbrgknowl.html

Py:   (lambda: print("run"))()
来源：http://hz.52xcode.cn/gtvyatsofk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.quarkkingdee.top/gtshdvcxfh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtigkbqhnh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cashguo.top/gtqynvinzi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtqzxzydnl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xingfuxueyuan.xyz/gtsseypniv.html

Ruby: -> { puts "run" }.call
来源：http://hz.sysykeji.top/gtotsksavx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pycfn.com/gtkivhieso.html

[C13] 类型声明 / 类型注解
来源：http://hz.andypj.xyz/gtcfbeapcf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gtofhqiwbp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtydpocmsl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shzxlz.cn/gtglnrdjjg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtqcuezuwu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtufbskjua.html

Go:   func add(a, b int) int
来源：http://hz.zhijiandao.cn/gthqrghkdw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gthkiekbkb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtqqmndxpf.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gttcctnygo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.haohaochexian.top/gthtrllrdr.html

PHP:  // 无泛型
来源：http://hz.jinqigfzy.top/gtjdmwszxw.html

JS:   // 无泛型
来源：http://hz.yanxiufei.cn/gthrxfvnrs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daxiang520.top/gttsfggoco.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sweek.top/gtegzaxovg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ivvv.top/gtndxnxfjz.html

Ruby: # 无泛型
来源：http://hz.hongshengwenyu.top/gtvbsfknez.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hammf.cn/gtovzwieec.html

[C15] 解构 / 展开参数
来源：http://hz.guannengcc.top/gtbohchurv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.vqdsnc.cn/gtflbvbpdb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.9152youxi.cn/gtxkhkdsdk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtdxwcbgzq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yongpay.top/gtprspyvng.html

Java: // 无解构
来源：http://hz.guowangkeji.top/gtmsacpcum.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtyzzqopxe.html

Ruby: a, b = pair
来源：http://hz.jlsjyb.cn/gtnktskgyc.html

C#:   var (a, b) = pair;
来源：http://hz.ehwqpu.com/gturuocqny.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtwmhneqgu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtrsqhkttp.html

PHP:  // 无重载
来源：http://hz.jinqigfzy.top/gtwljmtgvv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gtptdtqiav.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shangyingyoupin.top/gtbsdzliya.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gthsnrusdk.html

Go:   // 无重载：用不同函数名
来源：http://hz.mhx1999.top/gtsrrznskj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.havefunace.top/gtfezrrbxw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.316326.xyz/gtzqscxbkf.html

================================================================================
来源：http://hz.gotoacloud.top/gtxqzvcxzs.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigfzy.top/gtpdqequix.html

================================================================================
来源：http://hz.hnxiangtu.top/gttgbbqbxa.html

[D01] 创建数组 / 列表
来源：http://hz.pengpengdd.cyou/gtcfttpgsz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.haohaochexian.top/gthfdtqdoi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtwujjuqpk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shzxlz.cn/gtrdwnpwdu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinyuanbaomall.cn/gttbqbyvhn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.andypj.xyz/gtwbovtero.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.snrcjt.cn/gtypbouozo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hammf.cn/gtycrkkdwe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shuidangran.top/gttdmlatuw.html

[D02] 追加元素到末尾
来源：http://hz.9152youxi.cn/gtziytdcef.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnqzz.top/gtekjzxuwa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.snrcjt.cn/gtjisokdfe.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtwaxdxlnj.html

TS:   arr.push(4);
来源：http://hz.fzhhl.top/gtdwbjvejc.html

Java: list.add(4);
来源：http://hz.zycfv.cn/gtvvvztpae.html

Go:   arr = append(arr, 4)
来源：http://hz.cashguo.top/gtugbldtkq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydzc1.top/gtoftqynkf.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtambszvtq.html

[D03] 在指定位置插入元素
来源：http://hz.aizwys.cn/gtouafvesb.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtqtbkeszx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gzhubu.top/gtabwmaees.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtdaedrewg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenlongwang.top/gtpymslvxj.html

Java: list.add(0, 0);
来源：http://hz.zhixingplan.top/gtxixngqkw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shuidangran.top/gtezyunbpo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gtwyebaoij.html

C#:   list.Insert(0, 0);
来源：http://hz.hysaishi.cn/gtybzipccn.html

[D04] 删除元素
来源：http://hz.zdqjudy.top/gthqppjztk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtkyufsiqj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pengpengdd.cyou/gtntmljjdo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.smart0.xyz/gtngtxscvl.html

TS:   arr.splice(0, 1);
来源：http://hz.haohaochexian.top/gtwrfpmxrl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinghuilouyu.cn/gtloxwrxvb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnqzz.top/gthzcreksc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fengsongda.top/gtmztdcxbo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gttoglsfhy.html

[D05] 访问与修改元素
来源：http://hz.haohaochexian.top/gtwpcvfkqr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtiqkcsjml.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gtndrskbwu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cdnleiting.top/gtnudrnuyk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydzc1.top/gtrlgrkfyr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shzxlz.cn/gtzxvbfoaq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtkatujrqu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtpmobmfxy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.bjfxy.top/gtbaqjnvka.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtfborbbrb.html

Py:   len(arr)
来源：http://hz.svipenyu.cn/gtjvtpdkpg.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtrshwdfpa.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtoorqrhyr.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtfdnbbkev.html


<!-- 参考信息 -->