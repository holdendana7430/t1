代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuxming.cn/gtgvmjqurp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigufen.top/gthtrxzyxw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.daria6918.cn/gtbjryhocv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jinqigufen.top/gtdnfogerr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yueranfly.top/gtwcbkmhhq.html

[B06] 遍历字典 / 对象
来源：http://hz.kuanghao11.cn/gtkerwcyxz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.52xcode.cn/gtzesaglmw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.iojbl.cn/gtcvwecmuv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinghuilouyu.cn/gtsswzehby.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuxming.cn/gthyqrvqok.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenlongwang.top/gtclsgkhof.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shanyushiyangkeji.top/gtvmcmkozq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nwbrower.top/gtnjgluqdt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhoulong.xyz/gttemscbku.html

[B07] while 循环
来源：http://hz.zycfv.cn/gttnmhcqhc.html

Py:   while i < 10: i += 1
来源：http://hz.snrcjt.cn/gtbaazirgj.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.dashuyun.cn/gtktiqbjoy.html

JS:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtjppqhlvl.html

TS:   while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtiqhpsjqn.html

Java: while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtairmvaoz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cqqwz.cn/gtbwnrbgbu.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nanxinkj.top/gtfoquoyqu.html

C#:   while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gtadfjxfzu.html

[B08] do-while（至少执行一次）
来源：http://hz.jinqigufen.top/gtndikyjgy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cashguo.top/gtdgqvjksa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.feifeiyinyue.top/gtkuusbdkq.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtvzmfhbdj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtfxcvlycl.html

Java: do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtddnswpng.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.c1oappe.top/gtiaifctcu.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xuetiantiany.cn/gtqhiknvyp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gttvcbgwpc.html

[B09] break 与 continue
来源：http://hz.zdqjudy.top/gtelmyjerv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.quarkkingdee.top/gtdbrwnxpj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.fengsongda.top/gteskyrzpk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtajdqrguj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtrvolrerp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtnofjytef.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yanxiufei.cn/gtgwklawmv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtohqwevbf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gttwmjtnti.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigufen.top/gttpjdeqfq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guowangkeji.top/gtyuqtowiq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cqqwz.cn/gtskdvzluc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.316326.xyz/gtffcoeaqr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tanke756.top/gtwxrogxaz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yonumen.top/gthdiumhsc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.svipenyu.cn/gtyhyifknv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cqqwz.cn/gtxiaafjwc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinyuanbaomall.cn/gtsgyxvwbs.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgufenzy.top/gtupqzcccr.html

Py:   list(range(0, 10, 2))
来源：http://hz.hfpthk.cn/gtbmqvwxmk.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gtfvzsyslf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuanzx.com/gtyfehhumq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ywan-chungtsiang.top/gtetdstmre.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yvedp.cn/gtnfgxktuf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gttoecgzwy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yangfankeji.com/gtoakoreyd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtjruhwnlh.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangtech.top/gtdodofpka.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cdnleiting.top/gtxkrfrdcx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shanyushiyangkeji.top/gtloyxicql.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtujtebwwy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtgaptgyqc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtyyeexfxx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtqypzxoah.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ywan-chungtsiang.top/gtwjhxhily.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shanyushiyangkeji.top/gtqukwyotq.html

[B13] 判断是否为数字
来源：http://hz.xingfuxueyuan.xyz/gtaopajbkn.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigfzy.top/gtnquzjnps.html

PHP:  is_numeric($x)
来源：http://hz.jiagoushi.top/gtywvloufd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xingfuxueyuan.xyz/gtijprsohf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtacdeyzab.html

Java: x instanceof Number
来源：http://hz.dashuyun.cn/gtbcgcarpo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ydjk.org.cn/gtlmdhuscc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cashguo.top/gtaduumazm.html

C#:   x is int or double or decimal
来源：http://hz.wangshuangyany.cn/gtpcvvzens.html

[B14] 判断值是否在集合内
来源：http://hz.yj202588.top/gtqrhfbgzp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cucudq.cn/gtexrfuulw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtlyaehxkw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtwrpkqxqu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gtiskkhzes.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cqqwz.cn/gttkrirdfi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nwbrower.top/gtgpdvzdge.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nanxuanxn.top/gtrwryxhbg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hywenlv.cn/gtqlukwqku.html

[B15] 布尔运算与取反
来源：http://hz.sysykeji.top/gtttmpwgmg.html

Py:   a and b or not c
来源：http://hz.birdmap.top/gthmycvpnk.html

PHP:  $a && $b || !$c
来源：http://hz.sweek.top/gtjqchicyd.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtwtlcworf.html

TS:   a && b || !c
来源：http://hz.daxiang520.top/gtnvpgubgi.html

Java: a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtohpusvqo.html

Go:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtqjwezyxk.html

Ruby: a && b || !c
来源：http://hz.meibo888.top/gtvstuztrt.html

C#:   a && b || !c
来源：http://hz.hnxiangtu.top/gtcndzahzo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangshuangyany.cn/gtdsltlpiv.html

Py:   if not data: return
来源：http://hz.cqqwz.cn/gtsnuiiefb.html

PHP:  if (!$data) { return; }
来源：http://hz.tanke756.top/gtgekoagun.html

JS:   if (!data) return;
来源：http://hz.hammf.cn/gtankpfyhs.html

TS:   if (!data) return;
来源：http://hz.wangdashe.top/gtxhnhgwsj.html

Java: if (data == null) return;
来源：http://hz.ywan-chungtsiang.top/gtpgzmvxzx.html

Go:   if data == nil { return }
来源：http://hz.hywenlv.cn/gtfkogzqha.html

Ruby: return if data.nil?
来源：http://hz.vqdsnc.cn/gtxqksmfmr.html

C#:   if (data == null) return;
来源：http://hz.yanxiufei.cn/gthhaayyki.html

================================================================================
来源：http://hz.yuxming.cn/gtnnkqikrm.html

C. 函数与作用域
来源：http://hz.xinyue.icu/gtyhmphylu.html

================================================================================
来源：http://hz.shuidangran.top/gtugjpxmkh.html

[C01] 定义函数
来源：http://hz.snrcjt.cn/gtyynkjegv.html

Py:   def add(a, b): return a + b
来源：http://hz.hnqzz.top/gtrjprmlsl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtvqkumtub.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gttxljauzk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtummexbyr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtnlbdvjos.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtxhsoveoa.html

Ruby: def add(a, b); a + b; end
来源：http://hz.kuanghao11.cn/gtiqvtrzgv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gttgojlzin.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtlktnmmhj.html

Py:   def greet(name="World"): return name
来源：http://hz.tanke756.top/gtftbmuvpq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tian-w.cn/gtrjebwiro.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258888.top/gtafmajena.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gtorzxsvca.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gotoacloud.top/gtnieawvjj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.haohaochexian.top/gtsbgtfcsv.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuxming.cn/gtyymrpzsu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ydjk.org.cn/gtnokdnxrf.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gtyaxtkomg.html

Py:   def total(*args): return sum(args)
来源：http://hz.hywenlv.cn/gtkiuviqro.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gttcnadqwi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtjotgmcyz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtxhuttdlc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zycfv.cn/gtxoxpohxn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtmldgyphm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jqgfzy.top/gtzarbrnns.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jianghu66.top/gtjizwzrvu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ehwqpu.com/gtfillqgur.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtewhiiwsq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangdashe.top/gtlnyixcfp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtkuptiijj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenzaomai.com/gtgtdllhkj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daria6918.cn/gtcideabjl.html

Go:   // 无：用配置结构体参数
来源：http://hz.kuanghao11.cn/gtxzbfgxaj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtdzixrwpo.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtozxkgnra.html

[C05] 返回多个值
来源：http://hz.mhx1999.top/gtgflbcpvz.html

Py:   return a, b
来源：http://hz.gzhubu.top/gtdjobfymo.html

PHP:  return [$a, $b];
来源：http://hz.fzhhl.top/gtkkeeyekw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenzaomai.com/gtooxgaxhd.html

TS:   return { a, b };
来源：http://hz.smart0.xyz/gtptrskhlv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxuanxn.top/gtizkauqbi.html

Go:   return a, b
来源：http://hz.yvedp.cn/gtfxnqfaih.html

Ruby: return a, b
来源：http://hz.sweek.top/gtkesotkjp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jqgfzy.top/gtpjccshgc.html

[C06] 匿名函数 / lambda
来源：http://hz.jinghuilouyu.cn/gtazcfrgbg.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtnzawicnh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.feifeiyinyue.top/gtkypsywrq.html

JS:   const square = x => x * x;
来源：http://hz.aibaodan.cn/gtofcatbaf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.smart0.xyz/gtsyqathzv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtosuacswd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.havefunace.top/gtznmllixx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xinyue.icu/gtjgznmrgs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nwbrower.top/gtargqqrcx.html

[C07] 把函数作为参数传入
来源：http://hz.c1oappe.top/gthwdinqbl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.redwolf501.top/gtobbbtxat.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tianlin.xyz/gtpjakstqz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gtlexugtse.html

TS:   arr.map(String)
来源：http://hz.xingfuxueyuan.xyz/gthefryhia.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnxiangtu.top/gtivkfgqez.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ybcxt.top/gthzeafbeh.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangkeji.top/gtaaupcmhd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhiwuduotai.top/gtgbgwgbgm.html

[C08] 闭包
来源：http://hz.jinqigufen.top/gtfnnsfcwo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.haohaochexian.top/gtmhkpeija.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shuidangran.top/gtebfyurov.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtewzpgbir.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtcxlvlmcq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhongyouzk.top/gtzjaonsnx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yonumen.top/gtgrwklcau.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinqigufen.top/gtsdfgjhxk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtqmwfknjr.html

[C09] 递归
来源：http://hz.316326.xyz/gthzqpsykz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnqzz.top/gtqhlxkxak.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.wangdashe.top/gtjjyfrzvk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gtxsjextko.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gteealhwqa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgufenzy.top/gtvnxfpivx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.wangshuangyany.cn/gthimtpkou.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtqqwzwysl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gtirzoumqy.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtjowiypmi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.smart0.xyz/gtdccrzdzt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nwbrower.top/gtjwlczcqk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hywenlv.cn/gtzntcdtju.html

TS:   同 JS
来源：http://hz.shzxlz.cn/gtydvpbsoe.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtifuzflux.html

Go:   花括号块级作用域
来源：http://hz.yuxming.cn/gtpgpxsbwq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yuanzhike.top/gtlhoenlmz.html

C#:   块级作用域
来源：http://hz.pycfn.com/gtxnuqvlhp.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gtctzczcep.html

Py:   from module import func
来源：http://hz.jianghu66.top/gtpvtaycuv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtiehbearn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenzaomai.com/gtsoypttdl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.dashuyun.cn/gtbwgxjjmo.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gttueskirf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.birdmap.top/gtlxsbqtpy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtmwprjmbz.html

C#:   using System.Text;
来源：http://hz.yongpay.top/gtxvojljfh.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtudtzvfhk.html

Py:   (lambda: print("run"))()
来源：http://hz.cashguo.top/gtdgkazyoh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guowangkeji.top/gtshsxeljh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhiwuduotai.top/gtafwrzmzt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtovzpnxrd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zycfv.cn/gtwwtojsgb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gteimgpnta.html

Ruby: -> { puts "run" }.call
来源：http://hz.ywan-chungtsiang.top/gtrodosbnj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtzcvqorvx.html

[C13] 类型声明 / 类型注解
来源：http://hz.gaohongyu789.top/gtwwpfhend.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhoulong.xyz/gttfbolsbq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtzbrgetka.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.52xcode.cn/gtmlutverb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gtisilhwmf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtcbitfind.html

Go:   func add(a, b int) int
来源：http://hz.ppjwa.cn/gtsfvzxrmx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jlsjyb.cn/gtvknblmuc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.havefunace.top/gtctiuzfdk.html

[C14] 泛型函数
来源：http://hz.bjfxy.top/gtxwuicfns.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guowangkeji.top/gtxscgjknh.html

PHP:  // 无泛型
来源：http://hz.c1oappe.top/gtkaivgymm.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gttkqsxjpr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuxming.cn/gthcrbduyn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hfpthk.cn/gtppvsgzps.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258.top/gtjvdeiihu.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtgpvfrpkq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinqigufen.top/gtrbbjnrdd.html

[C15] 解构 / 展开参数
来源：http://hz.haohaochexian.top/gtyaepvmzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.kuanghao11.cn/gtammvshmt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gtyuvbganl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtsxxvthyj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangtech.top/gtjvlryjzp.html

Java: // 无解构
来源：http://hz.0kj1m.cn/gtvkpgbdqb.html

Go:   // 无解构
来源：http://hz.yanxiufei.cn/gtdrxgznsx.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gtzlyrddtw.html

C#:   var (a, b) = pair;
来源：http://hz.dianchejie.cn/gtgebimbry.html

[C16] 函数 / 方法重载
来源：http://hz.haohaochexian.top/gtdlyikezr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.feifeiyinyue.top/gtrooxpmfp.html

PHP:  // 无重载
来源：http://hz.zhaomingkeji.xyz/gtyrjvbjam.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhiwuduotai.top/gtdixptcob.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuanzhike.top/gtawwhjbdw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daxiang520.top/gttkmantdn.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigfzy.top/gtcedbjzrv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gaohongyu789.top/gtzybrcthy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenlongwang.top/gtuukgxpvt.html

================================================================================
来源：http://hz.jinqigufen.top/gtxlgfmzzy.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtrxpuepvo.html

================================================================================
来源：http://hz.gaohongyu789.top/gtdarzbkbc.html

[D01] 创建数组 / 列表
来源：http://hz.haohaochexian.top/gtaenrebyj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.kuanghao11.cn/gtnmycdgth.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtmwtzbzjn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.havefunace.top/gtpvhpgepy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xylfe.cn/gtoyvnmtwr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangtech.top/gtjiigqiap.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pycfn.com/gtjnksnprw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhengqikj.top/gtoflqnfkb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtctatnvve.html

[D02] 追加元素到末尾
来源：http://hz.vqdsnc.cn/gtgmkmuqha.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yanxiufei.cn/gtqvgtasxz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtbepqzurv.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtowlkgljs.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gtizpqpwtd.html

Java: list.add(4);
来源：http://hz.chenzaomai.com/gtlahruwwh.html

Go:   arr = append(arr, 4)
来源：http://hz.fzhhl.top/gtvceuspie.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinyuanbaomall.cn/gtdipjcvil.html

C#:   list.Add(4);
来源：http://hz.svipenyu.cn/gtwpbloyuy.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtzgkwjxed.html

Py:   arr.insert(0, 0)
来源：http://hz.daxiang520.top/gtyqfogola.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigufen.top/gtjlncbzza.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnxiangtu.top/gtfjogwxui.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtxcmlkasc.html

Java: list.add(0, 0);
来源：http://hz.cdnleiting.top/gtlzijxmib.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhongyouzk.top/gtyinckmrr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yangfankeji.com/gtmmcwktai.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtmzipnaru.html

[D04] 删除元素
来源：http://hz.andypj.xyz/gtubeladbd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtlztiacdx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtbpxqavdc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gttxxuzyxc.html

TS:   arr.splice(0, 1);
来源：http://hz.yuanzhike.top/gthwffekji.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gteojvzxzk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtnrjeqkkn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtxrledzqv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtvwjmknag.html

[D05] 访问与修改元素
来源：http://hz.tian-w.cn/gtgoqktgvl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtjxaickpz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gtpqlobanx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigufen.top/gtixqomvez.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhoulong.xyz/gtpacmmqrt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtmtdofdqu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gteqmjxhej.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtlvnikmur.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gthqoiiydi.html

[D06] 数组长度
来源：http://hz.xylfe.cn/gtnznxbjim.html


<!-- 参考信息 -->