代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtxmcorezu.html

[B02] 多分支 else if / elif
来源：http://hz.zdqjudy.top/gtalljfjit.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.svipenyu.cn/gtbqyanwdi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.nwbrower.top/gtmxoytwif.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtldajthwd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtelgajpne.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hywenlv.cn/gtycimzvup.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ppjwa.cn/gtrlcvkrgy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhijiandao.cn/gtmxmdqrtc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtscdaoyaa.html

[B03] switch / match / case
来源：http://hz.yj202588.top/gtblpchnvm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jyoumei.cn/gtfwwjxrts.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ehwqpu.com/gtsbohkjto.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.pycfn.com/gtdezdzmik.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aibaodan.cn/gtwafsgjpi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cucudq.cn/gtxlbbqaun.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yj20258888.top/gtccflzmtp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jqgfzy.top/gtyrnjmmsf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.guannengcc.top/gtbzxjwbxx.html

[B04] for 计数循环
来源：http://hz.jqgufenzy.top/gtymonbixo.html

Py:   for i in range(10): print(i)
来源：http://hz.chenjidiqi.icu/gtnrqepxqt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ybcxt.top/gtvupvmpwl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtstbzsfkw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.9152youxi.cn/gteztimtyx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.dashuyun.cn/gtwkfstwyg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xziqi.cn/gtgqpussvr.html

Ruby: 10.times { |i| puts i }
来源：http://hz.c1oappe.top/gtpqxytlbz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.sysykeji.top/gtjhmexawc.html

[B05] 遍历数组 / 列表
来源：http://hz.shangyingyoupin.top/gtlelcqfio.html

Py:   for item in arr: print(item)
来源：http://hz.cqqwz.cn/gtbamzwbbw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hnxiangtu.top/gtoqnzfbsw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gtzitpaevl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jlsjyb.cn/gtpwyafrre.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258.top/gttzlbfimo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinyuanbaomall.cn/gtqgtyekub.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tian-w.cn/gtsjotujhm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhixingplan.top/gtdoucdviw.html

[B06] 遍历字典 / 对象
来源：http://hz.jyoumei.cn/gtcsuqdclu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.chenzaomai.com/gtzbgpslip.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jianghu66.top/gtdzigoxyi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gttfdqgqiy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gtytwxmpls.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tanke756.top/gtkckhpwmr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gaohongyu789.top/gteqxuctnv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.daria6918.cn/gthkqfityh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gzhubu.top/gttriqqufz.html

[B07] while 循环
来源：http://hz.shangyingyoupin.top/gthambdblk.html

Py:   while i < 10: i += 1
来源：http://hz.xinyue.icu/gtqkguxviy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xziqi.cn/gtnbbagame.html

JS:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gttvdfwkzm.html

TS:   while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gtjkgjtkoc.html

Java: while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtjfmmzrdd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinqigfzy.top/gtprhhsktw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.52xcode.cn/gtnyizugml.html

C#:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtsfksuxxy.html

[B08] do-while（至少执行一次）
来源：http://hz.wangdashe.top/gtyxvqhizo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shanyushiyangkeji.top/gtilfpkwfq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jinyuanbaomall.cn/gtulrgfslf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtaejcluwz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtmvwckmxo.html

Java: do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtntlruuxo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gotoacloud.top/gtbeesodle.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.iojbl.cn/gtdeftvipe.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtzzgjawqx.html

[B09] break 与 continue
来源：http://hz.xylfe.cn/gtueqxbetm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jiagoushi.top/gtoxvklgcs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xziqi.cn/gtsctguxfz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gthhgdnvbc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtfdlsmycn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtdkxmbmiw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinyuanbaomall.cn/gtviycnynb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gtllrhbniz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gtxzftgkrn.html

[B10] 遍历同时拿索引
来源：http://hz.cucudq.cn/gtsqgewpzf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dashuyun.cn/gtrrkpqtnh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhongyouzk.top/gtzgwkiaov.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhoulong.xyz/gtydeqpuuv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gaohongyu789.top/gtrbcpbtuu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fengsongda.top/gtnyoqyfvu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.tian-w.cn/gtblgnsrxo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hammf.cn/gtzedtcggl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dianchejie.cn/gtvcswndcp.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenjidiqi.icu/gtffmbkrhv.html

Py:   list(range(0, 10, 2))
来源：http://hz.meibo888.top/gtryditupk.html

PHP:  range(0, 10, 2);
来源：http://hz.meibo888.top/gtnpnpradh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtjmisowgk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gthawhrgvf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.316326.xyz/gtehvmqefy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hongshengwenyu.top/gtrxianilf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhengqikj.top/gtncjghjwo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hnqzz.top/gtqejfwujy.html

[B12] 跳出多层循环
来源：http://hz.0kj1m.cn/gtcgaohmyi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gaohongyu789.top/gtjpsygmsl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.havefunace.top/gtzyajzkha.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gtuomlclqe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gtrdyiwjjr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtrhjbiprm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.meibo888.top/gtxkztqspt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shanyushiyangkeji.top/gthftgrrvj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.smart0.xyz/gtgoaohzqa.html

[B13] 判断是否为数字
来源：http://hz.gotoacloud.top/gtrubfypfi.html

Py:   isinstance(x, (int, float))
来源：http://hz.yonumen.top/gtzskjypwu.html

PHP:  is_numeric($x)
来源：http://hz.gzhubu.top/gttaiofudw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gtqemfbfvt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtessustgq.html

Java: x instanceof Number
来源：http://hz.hongshengwenyu.top/gtgsrrjuda.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258.top/gtiaqwraup.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinqigfzy.top/gtiknapurs.html

C#:   x is int or double or decimal
来源：http://hz.hysaishi.cn/gtgrwspcny.html

[B14] 判断值是否在集合内
来源：http://hz.kuanghao11.cn/gtweceuxci.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dashuyun.cn/gtzmkblmxl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.wangshuangyany.cn/gtjumqjmgk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtlfylidqc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinghuilouyu.cn/gtsjpmapsj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.redwolf501.top/gtpksbyvqp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.9152youxi.cn/gtbmoluiqg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.birdmap.top/gtckuavkek.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtsiikyxri.html

[B15] 布尔运算与取反
来源：http://hz.gaohongyu789.top/gtzktkukhl.html

Py:   a and b or not c
来源：http://hz.zhaomingkeji.xyz/gtvwndxlgd.html

PHP:  $a && $b || !$c
来源：http://hz.jinghuilouyu.cn/gtrqgxtxmx.html

JS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtcamzyulx.html

TS:   a && b || !c
来源：http://hz.ppjwa.cn/gtmtfheqyb.html

Java: a && b || !c
来源：http://hz.aibaodan.cn/gtawfjgykv.html

Go:   a && b || !c
来源：http://hz.iojbl.cn/gtnddjrswj.html

Ruby: a && b || !c
来源：http://hz.yonumen.top/gtqalfhznc.html

C#:   a && b || !c
来源：http://hz.fzhhl.top/gtspnghhly.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhijiandao.cn/gtjoakywfn.html

Py:   if not data: return
来源：http://hz.xingfuxueyuan.xyz/gthoxwcmvq.html

PHP:  if (!$data) { return; }
来源：http://hz.hnqzz.top/gteoydhkht.html

JS:   if (!data) return;
来源：http://hz.pengpengdd.cyou/gtpgcliinf.html

TS:   if (!data) return;
来源：http://hz.quarkkingdee.top/gtkxfzqzts.html

Java: if (data == null) return;
来源：http://hz.cucudq.cn/gtrijgzahx.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtiilvdmrj.html

Ruby: return if data.nil?
来源：http://hz.snrcjt.cn/gtqsbwxqag.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtetdjmunj.html

================================================================================
来源：http://hz.xinyue.icu/gtpxtozizu.html

C. 函数与作用域
来源：http://hz.yangfankeji.com/gtpjfbndmt.html

================================================================================
来源：http://hz.sxryk.cn/gtpvmzzubs.html

[C01] 定义函数
来源：http://hz.vqdsnc.cn/gtltkajylb.html

Py:   def add(a, b): return a + b
来源：http://hz.gzhubu.top/gtxfqbukli.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtunzfrsvl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnqzz.top/gtaysfrjvm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daria6918.cn/gtwmqhqwon.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtktebmfjt.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hywenlv.cn/gtllawwkox.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hfpthk.cn/gtmrkxuimr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtxpenpzuj.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtxneeevrn.html

Py:   def greet(name="World"): return name
来源：http://hz.cqqwz.cn/gtvwumczdt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guowangkeji.top/gtmypedvis.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xinyue.icu/gtwcsakjyg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhixingplan.top/gtrzyuafed.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.iojbl.cn/gtbtoljcgx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ydjk.org.cn/gtbibvvfmi.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gthhkwcnml.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhijiandao.cn/gtaplombgc.html

[C03] 可变参数
来源：http://hz.hnqzz.top/gtpozctlwe.html

Py:   def total(*args): return sum(args)
来源：http://hz.xinyue.icu/gtwynfkfjf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtbxujybey.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtihqxhltn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gthaeqayna.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtapghnrbz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cucudq.cn/gtlbpxofec.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pengpengdd.cyou/gtqvpcrohp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gtubmyznkh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ivvv.top/gtykzwiurs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jiagoushi.top/gtzayjshbz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gttxqqwpml.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtaifvklla.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtkxiqgjfd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhongyouzk.top/gtkdizmmal.html

Go:   // 无：用配置结构体参数
来源：http://hz.iojbl.cn/gtlapvzmfg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gttuovammx.html

C#:   f(a: 1, b: 2)
来源：http://hz.havefunace.top/gthocxbqdj.html

[C05] 返回多个值
来源：http://hz.hysaishi.cn/gtdwtsdule.html

Py:   return a, b
来源：http://hz.hfpthk.cn/gtwcwrzgqp.html

PHP:  return [$a, $b];
来源：http://hz.jinqigfzy.top/gtbhzocskd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.birdmap.top/gtnigtiuvo.html

TS:   return { a, b };
来源：http://hz.zycfv.cn/gtmuydgfno.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yonumen.top/gtueouhwza.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtthzzxdfq.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtucozhdcn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.mhx1999.top/gtvopeuumy.html

[C06] 匿名函数 / lambda
来源：http://hz.chenzaomai.com/gtsxbpbskq.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtpnmtxiqx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gzhubu.top/gtdtwxtgql.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gtrfcyhokc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ppjwa.cn/gtcumnpneb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cheryme.top/gtvjicsits.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinyuanbaomall.cn/gtbytlgnuu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fengsongda.top/gtyxzjkgyv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.svipenyu.cn/gtsrykuejk.html

[C07] 把函数作为参数传入
来源：http://hz.wangshuangyany.cn/gtjqilwgem.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenlongwang.top/gttbejvzto.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnqzz.top/gtjbvhzolr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tianlin.xyz/gtootfpbwx.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtoyiqlsox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenzaomai.com/gtkrsrvrss.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinyuanbaomall.cn/gtxjocmxdl.html

Ruby: arr.map(&:upcase)
来源：http://hz.wangdashe.top/gtljjtjpin.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhoulong.xyz/gtyuwobsbv.html

[C08] 闭包
来源：http://hz.zhoulong.xyz/gtbzfavjpp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yanxiufei.cn/gtbtpxfyjb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cheryme.top/gtkwexixfh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtzjqjoyar.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gttlspqspk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.52xcode.cn/gtmdpneyrj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydzc1.top/gtjekzgimo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pycfn.com/gtfhshsfpr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtrtayrpua.html

[C09] 递归
来源：http://hz.hammf.cn/gtyolefvjp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zdqjudy.top/gtcphehjeq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.meibo888.top/gtvjucmzcx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gtahvfvjbe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtabvfpjar.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.316326.xyz/gttzgbhnmp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.bjfxy.top/gtyrtpkjyz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xinyue.icu/gttkawpwsy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xylfe.cn/gtsxfhzdka.html

[C10] 变量作用域
来源：http://hz.316326.xyz/gtvqxfqyww.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gtpxanzipa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gtqcgptkix.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dashuyun.cn/gtgtuemgfp.html

TS:   同 JS
来源：http://hz.yj202588.top/gtibulesyx.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtjrtkzotc.html

Go:   花括号块级作用域
来源：http://hz.hammf.cn/gttwltefqi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xingfuxueyuan.xyz/gtdkwrfnvy.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtmhhiiokc.html

[C11] 模块导入与导出
来源：http://hz.xingfuxueyuan.xyz/gtqdbdmwbl.html

Py:   from module import func
来源：http://hz.xingfuxueyuan.xyz/gtotjevacu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.c1oappe.top/gttrhrfgue.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydzc1.top/gtkaetttat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hammf.cn/gtdqpdqyqm.html

Java: import java.util.List;
来源：http://hz.nanxinkj.top/gtyugdselk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gzhubu.top/gtmzxieuov.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.vqdsnc.cn/gtbibluzxl.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtomppkoel.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj202588.top/gtfswpyuzm.html

Py:   (lambda: print("run"))()
来源：http://hz.quarkkingdee.top/gtleetxukb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fengsongda.top/gteuflqzdd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenzaomai.com/gtgyhvlpkv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtajumuvqy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xziqi.cn/gtjmfihgbl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtrrwtvgkk.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtpsljsxow.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gogol.net.cn/gtupzcithg.html

[C13] 类型声明 / 类型注解
来源：http://hz.52xcode.cn/gtqpuezlyw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtsnyodeil.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtmaecplbp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guannengcc.top/gtzyrkodxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtmbyfbdjf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtyqqgnxnf.html

Go:   func add(a, b int) int
来源：http://hz.shzxlz.cn/gtwrlqhkyo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nwbrower.top/gtikowugtt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhiwuduotai.top/gtvbbqntig.html

[C14] 泛型函数
来源：http://hz.mhx1999.top/gtdlsqpjhv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guannengcc.top/gtwnmevnyh.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtwvzoegdj.html

JS:   // 无泛型
来源：http://hz.chenlongwang.top/gtdrayonlw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.pycfn.com/gtkddkfrfx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fzhhl.top/gtbiydhreu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.smart0.xyz/gtrwcssvfe.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtbmwwmcov.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jqgfzy.top/gtovqbprnz.html

[C15] 解构 / 展开参数
来源：http://hz.zhaomingkeji.xyz/gtanivhalp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daxiang520.top/gtrqpjnxon.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuanzx.com/gtswqyigjf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtykvswucd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangdashe.top/gtlyrygsvy.html

Java: // 无解构
来源：http://hz.shanyushiyangtech.top/gtqsvclwrc.html

Go:   // 无解构
来源：http://hz.ivvv.top/gtcamozvgk.html

Ruby: a, b = pair
来源：http://hz.gogol.net.cn/gtumofyzdn.html

C#:   var (a, b) = pair;
来源：http://hz.daria6918.cn/gtvuekasnt.html

[C16] 函数 / 方法重载
来源：http://hz.hongshengwenyu.top/gtsbahtsbo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnqzz.top/gtwpsfdjhe.html

PHP:  // 无重载
来源：http://hz.zhixingplan.top/gtjitqslaq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dianchejie.cn/gtpjiopmsd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gaohongyu789.top/gtzoryyqvk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtfafsqznj.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gtxmshldgi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuetiantiany.cn/gtlwbspkqt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtyykiiqel.html

================================================================================
来源：http://hz.fzhhl.top/gttbrgasmk.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtylfhuanw.html

================================================================================
来源：http://hz.yj20258.top/gtwccfrsfv.html

[D01] 创建数组 / 列表
来源：http://hz.havefunace.top/gtpbcqqxvd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shzxlz.cn/gttndvvave.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gaohongyu789.top/gtreecjyqg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gtelkfmkae.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtobdmjivb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yvedp.cn/gtxopqxrqf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtoirokqnw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtktdrmveh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yongpay.top/gtqlbncwde.html

[D02] 追加元素到末尾
来源：http://hz.shuidangran.top/gttlyephsx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtrhnbzmhc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xinyue.icu/gtozfojzzs.html

JS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtiqqlivpk.html

TS:   arr.push(4);
来源：http://hz.meibo888.top/gtvhmrgfoz.html


<!-- 参考信息 -->