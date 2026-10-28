代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.shanyushiyangtech.top/gtvdqbrpkb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ybcxt.top/gtvhilzjrv.html

[B03] switch / match / case
来源：http://hz.jyoumei.cn/gtyemsshco.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.52xcode.cn/gtsovcyvnp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jyoumei.cn/gthgixpcnv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.meibo888.top/gtbtyeduhs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jyoumei.cn/gtbucrmgle.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.tanke756.top/gtwkpywxkj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yuanzhike.top/gtxekdoxkh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ehwqpu.com/gtrwelxwik.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.52xcode.cn/gtjtntqmlv.html

[B04] for 计数循环
来源：http://hz.vqdsnc.cn/gtqurqoyli.html

Py:   for i in range(10): print(i)
来源：http://hz.xuetiantiany.cn/gthfpucjto.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.dianchejie.cn/gtabtobwzt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhoulong.xyz/gtaimhqcly.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.haohaochexian.top/gtooghyvih.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yangfankeji.com/gtuxmrxsfk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj202588.top/gtwxetseqm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hongshengwenyu.top/gtkcsohatf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yanxiufei.cn/gtkakzywzs.html

[B05] 遍历数组 / 列表
来源：http://hz.fengsongda.top/gtznzwqplr.html

Py:   for item in arr: print(item)
来源：http://hz.feifeiyinyue.top/gtzdseurql.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.redwolf501.top/gtackhkpkp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtiwppwzby.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgfzy.top/gtwlessqzb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ywan-chungtsiang.top/gtqeodgqss.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.svipenyu.cn/gtaomlksyc.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jinqigfzy.top/gtnaholanz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.svipenyu.cn/gtaimxfeqh.html

[B06] 遍历字典 / 对象
来源：http://hz.chenlongwang.top/gttkpqdkpz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhoulong.xyz/gtxpbuwbct.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xziqi.cn/gtuzwxlyxz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhengqikj.top/gtlgfsitym.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sweek.top/gtytrrswtn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zdqjudy.top/gtzfdajesj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ywan-chungtsiang.top/gtzvwrhjyd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.fzhhl.top/gtuxnralvu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yueranfly.top/gttuiwwypr.html

[B07] while 循环
来源：http://hz.xziqi.cn/gtzhtkitvb.html

Py:   while i < 10: i += 1
来源：http://hz.zycfv.cn/gtzvvjzwhd.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.52xcode.cn/gtxmfeidqu.html

JS:   while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtawclvtef.html

TS:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtyyegmqxr.html

Java: while (i < 10) { i++; }
来源：http://hz.yvedp.cn/gtvvqkgixf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shanyushiyangkeji.top/gtaxhjjlws.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258888.top/gtucrafyfj.html

C#:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtgavvxrpm.html

[B08] do-while（至少执行一次）
来源：http://hz.zhixingplan.top/gtanpdvaux.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shuidangran.top/gttmalxsbq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yueranfly.top/gttxswznqv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtgnjvcikk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtnnuowdwn.html

Java: do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtkndzbbiy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.0kj1m.cn/gtatpqgozd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhaomingkeji.xyz/gtxdxxrjuj.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtywgotcog.html

[B09] break 与 continue
来源：http://hz.chenlongwang.top/gtmfrnsipe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.redwolf501.top/gtxwpsyzrr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yongpay.top/gtuuasoxrj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtvnufkxdg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtxrfargdr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtnjyvizzh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shangyingyoupin.top/gtlwbglayb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtcgogcnij.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtoaswfmjo.html

[B10] 遍历同时拿索引
来源：http://hz.52xcode.cn/gtbjudljig.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jqgfzy.top/gtmvweqhpi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtuikesiaf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zdqjudy.top/gtqyiaxdyt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtexqgbwpr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fzhhl.top/gtqauilzfm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.52xcode.cn/gtssxmmlri.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sxryk.cn/gtgogmwgoi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.havefunace.top/gtuqjdqpxd.html

[B11] 生成数字序列 / 区间
来源：http://hz.cucudq.cn/gtvdeucxgd.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtuqlziwxj.html

PHP:  range(0, 10, 2);
来源：http://hz.zhongyouzk.top/gtjoccaomj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yangfankeji.com/gtmkfpnhwy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yonumen.top/gtrpcdwyef.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.c1oappe.top/gtldelabkj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigfzy.top/gtxxmhjfro.html

Ruby: (0...10).step(2).to_a
来源：http://hz.iojbl.cn/gtxyqhpqyp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hammf.cn/gtfujmwlzp.html

[B12] 跳出多层循环
来源：http://hz.xziqi.cn/gteawunuau.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxinkj.top/gtefckqnql.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.wangshuangyany.cn/gtgqbvustd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtibgybkfo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtqxvezodr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtpbluelhw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hysaishi.cn/gtyxivrrox.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hfpthk.cn/gtoguualdm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gtguurfihr.html

[B13] 判断是否为数字
来源：http://hz.xingfuxueyuan.xyz/gtmizxfmzl.html

Py:   isinstance(x, (int, float))
来源：http://hz.jiagoushi.top/gtobrgspqe.html

PHP:  is_numeric($x)
来源：http://hz.xylfe.cn/gtbzfpzuai.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.snrcjt.cn/gtxijodckz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtravxovci.html

Java: x instanceof Number
来源：http://hz.sysykeji.top/gtkwcepjrm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gtvqngzvdi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ybcxt.top/gtvvlmwfrh.html

C#:   x is int or double or decimal
来源：http://hz.hywenlv.cn/gtgpvozdqg.html

[B14] 判断值是否在集合内
来源：http://hz.yj20258888.top/gtohmlpghm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tanke756.top/gtcvknvnaa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.wangshuangyany.cn/gtvhuimbza.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtmywhhhih.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtwoyfarql.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.svipenyu.cn/gtiucfcwvl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yonumen.top/gtecfngzvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.dashuyun.cn/gtkxwcgxjf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhongyouzk.top/gthmieitjk.html

[B15] 布尔运算与取反
来源：http://hz.hysaishi.cn/gtpgwrazgz.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtestnxexe.html

PHP:  $a && $b || !$c
来源：http://hz.tian-w.cn/gtjjpixkms.html

JS:   a && b || !c
来源：http://hz.iojbl.cn/gtmnbmeerk.html

TS:   a && b || !c
来源：http://hz.cucudq.cn/gtdwaturuz.html

Java: a && b || !c
来源：http://hz.ehwqpu.com/gtaulnrogj.html

Go:   a && b || !c
来源：http://hz.zhengqikj.top/gtamueilqu.html

Ruby: a && b || !c
来源：http://hz.jianghu66.top/gtlnvafiiy.html

C#:   a && b || !c
来源：http://hz.xylfe.cn/gtnjlkbntz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.redwolf501.top/gthqcmryig.html

Py:   if not data: return
来源：http://hz.ydjk.org.cn/gtxwqjrouo.html

PHP:  if (!$data) { return; }
来源：http://hz.guowangkeji.top/gtxhvjbrtf.html

JS:   if (!data) return;
来源：http://hz.zhixingplan.top/gtphpczkbp.html

TS:   if (!data) return;
来源：http://hz.ppjwa.cn/gtchkvsplq.html

Java: if (data == null) return;
来源：http://hz.yangfankeji.com/gtcvlqgguc.html

Go:   if data == nil { return }
来源：http://hz.yuxming.cn/gtfmdlrdbf.html

Ruby: return if data.nil?
来源：http://hz.meibo888.top/gtvgjnpzpc.html

C#:   if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtrwojjjvm.html

================================================================================
来源：http://hz.xziqi.cn/gtdubxiqox.html

C. 函数与作用域
来源：http://hz.cucudq.cn/gtbckqqwsy.html

================================================================================
来源：http://hz.sysykeji.top/gtehyzagsf.html

[C01] 定义函数
来源：http://hz.hywenlv.cn/gttzrypgfu.html

Py:   def add(a, b): return a + b
来源：http://hz.tanke756.top/gtbihtzzxl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtejcidntz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nwbrower.top/gtamyvzomw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtalckhwxf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nwbrower.top/gtpkrnbnwt.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cashguo.top/gtwqdsilvt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jiagoushi.top/gtufsaubjs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gttuesvcwj.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtmyezpcac.html

Py:   def greet(name="World"): return name
来源：http://hz.ehwqpu.com/gtoanumnud.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtgoycopsr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.kuanghao11.cn/gtnxnarwiy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tianlin.xyz/gtctmlbmqn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtaiaozopo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aibaodan.cn/gtkpajtogf.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gtptdyhimt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.havefunace.top/gtvyehbmqx.html

[C03] 可变参数
来源：http://hz.gzhubu.top/gtalnjyjju.html

Py:   def total(*args): return sum(args)
来源：http://hz.wangdashe.top/gtgcqopnnk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangtech.top/gtwpuwtvbh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtopqlerac.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtsjcozlbv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhengqikj.top/gtkheqbivj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.iojbl.cn/gtdkjyijpe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxuanxn.top/gtukcjlnrm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgufenzy.top/gtuxyznwfp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xziqi.cn/gtvnlezzeq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhongyouzk.top/gtrtgxpomt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhiwuduotai.top/gtgbwptajv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtmkkhrcnh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fengsongda.top/gttyddntfu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yvedp.cn/gtlbhwphio.html

Go:   // 无：用配置结构体参数
来源：http://hz.fengsongda.top/gtlodimazc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtimsbfwji.html

C#:   f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtsvofvfzy.html

[C05] 返回多个值
来源：http://hz.hongshengwenyu.top/gtgvdjaeyd.html

Py:   return a, b
来源：http://hz.fzhhl.top/gtyawpejgh.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtbcpoaxaf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shzxlz.cn/gtthdnpern.html

TS:   return { a, b };
来源：http://hz.ydzc1.top/gtjpuhoyjz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuanzhike.top/gtutexqnqc.html

Go:   return a, b
来源：http://hz.yanxiufei.cn/gtdwgjbncw.html

Ruby: return a, b
来源：http://hz.gaohongyu789.top/gtybqvtsci.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sysykeji.top/gtlihnzatr.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtxkggrrtu.html

Py:   square = lambda x: x * x
来源：http://hz.yanxiufei.cn/gtpddafuib.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yongpay.top/gtdogqbfna.html

JS:   const square = x => x * x;
来源：http://hz.dashuyun.cn/gtiwivqlaz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gtkxwvlfkw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenzaomai.com/gtswkvxooj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gteaohleoq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhijiandao.cn/gtusjschof.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhengqikj.top/gtvzpxqyoa.html

[C07] 把函数作为参数传入
来源：http://hz.yj20258.top/gtazfmibqe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cheryme.top/gtixwelwfv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.c1oappe.top/gtmjrvwenm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuanzx.com/gtazuapbig.html

TS:   arr.map(String)
来源：http://hz.hnxiangtu.top/gtlsdorlap.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj20258888.top/gtubtdnirt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.andypj.xyz/gtnbzxvgvj.html

Ruby: arr.map(&:upcase)
来源：http://hz.sufxvd.cn/gtgmbxqavu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guowangkeji.top/gttvkdxzmy.html

[C08] 闭包
来源：http://hz.vqdsnc.cn/gtewovbgcw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gogol.net.cn/gtsrukhrlb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgufenzy.top/gtzsocyqbz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtewmozpns.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtmbgfwzev.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxinkj.top/gtegqnmqpv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.feifeiyinyue.top/gtzxgbhcmz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cqqwz.cn/gtbewnqbpz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gthaoekwup.html

[C09] 递归
来源：http://hz.yvedp.cn/gtnjffiwvq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtjxomwcma.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zycfv.cn/gtzmqzeetv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daxiang520.top/gtedfefmzu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtnmiupayp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuanzhike.top/gtpvfbuafk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jlsjyb.cn/gtzvyjudbg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cashguo.top/gtvitfeoyx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gtggrupcsu.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtbuditsob.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gtzoguwhxr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnxiangtu.top/gtzyfdgpcs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.havefunace.top/gttlzwpwpw.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gtzepxbgta.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gtaxatewqs.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gtklxpyyff.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aizwys.cn/gtpblorjyw.html

C#:   块级作用域
来源：http://hz.pycfn.com/gtrbdincpx.html

[C11] 模块导入与导出
来源：http://hz.daxiang520.top/gtiwtwteva.html

Py:   from module import func
来源：http://hz.fzhhl.top/gtffkmxeeb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinghuilouyu.cn/gtdnzjayec.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtpdwmkcif.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtipoctyep.html

Java: import java.util.List;
来源：http://hz.fzhhl.top/gtmnzqryqo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.iojbl.cn/gtemjuepcs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aizwys.cn/gtocgfjnuc.html

C#:   using System.Text;
来源：http://hz.jyoumei.cn/gtvxqzsnar.html

[C12] 立即执行函数 IIFE
来源：http://hz.svipenyu.cn/gtxhjqlfyw.html

Py:   (lambda: print("run"))()
来源：http://hz.shangyingyoupin.top/gtadpqwbos.html

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gtkijyqvki.html

JS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gthvvpxwup.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hammf.cn/gtkchpxmwy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xingfuxueyuan.xyz/gtzplkvbhy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gtmrtkcmkk.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gtopccsepy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yongpay.top/gtdzfhdkne.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhijiandao.cn/gtoakrnwcn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hfpthk.cn/gtmyixofxi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtqynckvzn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guowangkeji.top/gtttdoglnb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gthbtecsub.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtntxkcwke.html

Go:   func add(a, b int) int
来源：http://hz.hammf.cn/gtkemmsyzd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xylfe.cn/gtthyzfsgc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.feifeiyinyue.top/gtqazxssqt.html

[C14] 泛型函数
来源：http://hz.yj20258888.top/gtcnjrtynj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.pycfn.com/gtiaiqbsnz.html

PHP:  // 无泛型
来源：http://hz.meibo888.top/gtfrbluqoz.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtadcnhehq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hysaishi.cn/gtlfhdzjtg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.bjfxy.top/gtlxygydea.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gtpfeddlut.html

Ruby: # 无泛型
来源：http://hz.yuanzhike.top/gttfznxwxa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtyfyfzqwc.html

[C15] 解构 / 展开参数
来源：http://hz.cheryme.top/gtlvhcmdwa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj202588.top/gtyfhnevuu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dashuyun.cn/gtkmlhixwf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtxfdysofu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtouuyiwyy.html

Java: // 无解构
来源：http://hz.dashuyun.cn/gtbbfbbvwr.html

Go:   // 无解构
来源：http://hz.jinqigfzy.top/gtnalenncq.html

Ruby: a, b = pair
来源：http://hz.nanxinkj.top/gtkekcuxpt.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtqlavuovg.html

[C16] 函数 / 方法重载
来源：http://hz.jianghu66.top/gtpqwyfsae.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gogol.net.cn/gtikqqxpkt.html

PHP:  // 无重载
来源：http://hz.nanxuanxn.top/gtmfjgekzj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.feifeiyinyue.top/gtidanzqzu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sufxvd.cn/gtkswjpnga.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangshuangyany.cn/gtbnkkuabt.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhiwuduotai.top/gtggoofiiz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtsvxbnpje.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtxatbildj.html

================================================================================
来源：http://hz.nanxinkj.top/gtbwmqnqyw.html

D. 数组 / 列表 / 集合
来源：http://hz.svipenyu.cn/gtcpjxsjjz.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttsnlnccn.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtowhbmybv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.meibo888.top/gtqpvxksga.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fzhhl.top/gtjtvbdxor.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gttqnqahod.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gttoexhahj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtrwwzjvsk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtcubedvqf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenzaomai.com/gtmnuqnebu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtcosvimwk.html

[D02] 追加元素到末尾
来源：http://hz.ivvv.top/gtznpnojym.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cqqwz.cn/gtcftzbudp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ivvv.top/gtwyctdrko.html

JS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtmnjgiubi.html

TS:   arr.push(4);
来源：http://hz.tanke756.top/gtiwgoyyad.html

Java: list.add(4);
来源：http://hz.havefunace.top/gtrfyorlta.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtnlhvxcjr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xziqi.cn/gtktoasqmu.html

C#:   list.Add(4);
来源：http://hz.ybcxt.top/gtdwbtbwvb.html

[D03] 在指定位置插入元素
来源：http://hz.yj202588.top/gtyylfjlal.html

Py:   arr.insert(0, 0)
来源：http://hz.jlsjyb.cn/gtphkebssp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ppjwa.cn/gtpvmjxdko.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnqzz.top/gtpkixvfpn.html


<!-- 参考信息 -->