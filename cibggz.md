代发 wailian999

[A26] 类型转换总览
来源：http://hz.cqqwz.cn/gtiwmvknzx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yvedp.cn/gtfaplojht.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cucudq.cn/gtorrqvhej.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yangfankeji.com/gthduwulby.html

TS:   Number() String() Boolean() x as number
来源：http://hz.mhx1999.top/gtkwgadqwu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.sweek.top/gtozbyhnsc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.xinyue.icu/gtqcnsikcq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.snrcjt.cn/gtxgtjrfam.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jinqigufen.top/gtwlhkmypf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtsljurzhy.html

B. 流程控制
来源：http://hz.haohaochexian.top/gtzhiubmyg.html

================================================================================
来源：http://hz.hnxiangtu.top/gthgsrwurs.html

[B01] 条件判断 if / else
来源：http://hz.ppjwa.cn/gtjjeegctx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.fzhhl.top/gtstwkiwsy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hnqzz.top/gtmhfefxuh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtlsmzghbv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hammf.cn/gtyyxspbbq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gtxhslndjb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.pengpengdd.cyou/gthgxsepxb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jiagoushi.top/gtwngdyhhm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtkfunkjba.html

[B02] 多分支 else if / elif
来源：http://hz.gaohongyu789.top/gtougcwpqb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.chenjidiqi.icu/gtfqolgcrc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.sysykeji.top/gteckuimxs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtyrlqvuoy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtfcoekysn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sufxvd.cn/gtajvjyoio.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.andypj.xyz/gtyijueeal.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.tanke756.top/gtnvzdkcoi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gthtaaosov.html

[B03] switch / match / case
来源：http://hz.xuetiantiany.cn/gtekabmzvk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yuxming.cn/gtlqpezxgo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gaohongyu789.top/gtukxngaxj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.kuanghao11.cn/gtkobacbeh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yangfankeji.com/gtnvzducyc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.0kj1m.cn/gtxwpfmhus.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.fzhhl.top/gtqpotcjih.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.haohaochexian.top/gtaafysbty.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cqqwz.cn/gtdoyrzkbl.html

[B04] for 计数循环
来源：http://hz.zycfv.cn/gtefooizop.html

Py:   for i in range(10): print(i)
来源：http://hz.sufxvd.cn/gtitrjbfdw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xuanzx.com/gtmutrukea.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.kuanghao11.cn/gtaqhiluve.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nanxinkj.top/gtxppnosfb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinyuanbaomall.cn/gtgwncpavs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cdnleiting.top/gtlbmmzeeb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yonumen.top/gtjbggizte.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.nanxuanxn.top/gtgjcfnlie.html

[B05] 遍历数组 / 列表
来源：http://hz.vqdsnc.cn/gtwlccxzmz.html

Py:   for item in arr: print(item)
来源：http://hz.zhoulong.xyz/gtcfdexeby.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenjidiqi.icu/gtbvmlfblw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtgtyfyumj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sysykeji.top/gtmizphwmg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.smart0.xyz/gtnlfybcmo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shuidangran.top/gtmkeewccf.html

Ruby: arr.each { |item| puts item }
来源：http://hz.52xcode.cn/gtoxpdiwxw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.bjfxy.top/gtrbhtnwdq.html

[B06] 遍历字典 / 对象
来源：http://hz.yanxiufei.cn/gtoussnueq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.9152youxi.cn/gtgqbkofjh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.smart0.xyz/gttnuqgfco.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nwbrower.top/gtwspyhzds.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuanzx.com/gtjqopjspd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhoulong.xyz/gtncwgzmqz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yongpay.top/gteclzlwze.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hysaishi.cn/gtuqgizwls.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.redwolf501.top/gtocwvheqs.html

[B07] while 循环
来源：http://hz.cheryme.top/gtrgkwplbd.html

Py:   while i < 10: i += 1
来源：http://hz.cdnleiting.top/gtfqnbbncj.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hnqzz.top/gtqrdqrznx.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtqejpgdfp.html

TS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtufohmdhy.html

Java: while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtnzxydhmw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xuanzx.com/gtbqjklarh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jyoumei.cn/gtupeazzbo.html

C#:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtycuflebe.html

[B08] do-while（至少执行一次）
来源：http://hz.wangshuangyany.cn/gtipziuchy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuetiantiany.cn/gtwiwzyurn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sufxvd.cn/gtanqpkjro.html

JS:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtxusytpdz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtiqscrdib.html

Java: do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtmftkamuy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cashguo.top/gtzbosfrql.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ivvv.top/gtjrdxprbs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtersyqcwi.html

[B09] break 与 continue
来源：http://hz.sufxvd.cn/gtetgmpevn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhaomingkeji.xyz/gtbxqixdpz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ydzc1.top/gtwgumvgyi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtnwrbsovk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtlwhrxbui.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtekdaromc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtbhlbymvl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jiagoushi.top/gtmpbmzibk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shuidangran.top/gtvgwdofgl.html

[B10] 遍历同时拿索引
来源：http://hz.hongshengwenyu.top/gtuibensol.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zycfv.cn/gtnethvmru.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtorjbzjyo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cqqwz.cn/gtfukarhdq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zdqjudy.top/gtrphdsejx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yvedp.cn/gtjciwkymt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinyuanbaomall.cn/gtlrswhvqu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ywan-chungtsiang.top/gtnknvuxcu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gotoacloud.top/gtapvtpxtp.html

[B11] 生成数字序列 / 区间
来源：http://hz.kuanghao11.cn/gtnxawvaux.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtwrvsnyya.html

PHP:  range(0, 10, 2);
来源：http://hz.gogol.net.cn/gtjycgbwvx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangkeji.top/gtgotjfgxz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gticolexmr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.pycfn.com/gtxurhzxue.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shangyingyoupin.top/gtckyidvib.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gttstqrcqw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.meibo888.top/gticwrhgue.html

[B12] 跳出多层循环
来源：http://hz.gaohongyu789.top/gtrqaejifq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.fzhhl.top/gtkhqutenq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtpzcpdnwz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtykwhsmtp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtafkmlkyc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtwujjbzzz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.316326.xyz/gtjdckmqte.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xingfuxueyuan.xyz/gtmmwksxzf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gtifivbvij.html

[B13] 判断是否为数字
来源：http://hz.yanxiufei.cn/gtbtdrysmv.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigfzy.top/gtkgtbrbwy.html

PHP:  is_numeric($x)
来源：http://hz.wangdashe.top/gtlyhxmyld.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xinyue.icu/gtntosobms.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtqaixoxoe.html

Java: x instanceof Number
来源：http://hz.smart0.xyz/gtfpecosad.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dianchejie.cn/gtbrvnwdrc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.iojbl.cn/gtszmkbsxz.html

C#:   x is int or double or decimal
来源：http://hz.hfpthk.cn/gtnacdlbnd.html

[B14] 判断值是否在集合内
来源：http://hz.cqqwz.cn/gtemjvvtvx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.quarkkingdee.top/gthywmiwzq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sweek.top/gtacgslnyv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtdmnwdccz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtkbypofeq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.meibo888.top/gtvtcqhvqv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xingfuxueyuan.xyz/gtqcurcazu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hammf.cn/gthbwlxtak.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtsuitygpe.html

[B15] 布尔运算与取反
来源：http://hz.zhixingplan.top/gtvcbptqvw.html

Py:   a and b or not c
来源：http://hz.gotoacloud.top/gtjuhnfvob.html

PHP:  $a && $b || !$c
来源：http://hz.hongshengwenyu.top/gtfnumbfkr.html

JS:   a && b || !c
来源：http://hz.sysykeji.top/gtaryageja.html

TS:   a && b || !c
来源：http://hz.kuanghao11.cn/gtbmbumewq.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtjperenes.html

Go:   a && b || !c
来源：http://hz.smart0.xyz/gtmpjaksol.html

Ruby: a && b || !c
来源：http://hz.cqqwz.cn/gtuiitccly.html

C#:   a && b || !c
来源：http://hz.hammf.cn/gtlblgrcbw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhijiandao.cn/gtogzrscyy.html

Py:   if not data: return
来源：http://hz.sxryk.cn/gtddxfoalb.html

PHP:  if (!$data) { return; }
来源：http://hz.daria6918.cn/gtoytppeae.html

JS:   if (!data) return;
来源：http://hz.ybcxt.top/gtmratiake.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtatewstfl.html

Java: if (data == null) return;
来源：http://hz.smart0.xyz/gtrrvjgipp.html

Go:   if data == nil { return }
来源：http://hz.hnxiangtu.top/gtadodxdtu.html

Ruby: return if data.nil?
来源：http://hz.dianchejie.cn/gtlxqxtdos.html

C#:   if (data == null) return;
来源：http://hz.xinyue.icu/gtvfrxeptb.html

================================================================================
来源：http://hz.ppjwa.cn/gtapvbqlze.html

C. 函数与作用域
来源：http://hz.hnxiangtu.top/gtsdjiwece.html

================================================================================
来源：http://hz.yj20258.top/gtuzvaarts.html

[C01] 定义函数
来源：http://hz.svipenyu.cn/gtacsacjso.html

Py:   def add(a, b): return a + b
来源：http://hz.cashguo.top/gtumbnmfsq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtthcivrxa.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gtanxaquux.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtxtevjtwg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtpfhwzfin.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sweek.top/gtmhrxruku.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daxiang520.top/gttisgqabv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ivvv.top/gtqzcdxcce.html

[C02] 默认参数
来源：http://hz.hysaishi.cn/gtiojoivop.html

Py:   def greet(name="World"): return name
来源：http://hz.hongshengwenyu.top/gtzhksfmpc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ppjwa.cn/gtqxycqypd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.316326.xyz/gtzgeeyxrj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aibaodan.cn/gtdwqovolp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhijiandao.cn/gtyawsleql.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gtbrryyrhe.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuetiantiany.cn/gtvlizgint.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.svipenyu.cn/gthfquhwqv.html

[C03] 可变参数
来源：http://hz.hfpthk.cn/gttnrvakco.html

Py:   def total(*args): return sum(args)
来源：http://hz.ivvv.top/gtxxquscvq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fzhhl.top/gtyiceigjg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtlxwnkzvu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gtcmptkjty.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fzhhl.top/gtvcspfqfq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.havefunace.top/gtbgreekpf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cashguo.top/gtsyeoliiu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtaahdqbhm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gtndnczlat.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.52xcode.cn/gtypycdpbg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.kuanghao11.cn/gtrjaltyfx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtnpuwclgv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangkeji.top/gtpphsotxg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tianlin.xyz/gtpoqnhbxm.html

Go:   // 无：用配置结构体参数
来源：http://hz.tanke756.top/gtdcgvigoy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtdrthfdhj.html

C#:   f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtacdkoogq.html

[C05] 返回多个值
来源：http://hz.c1oappe.top/gtavcgywgp.html

Py:   return a, b
来源：http://hz.aibaodan.cn/gtgjcwerfn.html

PHP:  return [$a, $b];
来源：http://hz.gaohongyu789.top/gtjzkwhqlb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhixingplan.top/gtbzsobmwh.html

TS:   return { a, b };
来源：http://hz.kuanghao11.cn/gtguvhpzcn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yongpay.top/gtghsiysay.html

Go:   return a, b
来源：http://hz.ywan-chungtsiang.top/gtkbxocxbm.html

Ruby: return a, b
来源：http://hz.zhengqikj.top/gtikkdfjqv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jiagoushi.top/gtsazkvrmt.html

[C06] 匿名函数 / lambda
来源：http://hz.fzhhl.top/gtlbeehvzk.html

Py:   square = lambda x: x * x
来源：http://hz.feifeiyinyue.top/gtcrjphtrm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenjidiqi.icu/gtskihtwsh.html

JS:   const square = x => x * x;
来源：http://hz.tanke756.top/gtsbpxmrqh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtztvdxdgb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shzxlz.cn/gtgasehlbj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ehwqpu.com/gtnvlzyotp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangtech.top/gtexplzqhu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.guowangkeji.top/gtutvyzlko.html

[C07] 把函数作为参数传入
来源：http://hz.zhaomingkeji.xyz/gtjelywxtx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hnqzz.top/gtwjovzqmm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.9152youxi.cn/gtrdhzgxxb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sweek.top/gtpdkocgzl.html

TS:   arr.map(String)
来源：http://hz.nanxuanxn.top/gthucjuyrs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xinyue.icu/gtimnjgfrl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhaomingkeji.xyz/gtuqlovgcf.html

Ruby: arr.map(&:upcase)
来源：http://hz.yanxiufei.cn/gtzmlhupaa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gtewpxhqld.html

[C08] 闭包
来源：http://hz.guowangkeji.top/gtybjhbloe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jiagoushi.top/gtabdrjlxh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.snrcjt.cn/gtfzblqqgy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtmvlyohuf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtgafbpqwr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhongyouzk.top/gthhqpupjk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.0kj1m.cn/gtapzxldrv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pengpengdd.cyou/gtzkusxgyx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtgdxliwnf.html

[C09] 递归
来源：http://hz.ivvv.top/gtblswljbn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.c1oappe.top/gtnhimqvxb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj202588.top/gtvqazwuho.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gtyijpnvwn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtezbwkoqt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gtaitlkgsq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhengqikj.top/gtlpjyiele.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtkiokdlxq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.quarkkingdee.top/gtvvfjhgsi.html

[C10] 变量作用域
来源：http://hz.ehwqpu.com/gtecenivhz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.haohaochexian.top/gtodcplrcx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gthvmlrzfl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigfzy.top/gtwjowdmbs.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtrsynwaqd.html

Java: 方法内为块级作用域
来源：http://hz.tanke756.top/gtuvxjasqf.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gtdvxvofuq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigufen.top/gtjrhjgovz.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtdtqhqxat.html

[C11] 模块导入与导出
来源：http://hz.xuanzx.com/gtccevyqob.html

Py:   from module import func
来源：http://hz.quarkkingdee.top/gtsdgykxak.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ywan-chungtsiang.top/gtpvfjgvyv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhijiandao.cn/gtripcaghj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtaekklblg.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gthvzdmdww.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.mhx1999.top/gtpfufoeeh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shzxlz.cn/gtjupmighq.html

C#:   using System.Text;
来源：http://hz.quarkkingdee.top/gtishenslz.html

[C12] 立即执行函数 IIFE
来源：http://hz.feifeiyinyue.top/gtcntwbkeq.html

Py:   (lambda: print("run"))()
来源：http://hz.ppjwa.cn/gtvmduryqu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258888.top/gtkpkhswwz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtfosywhpy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtgrffgorr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tian-w.cn/gtniuophyv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cashguo.top/gtrnfreqza.html

Ruby: -> { puts "run" }.call
来源：http://hz.daria6918.cn/gtdcykhvxn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinyuanbaomall.cn/gtsvcuaeyv.html

[C13] 类型声明 / 类型注解
来源：http://hz.guannengcc.top/gtylefxogy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhixingplan.top/gtggxlbkwl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtapcxrsnd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gttvnzflav.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gtkiadzpwi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtjytjiyhn.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gtsqurzeww.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ywan-chungtsiang.top/gtdeuukrgk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.0kj1m.cn/gtgqggalth.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtozvjfyvp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yvedp.cn/gtdgrihmaj.html

PHP:  // 无泛型
来源：http://hz.yj20258.top/gtjzjibtze.html

JS:   // 无泛型
来源：http://hz.ehwqpu.com/gtvbiyjhkx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtjmwqgens.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtpkdjsceb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.havefunace.top/gtghjdrzpx.html

Ruby: # 无泛型
来源：http://hz.haohaochexian.top/gtpxcjdwds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.c1oappe.top/gtgrdsbghf.html

[C15] 解构 / 展开参数
来源：http://hz.gzhubu.top/gtajortmcr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yangfankeji.com/gtegxdbkpz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtkdnpevce.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tanke756.top/gtqphvdiao.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigufen.top/gtrtgwoail.html

Java: // 无解构
来源：http://hz.yueranfly.top/gthvuuaxej.html

Go:   // 无解构
来源：http://hz.sxryk.cn/gtauralxtz.html

Ruby: a, b = pair
来源：http://hz.0kj1m.cn/gtoguhcfvr.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gtfpecyxsd.html

[C16] 函数 / 方法重载
来源：http://hz.nanxuanxn.top/gtjlgvoxrx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shuidangran.top/gtmvrcmnbm.html

PHP:  // 无重载
来源：http://hz.cucudq.cn/gtwmtszseb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daria6918.cn/gtttxjyuum.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.birdmap.top/gtxljufvus.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangtech.top/gtolejjowt.html


<!-- 参考信息 -->