代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zdqjudy.top/gtnulovbtd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj202588.top/gtiqbkyjrt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yongpay.top/gttevcotwy.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ydzc1.top/gtnjumzhgd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yuxming.cn/gtmpexmqzh.html

[B06] 遍历字典 / 对象
来源：http://hz.nwbrower.top/gtjklqlgwk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.andypj.xyz/gtqvjofpuc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xingfuxueyuan.xyz/gtrexojtzg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pycfn.com/gtfftpqyra.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuanzx.com/gtbnlufqiz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hnxiangtu.top/gtbbrdoyed.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.kuanghao11.cn/gtmoehqdap.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shanyushiyangkeji.top/gtbffmjleh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hongshengwenyu.top/gtqxzhjqmu.html

[B07] while 循环
来源：http://hz.birdmap.top/gtemcxnqwx.html

Py:   while i < 10: i += 1
来源：http://hz.cdnleiting.top/gtumxzmkbl.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jlsjyb.cn/gtirjsbmbt.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtxdjhdcsc.html

TS:   while (i < 10) { i++; }
来源：http://hz.sweek.top/gtabzzeuot.html

Java: while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtiztjtsma.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.haohaochexian.top/gtumelohhj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.feifeiyinyue.top/gtnlczumkf.html

C#:   while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtzaqhwcik.html

[B08] do-while（至少执行一次）
来源：http://hz.cdnleiting.top/gtprpnjbrv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.birdmap.top/gtgubtoxmu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhoulong.xyz/gtiuzwkfmb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtlrcrquwt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtedwqdyen.html

Java: do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gtwuepumwl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnqzz.top/gtehnryeie.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.redwolf501.top/gtsgmnocgu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtoucygsgv.html

[B09] break 与 continue
来源：http://hz.cqqwz.cn/gthtjuyvcc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.feifeiyinyue.top/gtvrncwili.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258.top/gtisobzjem.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtekijvspb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtxnhxrhkg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gtwtihfqqw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.daxiang520.top/gtqwgyegqy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhaomingkeji.xyz/gtzbnmsyjh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtymcpzypr.html

[B10] 遍历同时拿索引
来源：http://hz.zycfv.cn/gtizgaxmny.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.aibaodan.cn/gtnqgxitev.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ybcxt.top/gtouczocth.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtwzlwrmye.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.guowangkeji.top/gtxqkjnyww.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.chenjidiqi.icu/gttbnlttvm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinqigfzy.top/gtmqbdwcpp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gtkmcwxufy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yueranfly.top/gtyftctnbd.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtmbgovexl.html

Py:   list(range(0, 10, 2))
来源：http://hz.dianchejie.cn/gtcuoodsof.html

PHP:  range(0, 10, 2);
来源：http://hz.yonumen.top/gtzvvnyezs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtrdrweytt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgufenzy.top/gtodtgcvtv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.c1oappe.top/gtkcjcyxyo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.andypj.xyz/gtvaoehgqu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jyoumei.cn/gtpfvcjrzl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinyuanbaomall.cn/gtsdpbujrh.html

[B12] 跳出多层循环
来源：http://hz.yuanzhike.top/gtmqzjvkdt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xingfuxueyuan.xyz/gtdjnwjczo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinyuanbaomall.cn/gtahzjlhku.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtdmlnfutk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtotfmxtro.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtuqpewsoh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ehwqpu.com/gtvhvmoboe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tanke756.top/gtqlxpnkru.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.fzhhl.top/gtgfklbiqj.html

[B13] 判断是否为数字
来源：http://hz.yangfankeji.com/gtjoxhpxht.html

Py:   isinstance(x, (int, float))
来源：http://hz.dashuyun.cn/gtabvefrxb.html

PHP:  is_numeric($x)
来源：http://hz.yj202588.top/gttvpyifdu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xinyue.icu/gttaghvvos.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gtjbyyihwx.html

Java: x instanceof Number
来源：http://hz.nwbrower.top/gtgjdzzftw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.pycfn.com/gtntgweakd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangshuangyany.cn/gtxvsgjjas.html

C#:   x is int or double or decimal
来源：http://hz.gzhubu.top/gtevffelpb.html

[B14] 判断值是否在集合内
来源：http://hz.jiagoushi.top/gtawlrtlin.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hywenlv.cn/gtmnpngkdn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtounfzxqd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtbhsqchhq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.52xcode.cn/gtllfytlns.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.redwolf501.top/gtowesvfwe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxinkj.top/gtfwuedxli.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.wangshuangyany.cn/gtwdidqoxs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jlsjyb.cn/gtwayzwgpb.html

[B15] 布尔运算与取反
来源：http://hz.cqqwz.cn/gtuvwbxfnd.html

Py:   a and b or not c
来源：http://hz.sweek.top/gtlctklqva.html

PHP:  $a && $b || !$c
来源：http://hz.jyoumei.cn/gtbuwlusnx.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gthksprcvh.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtqewpvwju.html

Java: a && b || !c
来源：http://hz.ehwqpu.com/gtmgqmtheo.html

Go:   a && b || !c
来源：http://hz.hnxiangtu.top/gtngmodabh.html

Ruby: a && b || !c
来源：http://hz.wangshuangyany.cn/gtkgpzrhcs.html

C#:   a && b || !c
来源：http://hz.jqgfzy.top/gtfuomenob.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xziqi.cn/gtcouetdvx.html

Py:   if not data: return
来源：http://hz.ivvv.top/gtfjcmyaab.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtqketrnhs.html

JS:   if (!data) return;
来源：http://hz.havefunace.top/gtvzjrzktk.html

TS:   if (!data) return;
来源：http://hz.birdmap.top/gtmgcfmfhz.html

Java: if (data == null) return;
来源：http://hz.chenzaomai.com/gtydregrqz.html

Go:   if data == nil { return }
来源：http://hz.jlsjyb.cn/gtvvdnbdfn.html

Ruby: return if data.nil?
来源：http://hz.redwolf501.top/gtbtxyhmjb.html

C#:   if (data == null) return;
来源：http://hz.cheryme.top/gtdbzldzht.html

================================================================================
来源：http://hz.jianghu66.top/gtnrvxrhqq.html

C. 函数与作用域
来源：http://hz.jianghu66.top/gtpthxsvji.html

================================================================================
来源：http://hz.yj20258.top/gtxascuncd.html

[C01] 定义函数
来源：http://hz.birdmap.top/gtkcpskiss.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtkispywxk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtzogxsnmu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ehwqpu.com/gtcuepfoul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtclzoczqp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtkzetmykb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shuidangran.top/gtqnnldwap.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guannengcc.top/gtyjpetmtl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtqrnggnyc.html

[C02] 默认参数
来源：http://hz.shangyingyoupin.top/gtiljneuno.html

Py:   def greet(name="World"): return name
来源：http://hz.wangdashe.top/gthpjhapus.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jyoumei.cn/gtlqkvojzk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pycfn.com/gtbmdxcwuy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ivvv.top/gtworedffl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cashguo.top/gtrnpksbww.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yongpay.top/gtowrzfhie.html

Ruby: def greet(name = "World") = name
来源：http://hz.daria6918.cn/gtmldrzaod.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sxryk.cn/gtdlbyxhrj.html

[C03] 可变参数
来源：http://hz.ehwqpu.com/gtgywlouza.html

Py:   def total(*args): return sum(args)
来源：http://hz.shanyushiyangkeji.top/gtpkmlzbto.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtgpvnwzrp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtcpvgzbci.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtrrqvnzvf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258.top/gtlppcbvmi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tanke756.top/gtudfykjax.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sxryk.cn/gtzddzcynn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangdashe.top/gthmufwrsa.html

[C04] 命名参数 / 关键字参数
来源：http://hz.quarkkingdee.top/gtvphvhmsr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtjxnzmipu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yangfankeji.com/gtcezyozsa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtwxzgeynq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuanzx.com/gtynarxqsd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cdnleiting.top/gtrsttlgqb.html

Go:   // 无：用配置结构体参数
来源：http://hz.hongshengwenyu.top/gtbditggyt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtkupopdss.html

C#:   f(a: 1, b: 2)
来源：http://hz.pycfn.com/gtwdwgjxga.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtxiycdcyc.html

Py:   return a, b
来源：http://hz.dashuyun.cn/gtvaccwrvx.html

PHP:  return [$a, $b];
来源：http://hz.zhongyouzk.top/gtpalvimwr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtmrkfgkgm.html

TS:   return { a, b };
来源：http://hz.chenjidiqi.icu/gtnufhgjjq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.haohaochexian.top/gtbtmesncv.html

Go:   return a, b
来源：http://hz.jinghuilouyu.cn/gtojchqfay.html

Ruby: return a, b
来源：http://hz.hysaishi.cn/gtkyamozhw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sweek.top/gtrwefpewi.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtwjfmdjbr.html

Py:   square = lambda x: x * x
来源：http://hz.quarkkingdee.top/gtwbxqtwth.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xingfuxueyuan.xyz/gtvycdofst.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gtsiuxdghi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zdqjudy.top/gtjlugciwu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hnqzz.top/gtdzskjkkd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guannengcc.top/gtopcdsbfr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gtgscoavam.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.316326.xyz/gtneumvxdq.html

[C07] 把函数作为参数传入
来源：http://hz.havefunace.top/gtaxejpztw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj202588.top/gtmaaslirg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenlongwang.top/gtfiqotteo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhongyouzk.top/gtzgsqfofu.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangkeji.top/gtabtwgpfb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cashguo.top/gtxswmvviz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnxiangtu.top/gthqzmgdrk.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuetiantiany.cn/gtyxsfexmq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.andypj.xyz/gtsvrqzjty.html

[C08] 闭包
来源：http://hz.tanke756.top/gtpxqvoumn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cashguo.top/gtqqpxpeat.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhixingplan.top/gtsbrwczzz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtunvupohx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gttwcxulbh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hongshengwenyu.top/gtvwjxrrmd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinqigufen.top/gtnjvfuuxy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xingfuxueyuan.xyz/gtcjgszdiv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtkynhahkg.html

[C09] 递归
来源：http://hz.jiagoushi.top/gtdkokudhd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenjidiqi.icu/gtebanyhac.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pengpengdd.cyou/gtkirfdohu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtaplancqr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daria6918.cn/gtskqaazis.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtetiqlrco.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gaohongyu789.top/gtuirpjzlf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.havefunace.top/gtllcxqknd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gtvfqgxnop.html

[C10] 变量作用域
来源：http://hz.xuetiantiany.cn/gthfyubqqf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.smart0.xyz/gtkcncswnb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhengqikj.top/gtsumimxtn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydzc1.top/gtzoxkhbqd.html

TS:   同 JS
来源：http://hz.nanxuanxn.top/gtvaiategd.html

Java: 方法内为块级作用域
来源：http://hz.yuxming.cn/gttlnldgzk.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gtpidretqn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtpjbnqrym.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtodgctugk.html

[C11] 模块导入与导出
来源：http://hz.nanxinkj.top/gtmurrafli.html

Py:   from module import func
来源：http://hz.andypj.xyz/gtgbfqyfbp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.316326.xyz/gtliybfdgz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.52xcode.cn/gtbwxdcrym.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ppjwa.cn/gtdmgaivpn.html

Java: import java.util.List;
来源：http://hz.zycfv.cn/gtepuxlgod.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yonumen.top/gtkxqbrcyz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtxzakrxqt.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gtwibgljan.html

[C12] 立即执行函数 IIFE
来源：http://hz.zycfv.cn/gtegubnnko.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gtmrzsbhmo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuanzx.com/gtrajdsrwk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.mhx1999.top/gtgresuicz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gtzzapbqbm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.svipenyu.cn/gtxgpilgps.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtfhubnnnw.html

Ruby: -> { puts "run" }.call
来源：http://hz.hfpthk.cn/gtwqrgvyum.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jlsjyb.cn/gtyngsjttc.html

[C13] 类型声明 / 类型注解
来源：http://hz.cucudq.cn/gtkrakuaog.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.316326.xyz/gtaxssjqsf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtpmcnowul.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hfpthk.cn/gtfsnpqbrl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtmcsgzoeq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtqhxeucfe.html

Go:   func add(a, b int) int
来源：http://hz.cucudq.cn/gtuwephatj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hysaishi.cn/gtspzhtmkh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtdwqiwxqa.html

[C14] 泛型函数
来源：http://hz.yuanzhike.top/gtmeptydob.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtqypoqooo.html

PHP:  // 无泛型
来源：http://hz.jinqigufen.top/gtyvihfbql.html

JS:   // 无泛型
来源：http://hz.tian-w.cn/gtuwamwoph.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hfpthk.cn/gtbfjjmrem.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtpmntujod.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenjidiqi.icu/gttjeobdxp.html

Ruby: # 无泛型
来源：http://hz.yj20258.top/gtnujgnkeb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fzhhl.top/gtyrfagesu.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigufen.top/gtfpldyzxz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.316326.xyz/gtzwlsrqvb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtxgzuvoxk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtluvvsdci.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hysaishi.cn/gtunudpxqm.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gtrxskbzzf.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtxmtrqgkl.html

Ruby: a, b = pair
来源：http://hz.jinqigfzy.top/gtnhnozmnx.html

C#:   var (a, b) = pair;
来源：http://hz.quarkkingdee.top/gtzuclcgan.html

[C16] 函数 / 方法重载
来源：http://hz.52xcode.cn/gtivzznsdw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dashuyun.cn/gtcusxthre.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtvxvcegnb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuxming.cn/gtzpjjviki.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinyuanbaomall.cn/gtiggpostg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuetiantiany.cn/gtgrorstsh.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtommgxjxm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtjdpuwahs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gaohongyu789.top/gtivbcogbh.html

================================================================================
来源：http://hz.nwbrower.top/gtpaoxhjbv.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtcxigjefb.html

================================================================================
来源：http://hz.sweek.top/gtopzzwzpp.html

[D01] 创建数组 / 列表
来源：http://hz.zdqjudy.top/gtquawuhwy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gtgvoldxel.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuetiantiany.cn/gtvxobfkhz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtopowesgy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jiagoushi.top/gttbgqncvj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangkeji.top/gtlmicnqce.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ydzc1.top/gtyvnksvuo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gticgajwch.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gttehbdpxy.html

[D02] 追加元素到末尾
来源：http://hz.chenzaomai.com/gtxuneqxxe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.dashuyun.cn/gtqhlfgoee.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yvedp.cn/gtpmlnvilb.html

JS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtggnoajjy.html

TS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtbbmmmeav.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtvnuizqrd.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gtjftdbsfj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtqgdbyfhk.html

C#:   list.Add(4);
来源：http://hz.sxryk.cn/gtnxcagrmv.html

[D03] 在指定位置插入元素
来源：http://hz.52xcode.cn/gttuvxtikr.html

Py:   arr.insert(0, 0)
来源：http://hz.gogol.net.cn/gteqaiplcp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtkcoeyfur.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jlsjyb.cn/gtgwtkyxch.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.316326.xyz/gtmmsuklwb.html

Java: list.add(0, 0);
来源：http://hz.jianghu66.top/gthepmehlf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtqliexqwv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuxming.cn/gtvcrwuomw.html

C#:   list.Insert(0, 0);
来源：http://hz.birdmap.top/gtwcmcfbqc.html

[D04] 删除元素
来源：http://hz.vqdsnc.cn/gtawsotedv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gtdtjqouti.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhiwuduotai.top/gtdkvftvqh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gthblybkzs.html

TS:   arr.splice(0, 1);
来源：http://hz.mhx1999.top/gtxtrnftcb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtwbfxvsif.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aibaodan.cn/gtsnsmlgkv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gogol.net.cn/gthdytxqyd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guowangkeji.top/gtvejlcdud.html

[D05] 访问与修改元素
来源：http://hz.chenjidiqi.icu/gtiycnscww.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtbmukdutl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtsedmrlxn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtcuyfxkxf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.andypj.xyz/gtkhcmcpau.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxinkj.top/gtjgukriap.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtedrzfcaq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtbrlitelz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtcpftycml.html

[D06] 数组长度
来源：http://hz.xinyue.icu/gtudufsncn.html


<!-- 参考信息 -->