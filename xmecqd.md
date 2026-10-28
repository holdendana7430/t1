代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenjidiqi.icu/gtuyzmujst.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jqgfzy.top/gteerxtufz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cdnleiting.top/gtevwaaxyv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.pycfn.com/gthsyhgnsa.html

[B05] 遍历数组 / 列表
来源：http://hz.shzxlz.cn/gtnksdnqkh.html

Py:   for item in arr: print(item)
来源：http://hz.svipenyu.cn/gtzauhfklx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinghuilouyu.cn/gtxmnamnuy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.nanxuanxn.top/gthcvfyxdy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.mhx1999.top/gtgkfqrhws.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ivvv.top/gtgoojirxu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guowangkeji.top/gtpwfdosvx.html

Ruby: arr.each { |item| puts item }
来源：http://hz.svipenyu.cn/gtijwbvsem.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jinqigufen.top/gtentyimea.html

[B06] 遍历字典 / 对象
来源：http://hz.jianghu66.top/gtpwxvgwdc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.vqdsnc.cn/gtwdeeafpu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gaohongyu789.top/gtgokbxshk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zycfv.cn/gtnmaxcesb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cdnleiting.top/gtpkzztdip.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aibaodan.cn/gtawiqvgzg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cdnleiting.top/gtdkstnmxn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xingfuxueyuan.xyz/gtfpleprrb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yanxiufei.cn/gtuiukarqq.html

[B07] while 循环
来源：http://hz.ywan-chungtsiang.top/gtunqrlfbb.html

Py:   while i < 10: i += 1
来源：http://hz.shanyushiyangtech.top/gtazwczzmt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinqigufen.top/gtbechqvcn.html

JS:   while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gticidvzal.html

TS:   while (i < 10) { i++; }
来源：http://hz.fzhhl.top/gtplnlwohs.html

Java: while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtamagxius.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.vqdsnc.cn/gtroaofjfr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hfpthk.cn/gtzekpsxvh.html

C#:   while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtvmddwudj.html

[B08] do-while（至少执行一次）
来源：http://hz.xylfe.cn/gtatnqpavr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yvedp.cn/gtxjfdylyt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.aizwys.cn/gtmdixcihc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtbcyzkgyd.html

TS:   do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gtnlbbgxrf.html

Java: do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtpxvpqlxn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hywenlv.cn/gtmsmokyel.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenjidiqi.icu/gtadtpevie.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtxytqbimt.html

[B09] break 与 continue
来源：http://hz.aibaodan.cn/gtibrvgmfg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.9152youxi.cn/gtygvejprc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yongpay.top/gtgbbdqtvx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gtmrueftit.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtkxvqjbcj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtoxugeoqp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.daria6918.cn/gtmanvavyv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtwggzobse.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtwrdicewv.html

[B10] 遍历同时拿索引
来源：http://hz.svipenyu.cn/gtgsqligev.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.havefunace.top/gtooyelapr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.nanxinkj.top/gtppreukrl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtrckbnrzd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cheryme.top/gtjspotldl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sufxvd.cn/gtxqcjtens.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhiwuduotai.top/gtqvdmxbai.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuanzx.com/gtsbmhqcfn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangkeji.top/gtogewmdue.html

[B11] 生成数字序列 / 区间
来源：http://hz.svipenyu.cn/gtfsvrklrn.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtlabpaxkm.html

PHP:  range(0, 10, 2);
来源：http://hz.shangyingyoupin.top/gthehirnel.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtlgdzwmtz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gtispgovuj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.pengpengdd.cyou/gtqjvrhunh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gotoacloud.top/gtkazbvhqt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258.top/gttjvtrhwp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhixingplan.top/gtpggmmyjy.html

[B12] 跳出多层循环
来源：http://hz.smart0.xyz/gtfyuxvlxt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.aibaodan.cn/gtjltfuxlw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shzxlz.cn/gtsxbnolxz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtgclpjzpd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtvbarihro.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtszitduqo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ehwqpu.com/gtdwlpxooa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ehwqpu.com/gtjyebvxyc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhixingplan.top/gtorobmndw.html

[B13] 判断是否为数字
来源：http://hz.zhongyouzk.top/gtlpqpznaz.html

Py:   isinstance(x, (int, float))
来源：http://hz.meibo888.top/gtowumlrce.html

PHP:  is_numeric($x)
来源：http://hz.haohaochexian.top/gtjorshmrm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtjsandlow.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtjkrtywds.html

Java: x instanceof Number
来源：http://hz.fengsongda.top/gtmscphsjx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yuanzhike.top/gthffhozms.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenlongwang.top/gtazuajmag.html

C#:   x is int or double or decimal
来源：http://hz.guowangkeji.top/gtcpnlmafi.html

[B14] 判断值是否在集合内
来源：http://hz.yonumen.top/gtqthfahud.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangtech.top/gtiqjobfra.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.dashuyun.cn/gtcafxsuud.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtvrqinmlu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtwmbqzgby.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.c1oappe.top/gtkxxjaegd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuetiantiany.cn/gtmrivttnv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zycfv.cn/gtxwocgsar.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj20258888.top/gtnlienbix.html

[B15] 布尔运算与取反
来源：http://hz.9152youxi.cn/gtkltaitaw.html

Py:   a and b or not c
来源：http://hz.zycfv.cn/gttfzdresz.html

PHP:  $a && $b || !$c
来源：http://hz.vqdsnc.cn/gtpmfblzur.html

JS:   a && b || !c
来源：http://hz.pycfn.com/gtfmhqffes.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtxcipwiky.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtenihysmv.html

Go:   a && b || !c
来源：http://hz.yj20258.top/gtyztlcxpb.html

Ruby: a && b || !c
来源：http://hz.gzhubu.top/gtfigrcmaw.html

C#:   a && b || !c
来源：http://hz.316326.xyz/gtlntsomhu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangshuangyany.cn/gtgouhvvyx.html

Py:   if not data: return
来源：http://hz.ehwqpu.com/gtkxclnawg.html

PHP:  if (!$data) { return; }
来源：http://hz.52xcode.cn/gtxngbzrgp.html

JS:   if (!data) return;
来源：http://hz.yvedp.cn/gtshmibilg.html

TS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtknjcfemz.html

Java: if (data == null) return;
来源：http://hz.sufxvd.cn/gtanahdqdp.html

Go:   if data == nil { return }
来源：http://hz.zhixingplan.top/gtsjfdurle.html

Ruby: return if data.nil?
来源：http://hz.sysykeji.top/gtgtgxawuw.html

C#:   if (data == null) return;
来源：http://hz.ppjwa.cn/gtxycsgmpf.html

================================================================================
来源：http://hz.gaohongyu789.top/gtvzlvpfai.html

C. 函数与作用域
来源：http://hz.jinqigfzy.top/gtsuembtur.html

================================================================================
来源：http://hz.dianchejie.cn/gtdcofuvuw.html

[C01] 定义函数
来源：http://hz.nanxinkj.top/gtxqiqjwxm.html

Py:   def add(a, b): return a + b
来源：http://hz.chenlongwang.top/gtfwatvznz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtifwdkakv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtegkfrppz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtqkonbqgy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtimkuiqwv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jyoumei.cn/gtasznlglc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.316326.xyz/gttciuptkg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtvrwprrcp.html

[C02] 默认参数
来源：http://hz.tanke756.top/gtfvosollr.html

Py:   def greet(name="World"): return name
来源：http://hz.svipenyu.cn/gtjcyuhgdn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hammf.cn/gtdcgimmqx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtfddgqckq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.fzhhl.top/gtfbyedumq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhaomingkeji.xyz/gttpgjqzjh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenlongwang.top/gtmacnujdt.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gtdqiymbif.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtjlsbguws.html

[C03] 可变参数
来源：http://hz.fzhhl.top/gttdtjnhau.html

Py:   def total(*args): return sum(args)
来源：http://hz.ivvv.top/gtpresuvsv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhengqikj.top/gtjblyohdj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtlbpxmaak.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtsalfvpkn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.smart0.xyz/gtkntfjgqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnqzz.top/gtsnltionx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ivvv.top/gtrzuwdeuh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cdnleiting.top/gtnhoksonp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.c1oappe.top/gtvyxcwkpd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cucudq.cn/gttnfprshi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gtmhhvovlj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtzprqsntf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenlongwang.top/gtcashjmzj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinqigfzy.top/gtbcrndryb.html

Go:   // 无：用配置结构体参数
来源：http://hz.dianchejie.cn/gtfgghvucz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtiqxnoera.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtiphqgdpn.html

[C05] 返回多个值
来源：http://hz.chenzaomai.com/gtuapbxhad.html

Py:   return a, b
来源：http://hz.9152youxi.cn/gtxfammvfh.html

PHP:  return [$a, $b];
来源：http://hz.zhongyouzk.top/gtvspzmbue.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.haohaochexian.top/gtrtlhqtxu.html

TS:   return { a, b };
来源：http://hz.ydzc1.top/gtbwavktzd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yvedp.cn/gtlqtqwqas.html

Go:   return a, b
来源：http://hz.gaohongyu789.top/gtiycxyidb.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gtbgacdmcg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtnqvaupvm.html

[C06] 匿名函数 / lambda
来源：http://hz.jinyuanbaomall.cn/gtsxlzumtf.html

Py:   square = lambda x: x * x
来源：http://hz.aibaodan.cn/gttghabexq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtivzbwxeu.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtshtwdybr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hnxiangtu.top/gtgeqhgfij.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yonumen.top/gtoyzlgsob.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ywan-chungtsiang.top/gthwzwiltq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtktxfppas.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tian-w.cn/gtihyqxzja.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigufen.top/gtcsfdphff.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhaomingkeji.xyz/gtszdgfcor.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.mhx1999.top/gtpqpsxbna.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xylfe.cn/gtarpvipco.html

TS:   arr.map(String)
来源：http://hz.tanke756.top/gtupezijli.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.redwolf501.top/gtbpdqjlef.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aibaodan.cn/gtkczrjbyw.html

Ruby: arr.map(&:upcase)
来源：http://hz.xinyue.icu/gtsaxnripj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtuwtwzmvr.html

[C08] 闭包
来源：http://hz.yvedp.cn/gtuitccbiu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtrwxbdfji.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.redwolf501.top/gtncoeunht.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtbwhbxrwb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtcuvmcbla.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yvedp.cn/gtegtvrfwl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gthljuztty.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.316326.xyz/gtkrqimkub.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtesvqttjq.html

[C09] 递归
来源：http://hz.xylfe.cn/gtxpwebhtk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuanzx.com/gtiribrwov.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.svipenyu.cn/gtirqhwjtx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtikzowdcb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gttzyfrxvf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtkwrqeivd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgfzy.top/gtchbqidgp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhijiandao.cn/gtksfimlsb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hywenlv.cn/gttydpvcbb.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gtscmofdiq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ywan-chungtsiang.top/gtuktsuoqx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.quarkkingdee.top/gtkvhkhuip.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtmntqljmt.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtdmwtehra.html

Java: 方法内为块级作用域
来源：http://hz.fengsongda.top/gtglrnnnvx.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangkeji.top/gtjwlziqrc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtohxgjegn.html

C#:   块级作用域
来源：http://hz.snrcjt.cn/gtvzmpfgde.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtmhkchvrv.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gtftomyzqb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.snrcjt.cn/gtkdtryple.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydjk.org.cn/gtfystdftx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigfzy.top/gthizrqktf.html

Java: import java.util.List;
来源：http://hz.kuanghao11.cn/gtobuzatqf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangtech.top/gtgotkcimc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinyuanbaomall.cn/gtsuafcfjf.html

C#:   using System.Text;
来源：http://hz.shanyushiyangtech.top/gtywavuzzx.html

[C12] 立即执行函数 IIFE
来源：http://hz.quarkkingdee.top/gtnikbvcsh.html

Py:   (lambda: print("run"))()
来源：http://hz.sweek.top/gtjtjckqql.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtogxkyias.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtivgnafub.html

TS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gtljqyqfpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinyuanbaomall.cn/gtswnspusu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xziqi.cn/gtlbmsoiqs.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhoulong.xyz/gturjmmgdh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.vqdsnc.cn/gtmnabwnjf.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtgooytwks.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.iojbl.cn/gthaoopptm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtrlrvxybj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258888.top/gtwedsghez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtnelzsihl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtohrscqvj.html

Go:   func add(a, b int) int
来源：http://hz.52xcode.cn/gtbhzrjrad.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gttmkeohwj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jyoumei.cn/gtvjcefkws.html

[C14] 泛型函数
来源：http://hz.sweek.top/gtlooiwfai.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.feifeiyinyue.top/gtqxrsgbip.html

PHP:  // 无泛型
来源：http://hz.yangfankeji.com/gtitbbmdag.html

JS:   // 无泛型
来源：http://hz.gogol.net.cn/gtscqhjmmv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtonklbeli.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.havefunace.top/gtdcucfegl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtzqxeriud.html

Ruby: # 无泛型
来源：http://hz.hfpthk.cn/gtlmudmbjk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yangfankeji.com/gtwwbtezgx.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258.top/gtdgwgnsav.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sweek.top/gtvtgkqzbr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gtqgcvhshq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtygemftfl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daria6918.cn/gtvqenfctj.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtocrpxxxh.html

Go:   // 无解构
来源：http://hz.zhijiandao.cn/gtlbduxusi.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtdpfkalnx.html

C#:   var (a, b) = pair;
来源：http://hz.jiagoushi.top/gtxrcypcns.html

[C16] 函数 / 方法重载
来源：http://hz.hammf.cn/gtwcebcspn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtdabbjuvq.html

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gthwqkaaru.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ydzc1.top/gtlbaytezp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuetiantiany.cn/gtltympjux.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtxmyrkdpk.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtndlrhcgd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtyxczzfnw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenjidiqi.icu/gtfbhexqpk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcadgxead.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtrpxnxnyg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbgbxuxva.html

[D01] 创建数组 / 列表
来源：http://hz.zhoulong.xyz/gtfseqsvad.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gzhubu.top/gtmydmgtgc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtdjleenig.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daxiang520.top/gtcgkvexft.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtvyuswevy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.kuanghao11.cn/gtamwcdjmn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gtmmxdbzxx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangdashe.top/gtchfotgas.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gtytfmazwj.html

[D02] 追加元素到末尾
来源：http://hz.xuanzx.com/gttoqvqvvo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.haohaochexian.top/gtemlulflc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gttnaedbat.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtzuqtafwo.html

TS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtxmjhihja.html

Java: list.add(4);
来源：http://hz.jianghu66.top/gthcymbcuu.html

Go:   arr = append(arr, 4)
来源：http://hz.zycfv.cn/gtsdqxxmcq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.iojbl.cn/gtviwfgvya.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtlfikhxsr.html

[D03] 在指定位置插入元素
来源：http://hz.kuanghao11.cn/gtbwxcizth.html

Py:   arr.insert(0, 0)
来源：http://hz.ydjk.org.cn/gtankypljd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuxming.cn/gtpwkssmdy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenjidiqi.icu/gtppifsvbk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtksciqpla.html

Java: list.add(0, 0);
来源：http://hz.xuanzx.com/gtpsmghbdl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gtkhrsqela.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ywan-chungtsiang.top/gtqsvdvvst.html

C#:   list.Insert(0, 0);
来源：http://hz.52xcode.cn/gtsmqeqmcx.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtxizuhgvk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtrpxkuiyh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ybcxt.top/gtxconmlfq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dashuyun.cn/gtxpzqajvv.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtyrwbwdje.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenjidiqi.icu/gtyoazwhfa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtblyaalfr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gotoacloud.top/gtegicjscz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shzxlz.cn/gtljcqbxai.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gthzjpxatn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtcopcxsme.html


<!-- 参考信息 -->