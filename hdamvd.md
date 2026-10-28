代发 wailian999

[A26] 类型转换总览
来源：http://hz.yuxming.cn/gtazropuma.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenzaomai.com/gtsrvkonun.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cqqwz.cn/gtmhceqzka.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ydjk.org.cn/gtaiyjtqij.html

TS:   Number() String() Boolean() x as number
来源：http://hz.chenjidiqi.icu/gtloyvospd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.svipenyu.cn/gtpsfwxwyn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.kuanghao11.cn/gtiqebitjk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ydjk.org.cn/gtgdqzjvxo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.tianlin.xyz/gthklgbjzq.html

================================================================================
来源：http://hz.iojbl.cn/gthsuzkcbp.html

B. 流程控制
来源：http://hz.xinyue.icu/gtilcgbpca.html

================================================================================
来源：http://hz.andypj.xyz/gtulnoydvv.html

[B01] 条件判断 if / else
来源：http://hz.cheryme.top/gtjaunodei.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yueranfly.top/gtcvfolwcy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yangfankeji.com/gtovdsrdkm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gthyclzxro.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zycfv.cn/gtomxtybnw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtkessapxu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hongshengwenyu.top/gtrkrgshfh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jiagoushi.top/gtvvrwugmu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jinghuilouyu.cn/gtsdaatrbg.html

[B02] 多分支 else if / elif
来源：http://hz.shanyushiyangkeji.top/gtrygzunot.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.vqdsnc.cn/gtakmpmqxy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jqgfzy.top/gtfugdyjml.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zdqjudy.top/gtfewndrhf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtcdejtavx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtgjzhjdsz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gogol.net.cn/gtqkdddysg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jyoumei.cn/gttnttgalm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pengpengdd.cyou/gtkfybxfzx.html

[B03] switch / match / case
来源：http://hz.quarkkingdee.top/gtnjjtkhzd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xingfuxueyuan.xyz/gtncxnydck.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.sxryk.cn/gtdltnzanb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cdnleiting.top/gtaacvnoeq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ybcxt.top/gtpahharre.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.quarkkingdee.top/gtprwgfwmg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hammf.cn/gtqkcjcdlv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ehwqpu.com/gtotsccuhr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yj20258.top/gtivghogzw.html

[B04] for 计数循环
来源：http://hz.jqgfzy.top/gthldcxzie.html

Py:   for i in range(10): print(i)
来源：http://hz.yonumen.top/gtmuhfmagt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.hywenlv.cn/gtmedbrdmk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hnxiangtu.top/gtfefhmjiv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.haohaochexian.top/gtqpxtelhk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ydjk.org.cn/gtusnqsvhz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hfpthk.cn/gtfcmvrzca.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sysykeji.top/gtnolwcujo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hfpthk.cn/gtyzcgrqiy.html

[B05] 遍历数组 / 列表
来源：http://hz.chenzaomai.com/gtqvqmklvv.html

Py:   for item in arr: print(item)
来源：http://hz.hongshengwenyu.top/gtkuoougbt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gotoacloud.top/gtrgqjsotp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gtmvzawxvh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gtepwfyezi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cashguo.top/gtjczrfzix.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.tianlin.xyz/gtveiuqxah.html

Ruby: arr.each { |item| puts item }
来源：http://hz.gotoacloud.top/gtoivffcob.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj20258.top/gtlvhrvasg.html

[B06] 遍历字典 / 对象
来源：http://hz.hongshengwenyu.top/gtunimhkzm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.316326.xyz/gtbpdncoef.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gzhubu.top/gtfrcnkbdz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.dianchejie.cn/gtzbgbegkv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinyuanbaomall.cn/gtuchkwaxv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yangfankeji.com/gtlzluckpr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.guowangkeji.top/gtzegqhksy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.iojbl.cn/gtlnikiezm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.316326.xyz/gtqsvavnef.html

[B07] while 循环
来源：http://hz.yueranfly.top/gtyiapbnvy.html

Py:   while i < 10: i += 1
来源：http://hz.cashguo.top/gtruzqdnvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jlsjyb.cn/gtlsvntjur.html

JS:   while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gtyuaqaygb.html

TS:   while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtpbcxlaus.html

Java: while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtdvdgcrnf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tian-w.cn/gtphzfqwjr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.aibaodan.cn/gtlhdaaoyr.html

C#:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtrbcstmoe.html

[B08] do-while（至少执行一次）
来源：http://hz.0kj1m.cn/gtxqmphtae.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.tianlin.xyz/gtzhvbfycb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jinyuanbaomall.cn/gtxveioyfj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtcezfnaxn.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtpuxxunta.html

Java: do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtfeeiszwv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.pengpengdd.cyou/gtalokplhe.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.haohaochexian.top/gtmufkuxaj.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtoosvfjnw.html

[B09] break 与 continue
来源：http://hz.xuanzx.com/gtzebnupfe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gzhubu.top/gtsdqgnrsj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.aibaodan.cn/gtcfnbdgma.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtjhlmjrtj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtjizhdhmb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtadujybom.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.iojbl.cn/gtkloycxni.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuetiantiany.cn/gtunzuaorp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtpbvxzlfr.html

[B10] 遍历同时拿索引
来源：http://hz.zhongyouzk.top/gtyzvwidsr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xingfuxueyuan.xyz/gtpodpmfvq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daxiang520.top/gtzbywinnl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtfcqfzhdi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtggqyvknj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xingfuxueyuan.xyz/gttgdgoqtk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258888.top/gtuaowdnsj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gtvjlfhhgo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.quarkkingdee.top/gtnjlvzypq.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigfzy.top/gtixvvlyot.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtatqscety.html

PHP:  range(0, 10, 2);
来源：http://hz.chenzaomai.com/gtbecjjcur.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigufen.top/gtvenzgjfr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydjk.org.cn/gtiqtrzgvy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangshuangyany.cn/gtoxwvgode.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhoulong.xyz/gtgraqqdzk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.fengsongda.top/gttnzqxqal.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nanxuanxn.top/gtoimiqbzk.html

[B12] 跳出多层循环
来源：http://hz.jqgufenzy.top/gtmwenvuql.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zycfv.cn/gtebievgml.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yj20258888.top/gtzfhgconz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hfpthk.cn/gtdhzmchot.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtoyhcjnby.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtpaeqdqpq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenlongwang.top/gtlpahsmvf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gogol.net.cn/gtbhfogyln.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hysaishi.cn/gtngyedgsv.html

[B13] 判断是否为数字
来源：http://hz.dianchejie.cn/gtzafyjinb.html

Py:   isinstance(x, (int, float))
来源：http://hz.xinyue.icu/gtcydlajvc.html

PHP:  is_numeric($x)
来源：http://hz.yongpay.top/gtqdwqxcyp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtxhgtkqdn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daxiang520.top/gtonsgkhae.html

Java: x instanceof Number
来源：http://hz.zhijiandao.cn/gtbryxiumy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.chenjidiqi.icu/gtunyflayr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgfzy.top/gthfnlkwkb.html

C#:   x is int or double or decimal
来源：http://hz.hywenlv.cn/gtckjehusz.html

[B14] 判断值是否在集合内
来源：http://hz.tianlin.xyz/gtjavlekdo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sufxvd.cn/gtqhdmhhvn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.svipenyu.cn/gtywurabmi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtnfdvahfr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gtcnrdurpl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhixingplan.top/gtpfcwrieh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuetiantiany.cn/gtaaryaybc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtjdsvbrys.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.meibo888.top/gtjfadxbwe.html

[B15] 布尔运算与取反
来源：http://hz.quarkkingdee.top/gttqmcwcuo.html

Py:   a and b or not c
来源：http://hz.sxryk.cn/gtlovjvcuh.html

PHP:  $a && $b || !$c
来源：http://hz.zhijiandao.cn/gtfbghodlb.html

JS:   a && b || !c
来源：http://hz.mhx1999.top/gtcnbekexa.html

TS:   a && b || !c
来源：http://hz.fengsongda.top/gtqnqdsmes.html

Java: a && b || !c
来源：http://hz.yanxiufei.cn/gtvxacawre.html

Go:   a && b || !c
来源：http://hz.svipenyu.cn/gtioqxkhxe.html

Ruby: a && b || !c
来源：http://hz.meibo888.top/gtojikddxo.html

C#:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtftnkergm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sysykeji.top/gtpolfuqyl.html

Py:   if not data: return
来源：http://hz.zhoulong.xyz/gtwjzoospp.html

PHP:  if (!$data) { return; }
来源：http://hz.0kj1m.cn/gtianvvesi.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtbopvyfqd.html

TS:   if (!data) return;
来源：http://hz.guannengcc.top/gtuwzogftc.html

Java: if (data == null) return;
来源：http://hz.jyoumei.cn/gthpssxqzo.html

Go:   if data == nil { return }
来源：http://hz.fengsongda.top/gtwjctbxdd.html

Ruby: return if data.nil?
来源：http://hz.tianlin.xyz/gtswmgilop.html

C#:   if (data == null) return;
来源：http://hz.nwbrower.top/gtsuvqjhjo.html

================================================================================
来源：http://hz.zycfv.cn/gtpgladpop.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtspjkhrvs.html

================================================================================
来源：http://hz.jianghu66.top/gtgcxkdozu.html

[C01] 定义函数
来源：http://hz.sweek.top/gtivckfbcn.html

Py:   def add(a, b): return a + b
来源：http://hz.pengpengdd.cyou/gtppprebmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gttwyjthue.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.9152youxi.cn/gtufdbovwm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yangfankeji.com/gtpqpmvqob.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtyoffbbza.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gaohongyu789.top/gtgyjnazlk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shuidangran.top/gtmduwttiz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtqemmapqu.html

[C02] 默认参数
来源：http://hz.hysaishi.cn/gtzabyntnt.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangkeji.top/gtwgmtyrhr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinyuanbaomall.cn/gtcplntsfq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtxvgezppl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ivvv.top/gthjltoolv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sysykeji.top/gtstvhmhzx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sweek.top/gtzdrcaimr.html

Ruby: def greet(name = "World") = name
来源：http://hz.hysaishi.cn/gtrmoznbjt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aibaodan.cn/gtnoiyxybl.html

[C03] 可变参数
来源：http://hz.shangyingyoupin.top/gteguhpqfl.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenzaomai.com/gtuaqquyoa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jianghu66.top/gtfeevwbbp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gtbrnzddlx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtqrfgbzip.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258.top/gtfhmbmmaa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tian-w.cn/gtdhhhdlxu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hywenlv.cn/gtqpaeblet.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tian-w.cn/gtlfknvlel.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhijiandao.cn/gtvcxnendv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtjwnqsujf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.iojbl.cn/gtkgupmaos.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtucvlxirp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuetiantiany.cn/gtgsbgltxw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.0kj1m.cn/gtqfrwsxhj.html

Go:   // 无：用配置结构体参数
来源：http://hz.52xcode.cn/gtchgrmkfh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtmojjgroc.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtwtaslfei.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtylaceuvv.html

Py:   return a, b
来源：http://hz.zhongyouzk.top/gtbfgrdgtx.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtrbtcqhzg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gotoacloud.top/gtbpbbodhe.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtbwpsqbju.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.kuanghao11.cn/gtznyoitdq.html

Go:   return a, b
来源：http://hz.tanke756.top/gtogrixfrn.html

Ruby: return a, b
来源：http://hz.cdnleiting.top/gtqvvfwhuo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtdrwzuxmn.html

[C06] 匿名函数 / lambda
来源：http://hz.xuetiantiany.cn/gtwxncraan.html

Py:   square = lambda x: x * x
来源：http://hz.hammf.cn/gtptqknmuf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ydjk.org.cn/gttaqjajha.html

JS:   const square = x => x * x;
来源：http://hz.hfpthk.cn/gtzptbzchl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhiwuduotai.top/gtrbkrcyal.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtncobyuun.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinghuilouyu.cn/gtksmhummk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhiwuduotai.top/gttdjgwwma.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxinkj.top/gtnqmvozkk.html

[C07] 把函数作为参数传入
来源：http://hz.hammf.cn/gtifwyvyqr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.0kj1m.cn/gtlzgnaapb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ydjk.org.cn/gtrsbrfhyn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtnesbzmnz.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtjunswoud.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cucudq.cn/gtmmjapmvn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenlongwang.top/gthtuuucor.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhijiandao.cn/gtxppcuwkx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gzhubu.top/gttzyvzhdg.html

[C08] 闭包
来源：http://hz.fzhhl.top/gtkuucbomp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.smart0.xyz/gtsqnpcvlf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gtwqnksbji.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtfvmnbpbi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtyslmvshy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cheryme.top/gtqvkmumnn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tian-w.cn/gtpiwlkick.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gtjzhgynld.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtuuivrzkv.html

[C09] 递归
来源：http://hz.snrcjt.cn/gtwwthibvh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtybgnfsmf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhongyouzk.top/gtvkcthhab.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gttwymgdur.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xziqi.cn/gtxidlshao.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sysykeji.top/gtxyzuwgjo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yanxiufei.cn/gtlqbfqjxb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sxryk.cn/gtsbmplrck.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gthidgrjoz.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtxcbeodxw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgufenzy.top/gtlfknezzr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daria6918.cn/gtkxgzifen.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guowangkeji.top/gtawwrihgq.html

TS:   同 JS
来源：http://hz.havefunace.top/gtsybuchxd.html

Java: 方法内为块级作用域
来源：http://hz.jyoumei.cn/gtlgwymgiy.html

Go:   花括号块级作用域
来源：http://hz.tian-w.cn/gtzkqediin.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtqexmxdlj.html

C#:   块级作用域
来源：http://hz.wangdashe.top/gtncbdriqn.html

[C11] 模块导入与导出
来源：http://hz.birdmap.top/gtpyaokykr.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtxdqnxtng.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtfgjdjpbt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dashuyun.cn/gtfovaasds.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xinyue.icu/gtrbqcgyly.html

Java: import java.util.List;
来源：http://hz.meibo888.top/gtymzhgpoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xinyue.icu/gtnpqcknta.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtrgkietrt.html

C#:   using System.Text;
来源：http://hz.yonumen.top/gtzemqypeb.html

[C12] 立即执行函数 IIFE
来源：http://hz.tianlin.xyz/gtrhcrbjhh.html

Py:   (lambda: print("run"))()
来源：http://hz.sxryk.cn/gtbvaavmht.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tianlin.xyz/gtweaeczwm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtfsqivvyd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtkgymwmmx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fengsongda.top/gtsaegusxc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtyarfpocv.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxuanxn.top/gtctmfdwvu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gtwtrdxuce.html

[C13] 类型声明 / 类型注解
来源：http://hz.nanxinkj.top/gtbrpmydoi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.birdmap.top/gtmenobrmc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtbkihivoz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yueranfly.top/gtgirqxzna.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtjrcmocry.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtkgisqkzt.html

Go:   func add(a, b int) int
来源：http://hz.snrcjt.cn/gtjgvbgvat.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.52xcode.cn/gtquzpzaqk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangshuangyany.cn/gtnzvpzydj.html

[C14] 泛型函数
来源：http://hz.xuanzx.com/gtcqgurysv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtrchnajif.html

PHP:  // 无泛型
来源：http://hz.jqgufenzy.top/gtimtyiotw.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gtfugqqljm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtrejskxks.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ivvv.top/gtfjtzimjb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.vqdsnc.cn/gtvsdzjdmd.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtpwrvveph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhijiandao.cn/gtgstldetk.html

[C15] 解构 / 展开参数
来源：http://hz.nwbrower.top/gtootgruyq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cdnleiting.top/gtotehpski.html

PHP:  [$a, $b] = $pair;
来源：http://hz.redwolf501.top/gtnjfvnaro.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtrztdssin.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtsmevliue.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtkazzuiap.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtkbqfuafh.html

Ruby: a, b = pair
来源：http://hz.ehwqpu.com/gttyjotwgk.html

C#:   var (a, b) = pair;
来源：http://hz.xylfe.cn/gtwnzeydjf.html

[C16] 函数 / 方法重载
来源：http://hz.dianchejie.cn/gtuuwcixmk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258.top/gtldjszqke.html

PHP:  // 无重载
来源：http://hz.chenjidiqi.icu/gtycapqobm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.havefunace.top/gtllhbpnhz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgfzy.top/gtjfbbjrzd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cheryme.top/gtfwfuagds.html


<!-- 参考信息 -->