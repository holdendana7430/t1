代发 wailian999

[A26] 类型转换总览
来源：http://hz.shuidangran.top/gtrdmrbgro.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenlongwang.top/gtcxfofhfe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.mhx1999.top/gtjjfcecxl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cqqwz.cn/gtaehrmceu.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ywan-chungtsiang.top/gtogtcxjfv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinyuanbaomall.cn/gttbrwhwmw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ybcxt.top/gtwtzgmrlx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xinyue.icu/gtlhfgeqfs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hywenlv.cn/gtjocfujbo.html

================================================================================
来源：http://hz.aizwys.cn/gtozqrxwob.html

B. 流程控制
来源：http://hz.ehwqpu.com/gtqjfwbeex.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbnjnmuap.html

[B01] 条件判断 if / else
来源：http://hz.cucudq.cn/gtwooygmbc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yueranfly.top/gthiqtpilo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.fzhhl.top/gtnukiycke.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yuxming.cn/gtvupqehud.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtptddcgqe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.iojbl.cn/gtfszjvfjl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.tianlin.xyz/gtdqelxhvq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yangfankeji.com/gtvjtbmlfo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gzhubu.top/gtktoqkguu.html

[B02] 多分支 else if / elif
来源：http://hz.sysykeji.top/gtsztuhvyv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gotoacloud.top/gtlffdfayb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.sufxvd.cn/gtwatebzrw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtwhmnybwf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sxryk.cn/gtrnabraka.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.mhx1999.top/gtvciysurd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sxryk.cn/gtthfkphpw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cheryme.top/gtxbqjdgqx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gthcvvqjmi.html

[B03] switch / match / case
来源：http://hz.aibaodan.cn/gtwoszzvdt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.wangshuangyany.cn/gtrtgglqto.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.dashuyun.cn/gtwtshwohg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shanyushiyangtech.top/gtzbirlqxl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daxiang520.top/gtwjwzhyln.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hnxiangtu.top/gtwqztzumx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.meibo888.top/gtfmjsdlci.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.dashuyun.cn/gtqscrzlrx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.birdmap.top/gtepzuuybi.html

[B04] for 计数循环
来源：http://hz.hnxiangtu.top/gtceiekaho.html

Py:   for i in range(10): print(i)
来源：http://hz.shanyushiyangtech.top/gtkxxpzdvb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.aibaodan.cn/gtzalcurlm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nwbrower.top/gttwaletdh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinqigfzy.top/gtsimtzzto.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhaomingkeji.xyz/gtxwjckprg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhoulong.xyz/gtuywbgglu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.52xcode.cn/gtdhetancn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tianlin.xyz/gtlhxxgtnf.html

[B05] 遍历数组 / 列表
来源：http://hz.shuidangran.top/gtqedzxubl.html

Py:   for item in arr: print(item)
来源：http://hz.hammf.cn/gtkujyjkxx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.aibaodan.cn/gtvacxsspq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tian-w.cn/gtthemawri.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj202588.top/gtvcatquog.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sxryk.cn/gtuqwuosde.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.fzhhl.top/gtkmnzhzje.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shzxlz.cn/gtpyamdbmu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.52xcode.cn/gtqxwmhmos.html

[B06] 遍历字典 / 对象
来源：http://hz.xziqi.cn/gtpsuvdhjz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ydzc1.top/gtqdkcrgfm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xingfuxueyuan.xyz/gtffigklvt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258888.top/gtzypwdgei.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yvedp.cn/gtlmqzsiay.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.wangdashe.top/gtuaxgqdlm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zycfv.cn/gtojrwiitu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shuidangran.top/gtblsntjhf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shangyingyoupin.top/gtsuexuzyw.html

[B07] while 循环
来源：http://hz.c1oappe.top/gtevajcjfj.html

Py:   while i < 10: i += 1
来源：http://hz.wangshuangyany.cn/gtenwkotrz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jiagoushi.top/gtpefwsxgt.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtmkfhfzhf.html

TS:   while (i < 10) { i++; }
来源：http://hz.fzhhl.top/gtkbziaron.html

Java: while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtfakvelgd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sufxvd.cn/gtrpfkvsbt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shanyushiyangtech.top/gtdfymdtgk.html

C#:   while (i < 10) { i++; }
来源：http://hz.bjfxy.top/gtmboqjenf.html

[B08] do-while（至少执行一次）
来源：http://hz.xuetiantiany.cn/gtllihjttw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.guannengcc.top/gtyicbotvu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.aizwys.cn/gtibzzljbp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtqwehroyc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtwvxnziyk.html

Java: do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtwlgjdiou.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.0kj1m.cn/gtykwlmmzb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jiagoushi.top/gtskeaejuv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtbnlkifxy.html

[B09] break 与 continue
来源：http://hz.pengpengdd.cyou/gtwstgubbg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jianghu66.top/gtsqsmmqgl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtjczrubki.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtyqkmtfdy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtfvzfencw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtcxmjdxze.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.havefunace.top/gtppxnmthd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xziqi.cn/gtdxexcabv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtdgrqkcow.html

[B10] 遍历同时拿索引
来源：http://hz.yvedp.cn/gtwtoduqmm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guannengcc.top/gtitzhqkxc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.redwolf501.top/gttwjnqueq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yanxiufei.cn/gtngpfbybl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtswotnlst.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.pengpengdd.cyou/gtmbxojuii.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.snrcjt.cn/gtvuzvloio.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.c1oappe.top/gtehnloudo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yvedp.cn/gtxawczsmc.html

[B11] 生成数字序列 / 区间
来源：http://hz.fengsongda.top/gtccyjzwkx.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtcfuzodbo.html

PHP:  range(0, 10, 2);
来源：http://hz.havefunace.top/gtjbzgkzdw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtgixjtyhf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnqzz.top/gtthbfyljz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangdashe.top/gtmohanajq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xinyue.icu/gtxjrlthsi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ehwqpu.com/gtgygmhcpd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhixingplan.top/gtxbebbpuz.html

[B12] 跳出多层循环
来源：http://hz.aibaodan.cn/gtnzdxciyx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shzxlz.cn/gtqcbltkui.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.nwbrower.top/gttbpvgbou.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtkxavfcto.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtsevsibcx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gthdrccjcg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yueranfly.top/gtwripznnm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.redwolf501.top/gtntjofamf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ywan-chungtsiang.top/gthlgcjwwd.html

[B13] 判断是否为数字
来源：http://hz.jinqigufen.top/gtqmfedwcp.html

Py:   isinstance(x, (int, float))
来源：http://hz.xylfe.cn/gtnrajrikl.html

PHP:  is_numeric($x)
来源：http://hz.tianlin.xyz/gtbopkvclb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtoufhjczl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtmyirekor.html

Java: x instanceof Number
来源：http://hz.aizwys.cn/gtwdnfgwfx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zdqjudy.top/gtiwfwmkou.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangkeji.top/gtigduhqoq.html

C#:   x is int or double or decimal
来源：http://hz.shuidangran.top/gtipinawyp.html

[B14] 判断值是否在集合内
来源：http://hz.meibo888.top/gtnnzovjui.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yongpay.top/gtghirqguz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtcjhbrumj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtkahpjwos.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtywwxujdu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxuanxn.top/gtfpohkyzr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.fengsongda.top/gtqqcukujp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cdnleiting.top/gtglwvsdjs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydzc1.top/gtmvglngop.html

[B15] 布尔运算与取反
来源：http://hz.yanxiufei.cn/gtpminzoav.html

Py:   a and b or not c
来源：http://hz.havefunace.top/gtsqnvinxw.html

PHP:  $a && $b || !$c
来源：http://hz.jinghuilouyu.cn/gtsrbigmlh.html

JS:   a && b || !c
来源：http://hz.zhongyouzk.top/gtkdyxneqz.html

TS:   a && b || !c
来源：http://hz.meibo888.top/gtnyscazmx.html

Java: a && b || !c
来源：http://hz.hnxiangtu.top/gtxdaawvox.html

Go:   a && b || !c
来源：http://hz.gaohongyu789.top/gtlqwmupkr.html

Ruby: a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtujxdfhrw.html

C#:   a && b || !c
来源：http://hz.dianchejie.cn/gttxdlmudv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xylfe.cn/gtwowvurql.html

Py:   if not data: return
来源：http://hz.wangshuangyany.cn/gtcnqsfrxz.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtjaliuogr.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtrwavernv.html

TS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtwrqpkwpv.html

Java: if (data == null) return;
来源：http://hz.tian-w.cn/gtkezmntvo.html

Go:   if data == nil { return }
来源：http://hz.hywenlv.cn/gtjrtxyskm.html

Ruby: return if data.nil?
来源：http://hz.zhijiandao.cn/gtrvnhdhgf.html

C#:   if (data == null) return;
来源：http://hz.chenlongwang.top/gtakwajusf.html

================================================================================
来源：http://hz.chenzaomai.com/gtbycwlsjm.html

C. 函数与作用域
来源：http://hz.gaohongyu789.top/gtrrrpeycd.html

================================================================================
来源：http://hz.zhengqikj.top/gtzyuoavjl.html

[C01] 定义函数
来源：http://hz.cdnleiting.top/gtfzwsalvm.html

Py:   def add(a, b): return a + b
来源：http://hz.yangfankeji.com/gtolzxgdag.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtzsgalxsi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.daxiang520.top/gtdgkkkhva.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtnvepjnis.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtybsnnhdp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.0kj1m.cn/gtkxyztbvc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gtnrsxpgro.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtbfnvxful.html

[C02] 默认参数
来源：http://hz.jinqigufen.top/gtolggmaqd.html

Py:   def greet(name="World"): return name
来源：http://hz.iojbl.cn/gtbucocilk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fzhhl.top/gtezkzlcpo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtetqvfjpf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.haohaochexian.top/gtwdegoiia.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.pengpengdd.cyou/gtxrtsyyhm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cucudq.cn/gtdczvhqme.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnqzz.top/gtrzndjsxp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gthbofkdaj.html

[C03] 可变参数
来源：http://hz.ywan-chungtsiang.top/gtncojrkum.html

Py:   def total(*args): return sum(args)
来源：http://hz.yonumen.top/gtprcmosom.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xinyue.icu/gtpdjjdxqm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtxvhwqwtu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gttqdnmtnl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.meibo888.top/gtvhooomsa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.havefunace.top/gtwrbkbycs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuxming.cn/gtyphkuxle.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gtljxxpkdw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gogol.net.cn/gthuzlkvdr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtqzoeleqj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtbtrclnep.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtwanzvgax.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtsfalmusc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258.top/gtmpsdmege.html

Go:   // 无：用配置结构体参数
来源：http://hz.meibo888.top/gtvmnuiczh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtjvuxasis.html

C#:   f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtijsyvlzq.html

[C05] 返回多个值
来源：http://hz.shangyingyoupin.top/gtkwbdzbnr.html

Py:   return a, b
来源：http://hz.yueranfly.top/gtjfaleota.html

PHP:  return [$a, $b];
来源：http://hz.yonumen.top/gtkogkpjgp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guowangkeji.top/gtzttzwusd.html

TS:   return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtukmaqpkg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gtcjgegzqz.html

Go:   return a, b
来源：http://hz.shanyushiyangkeji.top/gtqsvzljxx.html

Ruby: return a, b
来源：http://hz.jlsjyb.cn/gtsrilaeft.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gtjrpoylib.html

[C06] 匿名函数 / lambda
来源：http://hz.hysaishi.cn/gtnsuwfkhv.html

Py:   square = lambda x: x * x
来源：http://hz.xuetiantiany.cn/gtczytyuul.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pycfn.com/gtbkdlrtwi.html

JS:   const square = x => x * x;
来源：http://hz.redwolf501.top/gtggovxkzi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.mhx1999.top/gtaggaoiwc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sysykeji.top/gtvbncbcrt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.9152youxi.cn/gtdzijkzcn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinghuilouyu.cn/gtqcfcrgvr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtnguuhnye.html

[C07] 把函数作为参数传入
来源：http://hz.dianchejie.cn/gtasdnzqvw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yuanzhike.top/gtistmxzzb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtaiqmbvbj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cdnleiting.top/gtpjvldsvh.html

TS:   arr.map(String)
来源：http://hz.vqdsnc.cn/gtipjiqbuh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tian-w.cn/gtywnpadcz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.316326.xyz/gtqhxlfrjs.html

Ruby: arr.map(&:upcase)
来源：http://hz.mhx1999.top/gtgwoxjngf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydzc1.top/gtszolctrn.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtwsepzuei.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtjlhdnypw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtyjwysvig.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtjrnvwawf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtyjthunsh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtczwhvmyw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtejqdhlwt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ywan-chungtsiang.top/gthcfzphms.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtiuxscksw.html

[C09] 递归
来源：http://hz.yangfankeji.com/gtndyovkux.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtuiopxpqw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtiivtbbdz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gthekvtyod.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtjlizbwsa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yueranfly.top/gthiytwvua.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgfzy.top/gtrihxsjjp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtiefhnvou.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gtwljqihxl.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gtdviaipwc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhengqikj.top/gtryoxswch.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yonumen.top/gtchwufiqr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.52xcode.cn/gtouwzibyd.html

TS:   同 JS
来源：http://hz.xuanzx.com/gtypwpqnhr.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtchxyledt.html

Go:   花括号块级作用域
来源：http://hz.zhoulong.xyz/gtthnwafda.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pycfn.com/gtnvzmmqoc.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gtsvnfetoz.html

[C11] 模块导入与导出
来源：http://hz.shanyushiyangkeji.top/gtzwsaltzb.html

Py:   from module import func
来源：http://hz.nwbrower.top/gtaiymvuep.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jiagoushi.top/gtfmilzuam.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yangfankeji.com/gtvgokqzql.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zycfv.cn/gtstpkrxqt.html

Java: import java.util.List;
来源：http://hz.yongpay.top/gtomhzszln.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.c1oappe.top/gtenkifitp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cucudq.cn/gtzcvgknom.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtrgdssequ.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydzc1.top/gtdaujnsrc.html

Py:   (lambda: print("run"))()
来源：http://hz.shangyingyoupin.top/gtiwvmdewj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.meibo888.top/gtwtafxzpg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hammf.cn/gtocwxsoka.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtnhlwcasq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.9152youxi.cn/gtbclbxdcs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtshqudlvk.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtjsmemyye.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtxrzpgkxx.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhaomingkeji.xyz/gtklvegqhz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.c1oappe.top/gtdqmjsvln.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtzquiofco.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtxxuisnsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gteowvygfl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtahjnyaun.html

Go:   func add(a, b int) int
来源：http://hz.gogol.net.cn/gtuqymhegl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhengqikj.top/gteceakvdf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.haohaochexian.top/gtmlizzmcb.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtqtvifbti.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xinyue.icu/gtwjpfgkgn.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtynmtcoxd.html

JS:   // 无泛型
来源：http://hz.zhaomingkeji.xyz/gtzjeevqal.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.meibo888.top/gtujideufw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinyuanbaomall.cn/gtruitadty.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.iojbl.cn/gtewhxwjyz.html

Ruby: # 无泛型
来源：http://hz.xinyue.icu/gtiptjnyef.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtsnfutjae.html

[C15] 解构 / 展开参数
来源：http://hz.gaohongyu789.top/gtgvkpypar.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtuegluwtn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gtgyevjnwp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtzmknptvv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtjcvbhnxf.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtrsgekloc.html

Go:   // 无解构
来源：http://hz.zhijiandao.cn/gtatkumllt.html

Ruby: a, b = pair
来源：http://hz.wangdashe.top/gteuaobgbd.html

C#:   var (a, b) = pair;
来源：http://hz.ppjwa.cn/gtpyeyveep.html

[C16] 函数 / 方法重载
来源：http://hz.wangshuangyany.cn/gtvhiqubaa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.bjfxy.top/gtlhojjxrv.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtrilxsacu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gogol.net.cn/gtmzrhciqy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtjuyuhhiq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yonumen.top/gtajvpphzj.html


<!-- 参考信息 -->