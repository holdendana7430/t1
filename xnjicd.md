代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hz.gogol.net.cn/gtkbuhsqef.html

Py:   for item in arr: print(item)
来源：http://hz.jyoumei.cn/gtvvpfufky.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xylfe.cn/gtvtyrlqth.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gtltlgzkbg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sysykeji.top/gtxvnybcyh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigfzy.top/gtugeygcde.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jlsjyb.cn/gtsjndowlh.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nanxinkj.top/gtrzploivl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hysaishi.cn/gtgoavjntq.html

[B06] 遍历字典 / 对象
来源：http://hz.redwolf501.top/gtmcjmzdrv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xuanzx.com/gtgaonbbrp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shzxlz.cn/gtolzijolw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xinyue.icu/gtxzmzicgd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtqkagytsu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtvjjdhxjf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuetiantiany.cn/gtjhrznrwf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxuanxn.top/gtaftezwrs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.bjfxy.top/gtntuahdre.html

[B07] while 循环
来源：http://hz.aibaodan.cn/gtdlriofqj.html

Py:   while i < 10: i += 1
来源：http://hz.dianchejie.cn/gttrntfspz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gotoacloud.top/gtwqmcpytd.html

JS:   while (i < 10) { i++; }
来源：http://hz.havefunace.top/gthswywxur.html

TS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtjyfumwgl.html

Java: while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtxnclddwd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.pengpengdd.cyou/gtkocriiqr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.gotoacloud.top/gtyzrsskcu.html

C#:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtcdahpczi.html

[B08] do-while（至少执行一次）
来源：http://hz.shanyushiyangtech.top/gtialgrgpd.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hnqzz.top/gtbplwqeil.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hysaishi.cn/gtmlkoxpkt.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhengqikj.top/gtxoyblnty.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtekdohasr.html

Java: do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtuapbnyhe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.guowangkeji.top/gtoijwvkfi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yanxiufei.cn/gtrfwtmoyg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tian-w.cn/gtemeszcmp.html

[B09] break 与 continue
来源：http://hz.52xcode.cn/gtmkbgqevx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shuidangran.top/gtnrvatsxl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gaohongyu789.top/gtvezhklop.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gtcxbxfzst.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtpqxtfghi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtixxltnrh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.meibo888.top/gtejhoqgft.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gtzkhsibmz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gttlrdlefs.html

[B10] 遍历同时拿索引
来源：http://hz.hnqzz.top/gtwfqghqvi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yuxming.cn/gtweyaapig.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.snrcjt.cn/gtdijezfuz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtpljqxpaj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.9152youxi.cn/gtschfospx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.kuanghao11.cn/gtvlgythom.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.feifeiyinyue.top/gtkqawzuxw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgufenzy.top/gtcmljgbvb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.aibaodan.cn/gtcldugpbb.html

[B11] 生成数字序列 / 区间
来源：http://hz.haohaochexian.top/gtkcfvoyyj.html

Py:   list(range(0, 10, 2))
来源：http://hz.fzhhl.top/gtybxljtzd.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgufenzy.top/gthmkgehfx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sxryk.cn/gtzzjhroti.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.52xcode.cn/gtsblxwshr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gogol.net.cn/gtzsvltsmf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ydjk.org.cn/gtyzqjupxf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.mhx1999.top/gtchdwajub.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ywan-chungtsiang.top/gtafjhryhq.html

[B12] 跳出多层循环
来源：http://hz.haohaochexian.top/gtgxbrdcon.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sxryk.cn/gtoivudrpx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shanyushiyangkeji.top/gtmngtmxbv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtpisjtosj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtsdujzhrr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gttgzweqdc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.daria6918.cn/gtezvusbol.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.9152youxi.cn/gthwnfbuxj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenjidiqi.icu/gtutyjgqly.html

[B13] 判断是否为数字
来源：http://hz.gogol.net.cn/gtscdkkoki.html

Py:   isinstance(x, (int, float))
来源：http://hz.316326.xyz/gtebrvyegn.html

PHP:  is_numeric($x)
来源：http://hz.shanyushiyangtech.top/gttsdxqlrj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtjruxzjnp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jlsjyb.cn/gtyexrydlf.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gthaijdipj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigfzy.top/gtphsevkvk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.iojbl.cn/gtymxmmcrz.html

C#:   x is int or double or decimal
来源：http://hz.fengsongda.top/gtvexfrbtj.html

[B14] 判断值是否在集合内
来源：http://hz.dianchejie.cn/gtsmlfaoox.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yangfankeji.com/gtrjpnjimv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxuanxn.top/gtxwtmtnmy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.aizwys.cn/gtiniztvns.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gtecrlljvu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.vqdsnc.cn/gthndchhcs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenjidiqi.icu/gtppejutly.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jiagoushi.top/gtjaamdvbz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtixswrmux.html

[B15] 布尔运算与取反
来源：http://hz.shuidangran.top/gtmecenonk.html

Py:   a and b or not c
来源：http://hz.hnxiangtu.top/gtrsebzucf.html

PHP:  $a && $b || !$c
来源：http://hz.hywenlv.cn/gtozgaebih.html

JS:   a && b || !c
来源：http://hz.redwolf501.top/gtsugrfuoy.html

TS:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtaarihxbt.html

Java: a && b || !c
来源：http://hz.jqgufenzy.top/gtkujmmsrn.html

Go:   a && b || !c
来源：http://hz.redwolf501.top/gtpmiuzfch.html

Ruby: a && b || !c
来源：http://hz.cheryme.top/gtjkjkfyik.html

C#:   a && b || !c
来源：http://hz.bjfxy.top/gttvgtldkt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guowangkeji.top/gtthdiataq.html

Py:   if not data: return
来源：http://hz.hongshengwenyu.top/gtzqavbcxq.html

PHP:  if (!$data) { return; }
来源：http://hz.yanxiufei.cn/gtkrhklhkv.html

JS:   if (!data) return;
来源：http://hz.ybcxt.top/gtxevjoesp.html

TS:   if (!data) return;
来源：http://hz.yuxming.cn/gtwjutktej.html

Java: if (data == null) return;
来源：http://hz.zhengqikj.top/gtqxrulqdj.html

Go:   if data == nil { return }
来源：http://hz.nanxinkj.top/gtwonzyotf.html

Ruby: return if data.nil?
来源：http://hz.dashuyun.cn/gtrglkwtft.html

C#:   if (data == null) return;
来源：http://hz.zdqjudy.top/gtojgrdqsz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtiynmuhat.html

C. 函数与作用域
来源：http://hz.hongshengwenyu.top/gtubxqyiqb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrvdppqgr.html

[C01] 定义函数
来源：http://hz.guannengcc.top/gtfywbyfpd.html

Py:   def add(a, b): return a + b
来源：http://hz.xinyue.icu/gthtnzsicu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtyrzztsco.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fzhhl.top/gtadzdwchz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtzxwmmxnp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtwsxkojzq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gaohongyu789.top/gtdtyymjnf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinghuilouyu.cn/gtclzusabg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtceynerhc.html

[C02] 默认参数
来源：http://hz.tian-w.cn/gtxwmdsnlm.html

Py:   def greet(name="World"): return name
来源：http://hz.hammf.cn/gtspgyjlcw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gotoacloud.top/gtenfptxdq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.52xcode.cn/gtppiktvnn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aizwys.cn/gtekfmgtlf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hongshengwenyu.top/gtkydupdnk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtjoqymuug.html

Ruby: def greet(name = "World") = name
来源：http://hz.jyoumei.cn/gtxzsknnpd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.316326.xyz/gthnwgdbvc.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtntsrgidf.html

Py:   def total(*args): return sum(args)
来源：http://hz.ybcxt.top/gtwibtsril.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xuanzx.com/gtjqdiebbl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtkkfulqbz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pycfn.com/gtwenkmsyr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guowangkeji.top/gteqcjcekn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuanzhike.top/gtmivfztiy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hongshengwenyu.top/gtvudxtapi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtdrpkpvtt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jianghu66.top/gtaqdebgsy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hammf.cn/gtrjapsrxf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cdnleiting.top/gtusczksug.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gotoacloud.top/gtaguzxgoa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xingfuxueyuan.xyz/gtmgygpwpl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhengqikj.top/gtrozwolum.html

Go:   // 无：用配置结构体参数
来源：http://hz.birdmap.top/gtjfiimtoi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtuowwilnk.html

C#:   f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtdqlazlyo.html

[C05] 返回多个值
来源：http://hz.hfpthk.cn/gtngrlgvhz.html

Py:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtzgdhtaeb.html

PHP:  return [$a, $b];
来源：http://hz.gogol.net.cn/gtotyvmoqx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ivvv.top/gtkvebgcdn.html

TS:   return { a, b };
来源：http://hz.zhengqikj.top/gtwmjnsqey.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ybcxt.top/gtixrnenyb.html

Go:   return a, b
来源：http://hz.zhengqikj.top/gtkxyettti.html

Ruby: return a, b
来源：http://hz.yongpay.top/gtuhsyddms.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dashuyun.cn/gtwdabahge.html

[C06] 匿名函数 / lambda
来源：http://hz.jiagoushi.top/gtuidcooym.html

Py:   square = lambda x: x * x
来源：http://hz.guowangkeji.top/gtuakowlje.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.redwolf501.top/gtzixeyycr.html

JS:   const square = x => x * x;
来源：http://hz.yvedp.cn/gtpngndbkj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.316326.xyz/gtetorheqw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yvedp.cn/gtebxhtcvi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xylfe.cn/gtrejvlckg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.andypj.xyz/gtduzqxodp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tian-w.cn/gtgghrwjly.html

[C07] 把函数作为参数传入
来源：http://hz.316326.xyz/gtyykxjhhy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.havefunace.top/gtzisnffps.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.daxiang520.top/gtgxjwhpyc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jianghu66.top/gteqcknnpg.html

TS:   arr.map(String)
来源：http://hz.sysykeji.top/gtvtiruple.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhijiandao.cn/gtuuzvrhpk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhijiandao.cn/gtsdvhfgbl.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtqftgrvnz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.havefunace.top/gtiblzfhhj.html

[C08] 闭包
来源：http://hz.pengpengdd.cyou/gthldmaocf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gtjrmtxpdt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gaohongyu789.top/gtsanmemvl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtdluqgjoo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtdumajaat.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.andypj.xyz/gtmroaycud.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jiagoushi.top/gtyqrvevva.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtogwhizds.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtswmwdloq.html

[C09] 递归
来源：http://hz.316326.xyz/gtwncvatwz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shanyushiyangtech.top/gtorshokdy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.redwolf501.top/gtemisgmlk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangdashe.top/gtbgiplwhn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtvowniymj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shangyingyoupin.top/gtoshpignq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhijiandao.cn/gtrupeobqo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtgruwjsvk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangtech.top/gtiurueiwj.html

[C10] 变量作用域
来源：http://hz.nanxuanxn.top/gtsolnonqn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenzaomai.com/gtxmmqwkkt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.chenjidiqi.icu/gtjrbvkfct.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangtech.top/gtlxdrsckb.html

TS:   同 JS
来源：http://hz.52xcode.cn/gtbngrnbfk.html

Java: 方法内为块级作用域
来源：http://hz.xuetiantiany.cn/gtddnkkcar.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gthsbfvwur.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guannengcc.top/gtcmzdxola.html

C#:   块级作用域
来源：http://hz.gotoacloud.top/gtkeqlkxrm.html

[C11] 模块导入与导出
来源：http://hz.vqdsnc.cn/gtyuqhvsav.html

Py:   from module import func
来源：http://hz.cucudq.cn/gthheqxtyv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtzeijqddz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.meibo888.top/gttkikqaak.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gzhubu.top/gtzxyewywr.html

Java: import java.util.List;
来源：http://hz.jinqigfzy.top/gtcdtwypbj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.52xcode.cn/gtflchujgb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258888.top/gtvoaqpqdq.html

C#:   using System.Text;
来源：http://hz.52xcode.cn/gtgssylxcb.html

[C12] 立即执行函数 IIFE
来源：http://hz.haohaochexian.top/gtsguudoqz.html

Py:   (lambda: print("run"))()
来源：http://hz.jinghuilouyu.cn/gttwsyxzmc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtbdyfolqs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtcsjhwwtn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gttiyvpetl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pengpengdd.cyou/gtuslfexim.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yueranfly.top/gtaqzmibxx.html

Ruby: -> { puts "run" }.call
来源：http://hz.cucudq.cn/gtjtpfecpu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtoakqyvhy.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhiwuduotai.top/gtcgjimrjs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtbwsxyezl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtbkphkyew.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jianghu66.top/gthpuxirrh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtitwmdxaw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtvbwidmyg.html

Go:   func add(a, b int) int
来源：http://hz.shuidangran.top/gtmwyqipkl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtolpcgaoj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhixingplan.top/gtemlsuubs.html

[C14] 泛型函数
来源：http://hz.9152youxi.cn/gtkbdrzbyw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtpgcsbhdf.html

PHP:  // 无泛型
来源：http://hz.yanxiufei.cn/gtwyeirhwd.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gtoizetljk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dashuyun.cn/gtpdmsdbps.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuanzx.com/gtvluazzsr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xylfe.cn/gtglgogwqi.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtwjghajeq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hammf.cn/gtfgltpmja.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gthxhklrwf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtitbdbqsx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yonumen.top/gtyztyeyda.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gttrhptbld.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenjidiqi.icu/gtipfnyqnj.html

Java: // 无解构
来源：http://hz.ivvv.top/gthdhrrixh.html

Go:   // 无解构
来源：http://hz.chenzaomai.com/gtgryrklkl.html

Ruby: a, b = pair
来源：http://hz.redwolf501.top/gtwonvnvfu.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gttjelaajb.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtfkvpxswu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtcfrkefzc.html

PHP:  // 无重载
来源：http://hz.chenjidiqi.icu/gtqrsiuhox.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.snrcjt.cn/gtqqtxjfdp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenlongwang.top/gtujcpohll.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jiagoushi.top/gtrrnoasgi.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtquqylcqm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daxiang520.top/gtfeaiyhli.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtgisudfns.html

================================================================================
来源：http://hz.0kj1m.cn/gtsomjjuru.html

D. 数组 / 列表 / 集合
来源：http://hz.kuanghao11.cn/gtbcucljuc.html

================================================================================
来源：http://hz.dashuyun.cn/gtbxswzqmf.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtrtxpuncw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gthjjgqjks.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daria6918.cn/gtphzmvuor.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gtossgaria.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gtvenmwpda.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhijiandao.cn/gtquqemhxi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuxming.cn/gtlubpvntw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yuxming.cn/gtjtzojmku.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtkxdvqvsy.html

[D02] 追加元素到末尾
来源：http://hz.yuxming.cn/gtvcumfqcc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zdqjudy.top/gtecgvnvwk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ywan-chungtsiang.top/gtcarbmmpk.html

JS:   arr.push(4);
来源：http://hz.tian-w.cn/gtypvjwnew.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtaoygxtri.html

Java: list.add(4);
来源：http://hz.zhengqikj.top/gtfeosuzwc.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtainzfvgi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.svipenyu.cn/gtbilhbaqh.html

C#:   list.Add(4);
来源：http://hz.redwolf501.top/gtyscnegpe.html

[D03] 在指定位置插入元素
来源：http://hz.yuanzhike.top/gtqyhhimos.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtddwbemgd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtvnlpvbkg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtigdjkhoe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhoulong.xyz/gtsdfwzwqs.html

Java: list.add(0, 0);
来源：http://hz.dianchejie.cn/gtjwlugney.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gtjqygoseq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtzlnfsfdj.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigfzy.top/gtrdnyuxol.html

[D04] 删除元素
来源：http://hz.birdmap.top/gtmoejmrqm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dianchejie.cn/gtzwxcvkpg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinyuanbaomall.cn/gttkzkpbjl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shzxlz.cn/gttjojjngg.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtpraqegyj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.smart0.xyz/gtuqtzerij.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj20258888.top/gtrywfymes.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtymehwkzj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ywan-chungtsiang.top/gtmljvqhxv.html

[D05] 访问与修改元素
来源：http://hz.zhaomingkeji.xyz/gtwaqhocod.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtwcvqzaqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtnldptowz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhixingplan.top/gtnanleawd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yuanzhike.top/gtiwausgpk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtjoiwzsyx.html


<!-- 参考信息 -->