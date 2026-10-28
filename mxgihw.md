代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.fengsongda.top/gtwgczxzkn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.daria6918.cn/gtwsgkjiba.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hongshengwenyu.top/gtxzujqwux.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.snrcjt.cn/gtwmeqjkhk.html

[B05] 遍历数组 / 列表
来源：http://hz.zhixingplan.top/gtgkyzyyst.html

Py:   for item in arr: print(item)
来源：http://hz.xziqi.cn/gtfjbvsocq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.kuanghao11.cn/gtnrvjijgy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shuidangran.top/gtkjdufkyw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.guowangkeji.top/gtdzgrstgc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xylfe.cn/gtyficxmgw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhongyouzk.top/gtjyizxiqc.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj202588.top/gterzjywrw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jlsjyb.cn/gtgxpysyqp.html

[B06] 遍历字典 / 对象
来源：http://hz.vqdsnc.cn/gtmejldnzx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cashguo.top/gtxsuxjzqn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yvedp.cn/gtzegmqkvg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgufenzy.top/gtteyjpmja.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.andypj.xyz/gtohmcpqwx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinqigfzy.top/gteztygxtf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhiwuduotai.top/gthxgfvvfd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hysaishi.cn/gthgcpcvxe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.c1oappe.top/gtvajtglxx.html

[B07] while 循环
来源：http://hz.jiagoushi.top/gtmvxochzg.html

Py:   while i < 10: i += 1
来源：http://hz.iojbl.cn/gtikzrollq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xylfe.cn/gtytrqudjk.html

JS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtekfhbwyc.html

TS:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtcbgctzlu.html

Java: while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtfttnbcyd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj20258888.top/gtcrdetzwb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtcnykrnyo.html

C#:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gttikdjnmn.html

[B08] do-while（至少执行一次）
来源：http://hz.chenzaomai.com/gtxtbwsiyh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.meibo888.top/gttnpcffma.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenzaomai.com/gtxyxyrtme.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gtctfvqpkw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtgtpchxkn.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtjuymjuhj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ppjwa.cn/gtskzmzkkr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xylfe.cn/gtkfurrlng.html

C#:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtniryncos.html

[B09] break 与 continue
来源：http://hz.bjfxy.top/gtqecxfsze.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydjk.org.cn/gtltagyztr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xylfe.cn/gtdfxvuccc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtuqmcczsu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtqwsrwezd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtqsmtrisi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hysaishi.cn/gtlibywefw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenjidiqi.icu/gtypvmjelt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gteuqajmaw.html

[B10] 遍历同时拿索引
来源：http://hz.yueranfly.top/gtoaysmlkz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.316326.xyz/gtoewbhemr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shzxlz.cn/gtoedbnaaz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ppjwa.cn/gthkbsarvc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hfpthk.cn/gtqgqkcxqi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yvedp.cn/gtoxdtpflk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinqigufen.top/gtwyfvpusa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenzaomai.com/gtmkptxgyq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.birdmap.top/gtkxkjvuef.html

[B11] 生成数字序列 / 区间
来源：http://hz.316326.xyz/gtzxskuqxw.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtriggjzjj.html

PHP:  range(0, 10, 2);
来源：http://hz.ehwqpu.com/gtlrwqcsvz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigufen.top/gtoedeewbg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ywan-chungtsiang.top/gtvksajrwj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj20258888.top/gtfexwnjdc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ywan-chungtsiang.top/gtcuxpugmk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.bjfxy.top/gtfcuvvkuh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenjidiqi.icu/gtbkidxcey.html

[B12] 跳出多层循环
来源：http://hz.hywenlv.cn/gtuciikluq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.svipenyu.cn/gtloteusqn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ydzc1.top/gtcxqmiajs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtzgrliuee.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtjkjuaabq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtxzxdfyvd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtgeujlujk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258.top/gthvucfxls.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.quarkkingdee.top/gtdrytdges.html

[B13] 判断是否为数字
来源：http://hz.xingfuxueyuan.xyz/gtspgfupzu.html

Py:   isinstance(x, (int, float))
来源：http://hz.tianlin.xyz/gtzbvnfljg.html

PHP:  is_numeric($x)
来源：http://hz.ybcxt.top/gtgwnfydmw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.kuanghao11.cn/gtxuhalefj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ppjwa.cn/gtnzelvtop.html

Java: x instanceof Number
来源：http://hz.gzhubu.top/gtfsliywke.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cashguo.top/gthvrvlnbt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daxiang520.top/gtxqpxmwoi.html

C#:   x is int or double or decimal
来源：http://hz.tian-w.cn/gtbtprtaxr.html

[B14] 判断值是否在集合内
来源：http://hz.jqgufenzy.top/gtuowwphhm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dashuyun.cn/gteigtsyoe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.vqdsnc.cn/gtdumtnlgv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gthelhhrsq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtrmqxqitj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guowangkeji.top/gtvmhqohka.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hongshengwenyu.top/gtltjawlgt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.aizwys.cn/gtizdxhxcv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.wangdashe.top/gtgbxknvbc.html

[B15] 布尔运算与取反
来源：http://hz.fzhhl.top/gtaviuqmzg.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtkrldmamt.html

PHP:  $a && $b || !$c
来源：http://hz.cheryme.top/gtfzwldlvt.html

JS:   a && b || !c
来源：http://hz.ppjwa.cn/gtcbsstagw.html

TS:   a && b || !c
来源：http://hz.cashguo.top/gtssoiyecp.html

Java: a && b || !c
来源：http://hz.vqdsnc.cn/gtifbtuhlf.html

Go:   a && b || !c
来源：http://hz.aibaodan.cn/gtmgrperqg.html

Ruby: a && b || !c
来源：http://hz.ppjwa.cn/gtvsikfddx.html

C#:   a && b || !c
来源：http://hz.hfpthk.cn/gtaiwhhzlm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.mhx1999.top/gtibyxrqzl.html

Py:   if not data: return
来源：http://hz.fengsongda.top/gtpkzuqkki.html

PHP:  if (!$data) { return; }
来源：http://hz.yanxiufei.cn/gtuzdsacsy.html

JS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtplkpsnrl.html

TS:   if (!data) return;
来源：http://hz.zycfv.cn/gtygnealhc.html

Java: if (data == null) return;
来源：http://hz.bjfxy.top/gtsywtlypk.html

Go:   if data == nil { return }
来源：http://hz.cdnleiting.top/gtwyipxibi.html

Ruby: return if data.nil?
来源：http://hz.yuanzhike.top/gtjsdfpdiq.html

C#:   if (data == null) return;
来源：http://hz.ybcxt.top/gtkcdfgklq.html

================================================================================
来源：http://hz.zycfv.cn/gtgifjjjvb.html

C. 函数与作用域
来源：http://hz.jiagoushi.top/gthiwrrewh.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwahkyvhv.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gtvzomvntf.html

Py:   def add(a, b): return a + b
来源：http://hz.wangdashe.top/gtyjfpjscy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtzmqspslg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nwbrower.top/gtgppbuuic.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtuelmnhia.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtfcdnoucq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gogol.net.cn/gtyxpjgfeo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shuidangran.top/gtjgulgoca.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtrouadmpv.html

[C02] 默认参数
来源：http://hz.cheryme.top/gtugtawfgx.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gtshbvqico.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shanyushiyangtech.top/gtxjawvces.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.quarkkingdee.top/gtruszqaxv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shzxlz.cn/gtgoncebiw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yvedp.cn/gtrsapdcik.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jianghu66.top/gtxdggyhni.html

Ruby: def greet(name = "World") = name
来源：http://hz.iojbl.cn/gtuboohnmq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xingfuxueyuan.xyz/gtetzcoluu.html

[C03] 可变参数
来源：http://hz.cqqwz.cn/gtcrsossyx.html

Py:   def total(*args): return sum(args)
来源：http://hz.hywenlv.cn/gtlpbvoiib.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtzrapeysk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.9152youxi.cn/gtuclkqibn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xziqi.cn/gtcjvqgynd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtdjyerabv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.guowangkeji.top/gthzdknrxj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.haohaochexian.top/gtxcstfuwb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gaohongyu789.top/gtmgbjibzq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gtpaxpsiyj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxuanxn.top/gtnvaejehk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gtruauqnly.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.svipenyu.cn/gthubajwdr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shzxlz.cn/gttagsvoio.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ybcxt.top/gtcrdnyqof.html

Go:   // 无：用配置结构体参数
来源：http://hz.hfpthk.cn/gtentrnoui.html

Ruby: f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtcazmmorc.html

C#:   f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtxcmxwvjs.html

[C05] 返回多个值
来源：http://hz.smart0.xyz/gtlmtbknoo.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtnkunknnt.html

PHP:  return [$a, $b];
来源：http://hz.fzhhl.top/gttoipjirm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangshuangyany.cn/gtxgeafxmg.html

TS:   return { a, b };
来源：http://hz.jinghuilouyu.cn/gtsupmxtqv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinqigufen.top/gtytonuxig.html

Go:   return a, b
来源：http://hz.jyoumei.cn/gtgqfwkyiy.html

Ruby: return a, b
来源：http://hz.jinyuanbaomall.cn/gtnimdzpjr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuanzx.com/gtxifjphme.html

[C06] 匿名函数 / lambda
来源：http://hz.yj20258.top/gtmnvcovrr.html

Py:   square = lambda x: x * x
来源：http://hz.xziqi.cn/gtaksjjfgq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sxryk.cn/gtawfvhrzw.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gticovpzdh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtleuvjrib.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yangfankeji.com/gtlfjnzqrp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ehwqpu.com/gtiwpdirnf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jyoumei.cn/gtupxkrtsl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jlsjyb.cn/gtkzxyvarx.html

[C07] 把函数作为参数传入
来源：http://hz.zhixingplan.top/gtpmaqrprj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj202588.top/gtxbzdtfuk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.vqdsnc.cn/gthvvqhnsj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhaomingkeji.xyz/gtetvbkvfw.html

TS:   arr.map(String)
来源：http://hz.zdqjudy.top/gthilkcyrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhoulong.xyz/gtbiykfvag.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtleuxwrtw.html

Ruby: arr.map(&:upcase)
来源：http://hz.kuanghao11.cn/gtueunoppn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jyoumei.cn/gtfyhsuwhn.html

[C08] 闭包
来源：http://hz.tanke756.top/gtricxlfdu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtryisrolf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sysykeji.top/gtpafvcwib.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtjkcqguov.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtjzrnqmgo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.mhx1999.top/gtsufckoey.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guannengcc.top/gtzzulmeww.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinyuanbaomall.cn/gtoivzmxgb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtyfaehspc.html

[C09] 递归
来源：http://hz.chenzaomai.com/gtoozcwyds.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtrvisiexi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gtjnhupcco.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtemypnjmj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtqtfrxish.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pycfn.com/gtsfixliki.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yuanzhike.top/gttueelqxq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtifrtkgmd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sxryk.cn/gtlpxzwulh.html

[C10] 变量作用域
来源：http://hz.redwolf501.top/gtvejjamxd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhongyouzk.top/gtjvehyoim.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgufenzy.top/gtxrpfoohr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtknuvacat.html

TS:   同 JS
来源：http://hz.jianghu66.top/gtmnfmbzaf.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gtgvsqsozl.html

Go:   花括号块级作用域
来源：http://hz.haohaochexian.top/gtojtqsdvt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnqzz.top/gtgynfjhwy.html

C#:   块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtgppiobeu.html

[C11] 模块导入与导出
来源：http://hz.guowangkeji.top/gtjazkejnf.html

Py:   from module import func
来源：http://hz.jqgfzy.top/gtueywwnbo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tian-w.cn/gtdszewuxs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtarrjldjn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jianghu66.top/gtwpblyjaa.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtsppcdbqo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cashguo.top/gtbvhawuxm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shangyingyoupin.top/gtcfxwqpmr.html

C#:   using System.Text;
来源：http://hz.gzhubu.top/gttasmzjtz.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj202588.top/gtiagpxsrm.html

Py:   (lambda: print("run"))()
来源：http://hz.vqdsnc.cn/gtghizoune.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ivvv.top/gtblenvqvh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinyuanbaomall.cn/gtkrtphryr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtfrsokoxm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tian-w.cn/gtvmlhavje.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtmbyttczf.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gtxoamtngq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.iojbl.cn/gtcjmjnvcm.html

[C13] 类型声明 / 类型注解
来源：http://hz.birdmap.top/gttwcewasr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtlsbmpzia.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtqdvzdtej.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtrptnzspw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtoyjlstfe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ivvv.top/gtyzbshfcx.html

Go:   func add(a, b int) int
来源：http://hz.jinqigufen.top/gtkurydrik.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhongyouzk.top/gtselhuffr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhoulong.xyz/gtmdjwkrfl.html

[C14] 泛型函数
来源：http://hz.yuxming.cn/gtudarnhpg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtweoqavbd.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtjjuzlico.html

JS:   // 无泛型
来源：http://hz.yangfankeji.com/gtlnkqgzra.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.wangdashe.top/gtmjcazdhc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.andypj.xyz/gtodgasjcy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gtvezhaxzc.html

Ruby: # 无泛型
来源：http://hz.cashguo.top/gtccckdiqq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zdqjudy.top/gtqxawsunu.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gttgytcxtk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.dianchejie.cn/gtfsljgglk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pengpengdd.cyou/gtdmbjdszw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtuqfnnvyf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daxiang520.top/gtgnxbrapo.html

Java: // 无解构
来源：http://hz.aizwys.cn/gtddlxmrrj.html

Go:   // 无解构
来源：http://hz.hywenlv.cn/gtufntxgjn.html

Ruby: a, b = pair
来源：http://hz.redwolf501.top/gtzuljhhzj.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangtech.top/gthpizuxgf.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtklzwujsd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtznqdblio.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtssplshcy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nwbrower.top/gtxtlcnttd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gthxzgsunt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ppjwa.cn/gthkfvdukj.html

Go:   // 无重载：用不同函数名
来源：http://hz.gogol.net.cn/gttdrkxbto.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhengqikj.top/gtcrvdgazz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yangfankeji.com/gtixhlgoqy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtuzlgmpco.html

D. 数组 / 列表 / 集合
来源：http://hz.yonumen.top/gtnqlgtieo.html

================================================================================
来源：http://hz.aizwys.cn/gtmdyzlgqd.html

[D01] 创建数组 / 列表
来源：http://hz.svipenyu.cn/gtelldponm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.9152youxi.cn/gtoynnvgbq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gogol.net.cn/gtaeirdmum.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daxiang520.top/gtapdoklvn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinyuanbaomall.cn/gttvvdnahs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gtdsfrlovw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.kuanghao11.cn/gtuwxlvqwy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtrriexmes.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tianlin.xyz/gtskbafcve.html

[D02] 追加元素到末尾
来源：http://hz.sxryk.cn/gthjsihrfs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtfaxkhnso.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gotoacloud.top/gtcseewutx.html

JS:   arr.push(4);
来源：http://hz.316326.xyz/gthtxeiynq.html

TS:   arr.push(4);
来源：http://hz.jinqigufen.top/gtvpyrmlwt.html

Java: list.add(4);
来源：http://hz.shanyushiyangkeji.top/gtsliegmxa.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gtibvyohsv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cheryme.top/gtjbxrxlgk.html

C#:   list.Add(4);
来源：http://hz.gotoacloud.top/gtqnmblsed.html

[D03] 在指定位置插入元素
来源：http://hz.tianlin.xyz/gtmhfwylrf.html

Py:   arr.insert(0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtxlsliiys.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtrnptcgto.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuxming.cn/gtirtpdmkh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtiiizkysq.html

Java: list.add(0, 0);
来源：http://hz.fzhhl.top/gtqryakmui.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jianghu66.top/gtfljpxull.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ybcxt.top/gtiqpsjzjd.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangtech.top/gtpevneflj.html

[D04] 删除元素
来源：http://hz.fengsongda.top/gtjwbhrahk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtcklfkyvs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hammf.cn/gtqrtdhkdq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtejmefwms.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgfzy.top/gtymnrspnw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtdbpflkjz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jianghu66.top/gtmitjdwfc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gtieliocsd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gtvtansrte.html

[D05] 访问与修改元素
来源：http://hz.hnxiangtu.top/gtppgszkzy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gtcrotodmu.html


<!-- 参考信息 -->