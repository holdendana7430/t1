代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.316326.xyz/gtssqywudq.html

[B06] 遍历字典 / 对象
来源：http://hz.jianghu66.top/gtspzqvtpq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sxryk.cn/gteckrsqpf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hnqzz.top/gtmiwgnyzi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cdnleiting.top/gtscyrrdoo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gtodmjtfrj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.havefunace.top/gtxdpdwxwq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.52xcode.cn/gtqtquqhmf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.birdmap.top/gtcoyjqbtx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guowangkeji.top/gtvqrigwkw.html

[B07] while 循环
来源：http://hz.yj20258.top/gtdpwqksmt.html

Py:   while i < 10: i += 1
来源：http://hz.meibo888.top/gtxoegumvo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ppjwa.cn/gtozjtpjnn.html

JS:   while (i < 10) { i++; }
来源：http://hz.dashuyun.cn/gtjnegnocs.html

TS:   while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gthkxvjbgi.html

Java: while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtzrbpejre.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xinyue.icu/gtddntzdgp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhaomingkeji.xyz/gtztegxhes.html

C#:   while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gtngdtirfd.html

[B08] do-while（至少执行一次）
来源：http://hz.jinyuanbaomall.cn/gtcqoupcvf.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sufxvd.cn/gtsvjgeigj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.quarkkingdee.top/gtkilooksw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtdfaoqfwj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtaoxtmlkz.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtvcgidkza.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj20258888.top/gtgovhefik.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yonumen.top/gtfehkprik.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtggopigea.html

[B09] break 与 continue
来源：http://hz.gogol.net.cn/gtprstcvwc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zdqjudy.top/gtwajsqgtc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.bjfxy.top/gtiptelnpy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtkqrfifir.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtduafduym.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gthvjnnmtm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yanxiufei.cn/gtwjwxudgp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gttisdfsse.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtbnmvpqrt.html

[B10] 遍历同时拿索引
来源：http://hz.nanxinkj.top/gtlbzkxxfm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.iojbl.cn/gtbfpjistz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yongpay.top/gtsujiunsl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sysykeji.top/gtymigipbr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.guannengcc.top/gtvgvgvgux.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hnxiangtu.top/gtvjghgwou.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinqigfzy.top/gtknjlikqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhaomingkeji.xyz/gtrdjjhagl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cheryme.top/gtvnkofhvc.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenlongwang.top/gtemgjawkh.html

Py:   list(range(0, 10, 2))
来源：http://hz.jinqigfzy.top/gtbyleiolo.html

PHP:  range(0, 10, 2);
来源：http://hz.jlsjyb.cn/gtekjikplo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxuanxn.top/gtytjqqach.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenlongwang.top/gtmsmteuwm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.pycfn.com/gtlubtetnz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj202588.top/gtvpxkbegx.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gotoacloud.top/gtummnjuiq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ydjk.org.cn/gtmfumkjyy.html

[B12] 跳出多层循环
来源：http://hz.ppjwa.cn/gtsnwcmhsm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xuetiantiany.cn/gtfwmuncwo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cashguo.top/gtcqaxrexv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtpnmgzclz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gtseqyxtre.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtclxzggqb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cucudq.cn/gtvfgifyfo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhiwuduotai.top/gtiufqadta.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.316326.xyz/gthkouyrvy.html

[B13] 判断是否为数字
来源：http://hz.hnxiangtu.top/gtmotqvyvw.html

Py:   isinstance(x, (int, float))
来源：http://hz.aibaodan.cn/gtbxtdzegk.html

PHP:  is_numeric($x)
来源：http://hz.meibo888.top/gtkdsnfjhw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gtjowzogzz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtfyqohnmk.html

Java: x instanceof Number
来源：http://hz.jinghuilouyu.cn/gtkiubwdpr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ivvv.top/gthokkiqbo.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pengpengdd.cyou/gtpybfkzfs.html

C#:   x is int or double or decimal
来源：http://hz.cqqwz.cn/gtdegifixg.html

[B14] 判断值是否在集合内
来源：http://hz.vqdsnc.cn/gtlokefrky.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuanzx.com/gtsmtlnvuq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.meibo888.top/gtwqdrkfuy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtmtfgjvzg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.52xcode.cn/gtixgqkuxe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.chenjidiqi.icu/gtiketzvmt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinyuanbaomall.cn/gtkwektdcg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuxming.cn/gtchlxiamb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenzaomai.com/gtpmrbtahv.html

[B15] 布尔运算与取反
来源：http://hz.chenjidiqi.icu/gtmakdxbur.html

Py:   a and b or not c
来源：http://hz.havefunace.top/gtequaqdku.html

PHP:  $a && $b || !$c
来源：http://hz.pycfn.com/gtuojabykf.html

JS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtnypgpvaq.html

TS:   a && b || !c
来源：http://hz.aizwys.cn/gtuvutwcyn.html

Java: a && b || !c
来源：http://hz.zhongyouzk.top/gtrfjxleud.html

Go:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtrzlzxeta.html

Ruby: a && b || !c
来源：http://hz.zhengqikj.top/gtlyfigmiy.html

C#:   a && b || !c
来源：http://hz.jqgfzy.top/gtcovfkokg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shuidangran.top/gtooqyewni.html

Py:   if not data: return
来源：http://hz.havefunace.top/gtxrhnnakz.html

PHP:  if (!$data) { return; }
来源：http://hz.aibaodan.cn/gtqdzmwysv.html

JS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtjjuizvps.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtxvhrprpz.html

Java: if (data == null) return;
来源：http://hz.ydjk.org.cn/gtkeadmzew.html

Go:   if data == nil { return }
来源：http://hz.cdnleiting.top/gtqlwgpxng.html

Ruby: return if data.nil?
来源：http://hz.tian-w.cn/gtvzfzahae.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtuqcwylwp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvuphyuna.html

C. 函数与作用域
来源：http://hz.gogol.net.cn/gtetlsrzpa.html

================================================================================
来源：http://hz.yvedp.cn/gtovwitdjg.html

[C01] 定义函数
来源：http://hz.yuanzhike.top/gthwraidsm.html

Py:   def add(a, b): return a + b
来源：http://hz.xuetiantiany.cn/gtmkemhgrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtktemdpvz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.meibo888.top/gtdvpjeafm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtqvvpsffw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtbrpqmcet.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.0kj1m.cn/gtptdwmdjs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.aibaodan.cn/gtzispvrht.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtwwckxajq.html

[C02] 默认参数
来源：http://hz.ehwqpu.com/gtldwforib.html

Py:   def greet(name="World"): return name
来源：http://hz.chenjidiqi.icu/gtgtqgppva.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhijiandao.cn/gthfzgkmzv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zdqjudy.top/gttpduywxb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuxming.cn/gtyirydgrr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gaohongyu789.top/gtngevkblv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenlongwang.top/gtvbgzanlu.html

Ruby: def greet(name = "World") = name
来源：http://hz.yj202588.top/gtowhfxfvm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gtlcdzjyya.html

[C03] 可变参数
来源：http://hz.jinqigufen.top/gtlnidgvgg.html

Py:   def total(*args): return sum(args)
来源：http://hz.meibo888.top/gteqnqtitt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xziqi.cn/gtmluvvfla.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhixingplan.top/gtczkoqsdo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtldkmwurk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtauqbhxpd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenlongwang.top/gtlrkqucbi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xinyue.icu/gtvsedavub.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtrxjlkiux.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtssrortjn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sweek.top/gtxhvzdosh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cheryme.top/gtvxvgiosv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtytrnhtsz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtmmwyhlmb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ppjwa.cn/gtgymtlhft.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhaomingkeji.xyz/gtcxuuctxb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtmqpzirmk.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtewxxiubz.html

[C05] 返回多个值
来源：http://hz.bjfxy.top/gttuxdwcci.html

Py:   return a, b
来源：http://hz.jianghu66.top/gtphshlpnv.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtwxzqtely.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guowangkeji.top/gtmuseojzd.html

TS:   return { a, b };
来源：http://hz.nwbrower.top/gthvghihyg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.kuanghao11.cn/gtqvuuqidk.html

Go:   return a, b
来源：http://hz.ivvv.top/gtjjfaqmuc.html

Ruby: return a, b
来源：http://hz.xylfe.cn/gtqimlkfqw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jqgufenzy.top/gtimlrwgkj.html

[C06] 匿名函数 / lambda
来源：http://hz.zhoulong.xyz/gtodtpsdte.html

Py:   square = lambda x: x * x
来源：http://hz.guowangkeji.top/gtrbczmeng.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sufxvd.cn/gtoxvldnfa.html

JS:   const square = x => x * x;
来源：http://hz.aizwys.cn/gtgtnaceyr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guannengcc.top/gtlbarvrym.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtsyidsqkl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.smart0.xyz/gtzbgoflhe.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jlsjyb.cn/gtbjuczwoc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.daxiang520.top/gtvhnvfrvo.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gtbqliifhq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jianghu66.top/gthosaacdd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenlongwang.top/gthcbpizuy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtvphgurax.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangkeji.top/gtomxdgikf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinghuilouyu.cn/gtvguffcub.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hywenlv.cn/gticotiart.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj202588.top/gtrjyqfmrz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nwbrower.top/gtweilvmjm.html

[C08] 闭包
来源：http://hz.guannengcc.top/gtxxlznraj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gtihbdvqiu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuanzx.com/gtvlloojnm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtzexydnrc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtylzatuyt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhengqikj.top/gttvbbvlkx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guowangkeji.top/gtmyjrccgg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gtadphfjil.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtulmvuomh.html

[C09] 递归
来源：http://hz.9152youxi.cn/gtowlxeplf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jiagoushi.top/gthfhjrlod.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xylfe.cn/gtbprfbzpn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tianlin.xyz/gtnkihfjzc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtufykyeci.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cashguo.top/gtejerbafs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gaohongyu789.top/gtaycykeet.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtikimpeog.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ybcxt.top/gtwuhylgbc.html

[C10] 变量作用域
来源：http://hz.andypj.xyz/gtzddobcbq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.meibo888.top/gtjjgquauq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ybcxt.top/gtvyuzhntx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yueranfly.top/gtwdegxnbe.html

TS:   同 JS
来源：http://hz.sxryk.cn/gttvgzxuiv.html

Java: 方法内为块级作用域
来源：http://hz.tanke756.top/gtvhmtxdzo.html

Go:   花括号块级作用域
来源：http://hz.yongpay.top/gtohjfqbrj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuetiantiany.cn/gtekmnmaor.html

C#:   块级作用域
来源：http://hz.hnqzz.top/gtjimgbsit.html

[C11] 模块导入与导出
来源：http://hz.nanxuanxn.top/gtoqmspdwl.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtyslsdjfa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.smart0.xyz/gtdpocsnib.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtpxkuskdm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinghuilouyu.cn/gtbawdlrup.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtseunofvt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.52xcode.cn/gtrwqzfnza.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.0kj1m.cn/gtehynekwa.html

C#:   using System.Text;
来源：http://hz.daxiang520.top/gtyqyjiahr.html

[C12] 立即执行函数 IIFE
来源：http://hz.feifeiyinyue.top/gtrlfavbia.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtncvzhsmx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhoulong.xyz/gtkdnqjffr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtjugdtjhi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtudztoiwk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtwiqfjqtt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhoulong.xyz/gtifctkrkl.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangkeji.top/gtcpupqtrj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangkeji.top/gttngnfrjw.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtmbshwwee.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.iojbl.cn/gtyfqzaqsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtnimrshgy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tanke756.top/gtpwfjujiz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.iojbl.cn/gtxcbfveif.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtgxhbreqj.html

Go:   func add(a, b int) int
来源：http://hz.ywan-chungtsiang.top/gtocytoynv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhongyouzk.top/gtnnmbdhau.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhengqikj.top/gtfvgfdbbc.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtqeqddabs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.havefunace.top/gtthhrytij.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtrpvzghod.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gtwxiimbfj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenjidiqi.icu/gtomwizcqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtnzxkzudq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hysaishi.cn/gtcdmckjsg.html

Ruby: # 无泛型
来源：http://hz.feifeiyinyue.top/gtvguegjtn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cucudq.cn/gtaoecixsi.html

[C15] 解构 / 展开参数
来源：http://hz.meibo888.top/gtjpzijzbt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fengsongda.top/gthjetgbfm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.meibo888.top/gtodmlndma.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtsrjnmppb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jqgfzy.top/gtcoahziqp.html

Java: // 无解构
来源：http://hz.shangyingyoupin.top/gthjzbbhzp.html

Go:   // 无解构
来源：http://hz.tanke756.top/gtaatyyzab.html

Ruby: a, b = pair
来源：http://hz.chenlongwang.top/gtjhvyxhtl.html

C#:   var (a, b) = pair;
来源：http://hz.0kj1m.cn/gteambfjld.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gtiwwuqbkz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtmbwtzbye.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gtyezxaqvj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangkeji.top/gtdvodwrmj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gtbccedcvr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cheryme.top/gtemcmvcyb.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangshuangyany.cn/gtsoqnvzpb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gtpsxltnjc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxinkj.top/gtfdclogwi.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjxhycqzo.html

D. 数组 / 列表 / 集合
来源：http://hz.yangfankeji.com/gtooxinxjp.html

================================================================================
来源：http://hz.sufxvd.cn/gtyzwudhwf.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtzyiteark.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sweek.top/gtroqynoav.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnxiangtu.top/gtysvhmztb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ivvv.top/gtiotmelvt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtecugokyf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtpzndabgu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.smart0.xyz/gtawdgqgvy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtzeraezin.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtpfjecvzn.html

[D02] 追加元素到末尾
来源：http://hz.52xcode.cn/gtgbvdddfn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fengsongda.top/gtjhkrfnvo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sysykeji.top/gtqvwremah.html

JS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtjzwawpvz.html

TS:   arr.push(4);
来源：http://hz.cucudq.cn/gtsykdvwey.html

Java: list.add(4);
来源：http://hz.xziqi.cn/gtntxumjrc.html

Go:   arr = append(arr, 4)
来源：http://hz.daria6918.cn/gtncldpdnq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yvedp.cn/gtpgixiqkp.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtlqpwcbsb.html

[D03] 在指定位置插入元素
来源：http://hz.shuidangran.top/gtoakzuioo.html

Py:   arr.insert(0, 0)
来源：http://hz.yj202588.top/gtehvvkoni.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gaohongyu789.top/gtolpcqenz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hywenlv.cn/gtwlbciifs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ybcxt.top/gtyokcqnpe.html

Java: list.add(0, 0);
来源：http://hz.gaohongyu789.top/gtsayrhybc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gtbjiuuchf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shangyingyoupin.top/gtasfafevx.html

C#:   list.Insert(0, 0);
来源：http://hz.ivvv.top/gtsfiildxs.html

[D04] 删除元素
来源：http://hz.yueranfly.top/gtgsgbjmlw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtbltlautj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.smart0.xyz/gtdbffrrbb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtefxbmmjq.html

TS:   arr.splice(0, 1);
来源：http://hz.smart0.xyz/gtfafvxeqj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cdnleiting.top/gtbbswmann.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ehwqpu.com/gtwwjnimqm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.0kj1m.cn/gtbiewjskq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtmczmqvwl.html

[D05] 访问与修改元素
来源：http://hz.chenlongwang.top/gtosueulhx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtukksvndf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtzsbvmzlz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.52xcode.cn/gtysamxwnn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cheryme.top/gtjterzhud.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gthqgtnhgu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtipcwdoib.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtmjsnbqmk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.9152youxi.cn/gtmutlysrl.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtojcczrhf.html

Py:   len(arr)
来源：http://hz.jianghu66.top/gtewgzwwgt.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtfigyuuqq.html

JS:   arr.length
来源：http://hz.zhongyouzk.top/gtamcjhaxl.html

TS:   arr.length
来源：http://hz.meibo888.top/gtaomgvcwl.html


<!-- 参考信息 -->