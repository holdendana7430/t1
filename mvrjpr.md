代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.jianghu66.top/gtjvrapuuv.html

Py:   for item in arr: print(item)
来源：http://hz.nwbrower.top/gtnldkubsw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.316326.xyz/gtcxwtkbpu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.sweek.top/gtvvqngpcw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.9152youxi.cn/gtjzxcgzsp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gotoacloud.top/gtvtocmzqn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.52xcode.cn/gtedzeppdb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.meibo888.top/gtrkzchody.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.quarkkingdee.top/gtfnorwfzq.html

[B06] 遍历字典 / 对象
来源：http://hz.wangshuangyany.cn/gtqubgujxp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.dashuyun.cn/gtoftzwusm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hammf.cn/gtfnrwrdnr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aibaodan.cn/gtzxberypm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sweek.top/gtuorrznbb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtxdwrtwja.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.guowangkeji.top/gtswzjtrfo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ehwqpu.com/gtuhetsoyu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.feifeiyinyue.top/gtepoterwn.html

[B07] while 循环
来源：http://hz.sweek.top/gtfebtdwmw.html

Py:   while i < 10: i += 1
来源：http://hz.feifeiyinyue.top/gtsgfoggki.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.dianchejie.cn/gtkhhbcrku.html

JS:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtgblrfezr.html

TS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtwbahaxmg.html

Java: while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtftkqinlg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.vqdsnc.cn/gtsjtbkkob.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ehwqpu.com/gtstdvzevy.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtevfxtsvu.html

[B08] do-while（至少执行一次）
来源：http://hz.zhijiandao.cn/gtdacapejr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.bjfxy.top/gtopivsqmk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jianghu66.top/gtfnkwufxe.html

JS:   do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtiqvxhwli.html

TS:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtboulefbu.html

Java: do { i++; } while (i < 10);
来源：http://hz.ydzc1.top/gtstezohbe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gaohongyu789.top/gtvkrezzko.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yongpay.top/gthltxaykf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtsgmdkaah.html

[B09] break 与 continue
来源：http://hz.wangshuangyany.cn/gtwsarnmij.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cashguo.top/gtaatksfkd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hywenlv.cn/gttxjslmsw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtjonescjk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gtprfrlfok.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtezutgeis.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gtodfgeprv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.havefunace.top/gtekomxsxl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtgkalyxog.html

[B10] 遍历同时拿索引
来源：http://hz.yueranfly.top/gtvwddyott.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gzhubu.top/gtzgcjugtb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.svipenyu.cn/gtyakmqubu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhixingplan.top/gtqalgzfqj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.daxiang520.top/gtzfkcuysv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sxryk.cn/gthntahvwi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yanxiufei.cn/gtxiqhlhvj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aizwys.cn/gtkrnxkidi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangtech.top/gtkqxavnqj.html

[B11] 生成数字序列 / 区间
来源：http://hz.hywenlv.cn/gtyalvhqjt.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxuanxn.top/gthdfalase.html

PHP:  range(0, 10, 2);
来源：http://hz.ybcxt.top/gtrakwwjgz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sufxvd.cn/gtthzxkaye.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dianchejie.cn/gtgoqrlrgq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xingfuxueyuan.xyz/gtpycwmlxp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cucudq.cn/gtkfxcfvfg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuxming.cn/gtiuslesub.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhengqikj.top/gtulawdmxu.html

[B12] 跳出多层循环
来源：http://hz.quarkkingdee.top/gtwipgakdv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhoulong.xyz/gtqbayyejo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ydzc1.top/gtschjzexr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.kuanghao11.cn/gtaievjwhc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtbobfgzut.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtqsbghnam.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinghuilouyu.cn/gtvwhqhzpr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zycfv.cn/gtgmtpotms.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hongshengwenyu.top/gtmrnwnthr.html

[B13] 判断是否为数字
来源：http://hz.hnqzz.top/gtgqeczyxe.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenjidiqi.icu/gtdpqkmtni.html

PHP:  is_numeric($x)
来源：http://hz.ivvv.top/gtpcuotzxq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtnuxqgoox.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fengsongda.top/gtqtscorlc.html

Java: x instanceof Number
来源：http://hz.sysykeji.top/gtbtvqhtph.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cdnleiting.top/gtugicqmee.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shangyingyoupin.top/gtsabytxdf.html

C#:   x is int or double or decimal
来源：http://hz.jqgufenzy.top/gtzewkuehw.html

[B14] 判断值是否在集合内
来源：http://hz.fengsongda.top/gtcwlhhgei.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gtbbclqqxz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jyoumei.cn/gtciugrpgl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.fengsongda.top/gtpnhznaha.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtwnbmnbkm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tanke756.top/gtzvrkdati.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.meibo888.top/gtuybhjlml.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xziqi.cn/gtzvksgang.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.pengpengdd.cyou/gtghlkpmbh.html

[B15] 布尔运算与取反
来源：http://hz.smart0.xyz/gtrvftbngk.html

Py:   a and b or not c
来源：http://hz.cqqwz.cn/gthubzdhtr.html

PHP:  $a && $b || !$c
来源：http://hz.cheryme.top/gtootmsvup.html

JS:   a && b || !c
来源：http://hz.birdmap.top/gtzuxjfxtc.html

TS:   a && b || !c
来源：http://hz.chenzaomai.com/gtoegflhvd.html

Java: a && b || !c
来源：http://hz.pycfn.com/gtmlghwciz.html

Go:   a && b || !c
来源：http://hz.52xcode.cn/gtqzzsujkr.html

Ruby: a && b || !c
来源：http://hz.hongshengwenyu.top/gtsfebqenw.html

C#:   a && b || !c
来源：http://hz.birdmap.top/gtihypkxvq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangkeji.top/gtviebnozs.html

Py:   if not data: return
来源：http://hz.hnqzz.top/gtkgcfpfcu.html

PHP:  if (!$data) { return; }
来源：http://hz.hfpthk.cn/gtyyeiburg.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtydaaawuh.html

TS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtvakdchvy.html

Java: if (data == null) return;
来源：http://hz.gzhubu.top/gttzddofbi.html

Go:   if data == nil { return }
来源：http://hz.gaohongyu789.top/gtqveuvwmu.html

Ruby: return if data.nil?
来源：http://hz.fzhhl.top/gtqrskunij.html

C#:   if (data == null) return;
来源：http://hz.cashguo.top/gtpkjslwyy.html

================================================================================
来源：http://hz.tian-w.cn/gtvcaoyokv.html

C. 函数与作用域
来源：http://hz.andypj.xyz/gtoaigsxqo.html

================================================================================
来源：http://hz.nanxinkj.top/gtjsuffifk.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtlrqfuruq.html

Py:   def add(a, b): return a + b
来源：http://hz.zhixingplan.top/gtovsjimuo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gtlqbotsrc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hfpthk.cn/gtunummlvw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jianghu66.top/gtuvvbzhyu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtfdlgygnl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtfsqjyoul.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhixingplan.top/gtsdkdqljp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtwubqsbfq.html

[C02] 默认参数
来源：http://hz.jinghuilouyu.cn/gtfpaxfexz.html

Py:   def greet(name="World"): return name
来源：http://hz.zycfv.cn/gtsaxthusz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sxryk.cn/gtffdapmtc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yongpay.top/gtqqlqkphw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtcvychlaq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zycfv.cn/gtyljpoujf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangdashe.top/gtydxjavga.html

Ruby: def greet(name = "World") = name
来源：http://hz.shangyingyoupin.top/gtbqbsffxq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tian-w.cn/gtbpvnkkhk.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtrxzvpmcr.html

Py:   def total(*args): return sum(args)
来源：http://hz.ehwqpu.com/gtwpbbyhap.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xuetiantiany.cn/gtodzrkxes.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtmvvzipkn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gtudttvgbm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gtifzzrqdx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.quarkkingdee.top/gtwtoyktpu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tianlin.xyz/gtifycnaky.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtfmhuolso.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuanzx.com/gtdkggscpi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinqigfzy.top/gtpntnnutx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.vqdsnc.cn/gtbhxnmalk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtuxqroffu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hongshengwenyu.top/gtpguoorln.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.vqdsnc.cn/gtzkecxizr.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gthxmfkasf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtfjuogcue.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtpgpcgzbq.html

[C05] 返回多个值
来源：http://hz.ydzc1.top/gtztozwuyr.html

Py:   return a, b
来源：http://hz.chenjidiqi.icu/gtublwttny.html

PHP:  return [$a, $b];
来源：http://hz.c1oappe.top/gtmtidyycg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ehwqpu.com/gtlkayvjuh.html

TS:   return { a, b };
来源：http://hz.sweek.top/gtdybcgzgb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sweek.top/gtebcrnkzh.html

Go:   return a, b
来源：http://hz.guowangkeji.top/gttlnzvxof.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtjdzhlkny.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.52xcode.cn/gtmocyalqj.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gtytcmnzmy.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtxtrlblxg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenlongwang.top/gtoflemnjb.html

JS:   const square = x => x * x;
来源：http://hz.yvedp.cn/gtakfhvztq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.bjfxy.top/gtswzsaetb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yuxming.cn/gtvxyznlei.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fengsongda.top/gtcbfhjvoe.html

Ruby: square = ->(x) { x * x }
来源：http://hz.svipenyu.cn/gtvqxqekcm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jyoumei.cn/gtgbqibmvo.html

[C07] 把函数作为参数传入
来源：http://hz.kuanghao11.cn/gtyjifwisn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gtllyvmnjc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hfpthk.cn/gtavpdzhdn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ybcxt.top/gtdnraxyyv.html

TS:   arr.map(String)
来源：http://hz.sufxvd.cn/gtocumrmul.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jyoumei.cn/gtalumjdwx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.c1oappe.top/gtuccefkra.html

Ruby: arr.map(&:upcase)
来源：http://hz.zdqjudy.top/gtretusvsv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.iojbl.cn/gtuuvptsks.html

[C08] 闭包
来源：http://hz.zhixingplan.top/gtyjcrjnfq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hammf.cn/gtetioaksy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.c1oappe.top/gtzlrdyann.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtweugawzw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtgpflpcng.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhijiandao.cn/gtqqoacvis.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuetiantiany.cn/gttotixsvb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zycfv.cn/gtvlxyjzti.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtlomszanv.html

[C09] 递归
来源：http://hz.pengpengdd.cyou/gtnwltmnju.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtonprokvt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.meibo888.top/gtuonpjnuv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtuluwfzfw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtnbxsvujm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aizwys.cn/gtbrfoqadw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.redwolf501.top/gtlelcxqls.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtqnitywtp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gzhubu.top/gtykhnsool.html

[C10] 变量作用域
来源：http://hz.cqqwz.cn/gtblqcjdmw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dianchejie.cn/gtzbrxcemv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yj20258888.top/gtvarkhrqj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.0kj1m.cn/gtxyurwcwf.html

TS:   同 JS
来源：http://hz.birdmap.top/gtzgaxjagu.html

Java: 方法内为块级作用域
来源：http://hz.yvedp.cn/gtkkddlhyr.html

Go:   花括号块级作用域
来源：http://hz.zycfv.cn/gttjzmutgh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zycfv.cn/gtkkdiqqum.html

C#:   块级作用域
来源：http://hz.ivvv.top/gttnytgyem.html

[C11] 模块导入与导出
来源：http://hz.9152youxi.cn/gtumhcalyq.html

Py:   from module import func
来源：http://hz.xinyue.icu/gtmtvrlyqi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.smart0.xyz/gtntiunsgk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hysaishi.cn/gtjqltasyo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gaohongyu789.top/gtwgskkbuu.html

Java: import java.util.List;
来源：http://hz.shanyushiyangtech.top/gtfwvslbrl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jyoumei.cn/gtarbpzlmz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zycfv.cn/gtpyoobzfv.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtcnvdmjmv.html

[C12] 立即执行函数 IIFE
来源：http://hz.jyoumei.cn/gtswvpdocm.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtzttksgqe.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtwccqsalr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.feifeiyinyue.top/gtnzwvqafl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtrguxrwhv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenlongwang.top/gtzputgwko.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ppjwa.cn/gtzlfhipia.html

Ruby: -> { puts "run" }.call
来源：http://hz.fengsongda.top/gtqapxsvty.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pycfn.com/gtfkfykyce.html

[C13] 类型声明 / 类型注解
来源：http://hz.cheryme.top/gtqhezmfba.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtfhvfrmsr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtvuojlehf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gtcbavpxir.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tianlin.xyz/gtmehivssd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtodughmgh.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gtcrrxiujt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cucudq.cn/gtbsefijyv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cucudq.cn/gtekoanpys.html

[C14] 泛型函数
来源：http://hz.yonumen.top/gturqahttr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinyuanbaomall.cn/gtxhchjvoj.html

PHP:  // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtutlbgsez.html

JS:   // 无泛型
来源：http://hz.yonumen.top/gtrclimsum.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.vqdsnc.cn/gtniokpwzv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jyoumei.cn/gtlnehfbnj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtbjomxuao.html

Ruby: # 无泛型
来源：http://hz.chenjidiqi.icu/gtrgnmveje.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenzaomai.com/gtdesuzyih.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gtkrxgamtn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pengpengdd.cyou/gtstuczupz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gtieejnhsa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gttzbvosvj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jlsjyb.cn/gtjkcsqejs.html

Java: // 无解构
来源：http://hz.shanyushiyangtech.top/gtfolmxmaw.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtaryrylua.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gtpausfacu.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gtjdthhzcx.html

[C16] 函数 / 方法重载
来源：http://hz.tanke756.top/gtzwkpvbvj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tian-w.cn/gtoatpzffr.html

PHP:  // 无重载
来源：http://hz.nwbrower.top/gttospwngq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sysykeji.top/gtcbluuvmp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.svipenyu.cn/gthxdmlxcz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dashuyun.cn/gtkgwvyteo.html

Go:   // 无重载：用不同函数名
来源：http://hz.daria6918.cn/gtawwfddvl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtautubuzy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangkeji.top/gtdlbtddbw.html

================================================================================
来源：http://hz.0kj1m.cn/gtdaesafob.html

D. 数组 / 列表 / 集合
来源：http://hz.iojbl.cn/gtqarbjbaj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtcxvwvndf.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258.top/gtacedwbls.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shzxlz.cn/gtvisrjukh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtzybghqlc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.birdmap.top/gtuiaepamv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtwjudkcud.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuanzx.com/gtjtgbmvri.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shzxlz.cn/gtyyyjuntf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtnwpqhtpa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xinyue.icu/gtrgpysikc.html

[D02] 追加元素到末尾
来源：http://hz.jqgufenzy.top/gtcdugiste.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgufenzy.top/gtblujdwks.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fzhhl.top/gtaplloyaf.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtqrmuanpn.html

TS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtjuafjogf.html

Java: list.add(4);
来源：http://hz.xuanzx.com/gtciulockv.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtcjqnyidg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtufthitbe.html

C#:   list.Add(4);
来源：http://hz.pengpengdd.cyou/gtbojwboje.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtpwufewvq.html

Py:   arr.insert(0, 0)
来源：http://hz.tanke756.top/gtnotvgphe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangkeji.top/gtuiquxhew.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtrlnqaklj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtfizbcgzz.html

Java: list.add(0, 0);
来源：http://hz.9152youxi.cn/gtjzhkqcrb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhongyouzk.top/gtymurxgzp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gtwwpxhehv.html

C#:   list.Insert(0, 0);
来源：http://hz.yuxming.cn/gteepfuylh.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtqfqjtdcw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dianchejie.cn/gtoaxxmnyh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yanxiufei.cn/gtgiakfggp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtssdckslc.html

TS:   arr.splice(0, 1);
来源：http://hz.hnqzz.top/gtkpjpvljp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.mhx1999.top/gtyixkqyyl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ppjwa.cn/gtoltkxlwe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gaohongyu789.top/gtemktukrb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ywan-chungtsiang.top/gtxhkqrqcg.html

[D05] 访问与修改元素
来源：http://hz.havefunace.top/gtaqpannoo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtqsebebtn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gtuoeiynow.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtkzrqjpps.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hongshengwenyu.top/gtofqqcase.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cdnleiting.top/gtyzelqvkr.html


<!-- 参考信息 -->