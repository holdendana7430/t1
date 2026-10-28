代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xinyue.icu/gtateyvppn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.kuanghao11.cn/gtpdbdruax.html

[B03] switch / match / case
来源：http://hz.xziqi.cn/gtooltvppg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jqgfzy.top/gtkaqjnghb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhiwuduotai.top/gtwqojdyvo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtccebbqug.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258888.top/gtmaramueu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.aizwys.cn/gtfdefcuux.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.gogol.net.cn/gteyzvjcrh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.daxiang520.top/gtexbixefg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.sysykeji.top/gtyzrvvcfi.html

[B04] for 计数循环
来源：http://hz.iojbl.cn/gtjbcwncxt.html

Py:   for i in range(10): print(i)
来源：http://hz.sxryk.cn/gtwlsrcbcu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ppjwa.cn/gtxdmptkly.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gtvvdssuso.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.guannengcc.top/gtufkfecky.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yuanzhike.top/gtxljcyqlw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinyuanbaomall.cn/gtwpevcbuo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinqigufen.top/gtdrepvdfl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zycfv.cn/gtpghvkzvv.html

[B05] 遍历数组 / 列表
来源：http://hz.cqqwz.cn/gtjjbuojlr.html

Py:   for item in arr: print(item)
来源：http://hz.yj202588.top/gtrwreneag.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhongyouzk.top/gtrpgmhivr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hysaishi.cn/gtkpcdsiyg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daria6918.cn/gtifdwvcid.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.birdmap.top/gtdjtdkebf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.meibo888.top/gtordgnwei.html

Ruby: arr.each { |item| puts item }
来源：http://hz.gogol.net.cn/gtkpgcbeuh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhijiandao.cn/gttnvvnxbr.html

[B06] 遍历字典 / 对象
来源：http://hz.fzhhl.top/gtjimaoqdf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ywan-chungtsiang.top/gtbnlabufk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinghuilouyu.cn/gtzpymjlxs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydzc1.top/gtfvcgwsyv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.mhx1999.top/gtwrjdpswh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.wangdashe.top/gtufnsqxja.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.guowangkeji.top/gtnvucombl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hammf.cn/gtxkgjepqk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinyuanbaomall.cn/gtodvnoziy.html

[B07] while 循环
来源：http://hz.wangshuangyany.cn/gtqfzhkjnh.html

Py:   while i < 10: i += 1
来源：http://hz.316326.xyz/gtjylyqihc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xylfe.cn/gtgxmmholt.html

JS:   while (i < 10) { i++; }
来源：http://hz.feifeiyinyue.top/gtywdauril.html

TS:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtfdrierhk.html

Java: while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtulmynhwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhixingplan.top/gteyyiiriz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.sxryk.cn/gtqiogeexm.html

C#:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtrwlhmzdo.html

[B08] do-while（至少执行一次）
来源：http://hz.nanxinkj.top/gtfoxroqcj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.kuanghao11.cn/gtrpravvvb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ybcxt.top/gtwdfzjozb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtylglmjeo.html

TS:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtkhpdxbeu.html

Java: do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gthgsvtlwn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj20258888.top/gtskpbtnqv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cucudq.cn/gtwpecsuvz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtsipogerj.html

[B09] break 与 continue
来源：http://hz.jlsjyb.cn/gtcdmdqzha.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.havefunace.top/gtrxtpmluu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.redwolf501.top/gtxiiwlnrw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtwioawkjg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtycyzczck.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtpiekmzaw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jiagoushi.top/gtzptqmadp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ivvv.top/gttzrjmqyb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtbpylemcc.html

[B10] 遍历同时拿索引
来源：http://hz.jiagoushi.top/gtofjzefss.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gogol.net.cn/gtheuitqyl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenzaomai.com/gtrvquenac.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hnxiangtu.top/gtdxhcasiz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhiwuduotai.top/gttsvojrjq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.chenzaomai.com/gtiyxeukox.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangshuangyany.cn/gthgicnnnd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yongpay.top/gthddnzcii.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.chenzaomai.com/gtqchhjesz.html

[B11] 生成数字序列 / 区间
来源：http://hz.gogol.net.cn/gtcmsuisrh.html

Py:   list(range(0, 10, 2))
来源：http://hz.yuanzhike.top/gtktkciriy.html

PHP:  range(0, 10, 2);
来源：http://hz.pycfn.com/gtrzxrgjsk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtoqzfuhuy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtpbvimhtf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shanyushiyangtech.top/gtysemshaa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.nwbrower.top/gtpytzftwl.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yvedp.cn/gtusgnbqja.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yongpay.top/gtnydnciyt.html

[B12] 跳出多层循环
来源：http://hz.iojbl.cn/gtfpwivfsa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shanyushiyangkeji.top/gtukqsvkdx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.andypj.xyz/gttuvgisla.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtlfbnhlqa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtamntlmzf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtiiarjsql.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shangyingyoupin.top/gtbgescfhh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.bjfxy.top/gtbfbxwiad.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gotoacloud.top/gtwzokmsnb.html

[B13] 判断是否为数字
来源：http://hz.shangyingyoupin.top/gtusuqtpyc.html

Py:   isinstance(x, (int, float))
来源：http://hz.xylfe.cn/gtqkmvxcts.html

PHP:  is_numeric($x)
来源：http://hz.tian-w.cn/gtgskwbarq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yanxiufei.cn/gtggcprevm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtnczppygp.html

Java: x instanceof Number
来源：http://hz.zhongyouzk.top/gtlveqiyly.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtukybxhtx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xinyue.icu/gtpltzaein.html

C#:   x is int or double or decimal
来源：http://hz.xinyue.icu/gtnigippku.html

[B14] 判断值是否在集合内
来源：http://hz.zhijiandao.cn/gtcrfbuifj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ywan-chungtsiang.top/gtpjrjzojg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xinyue.icu/gtoqiybrpj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhaomingkeji.xyz/gtavvhnjln.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yuanzhike.top/gtowcaaufn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.birdmap.top/gtlfsvinfm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xylfe.cn/gthisjxxew.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pengpengdd.cyou/gtwmhvtptk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sweek.top/gtrxbkuixm.html

[B15] 布尔运算与取反
来源：http://hz.chenlongwang.top/gtnnozxtkf.html

Py:   a and b or not c
来源：http://hz.zhongyouzk.top/gtogfyztkh.html

PHP:  $a && $b || !$c
来源：http://hz.kuanghao11.cn/gtrsnebsrq.html

JS:   a && b || !c
来源：http://hz.cheryme.top/gtngionjtm.html

TS:   a && b || !c
来源：http://hz.bjfxy.top/gtunriedjd.html

Java: a && b || !c
来源：http://hz.ppjwa.cn/gtmnmhjfaf.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gtvmjjwqtr.html

Ruby: a && b || !c
来源：http://hz.svipenyu.cn/gtylodasrt.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gtmuwgzlos.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yangfankeji.com/gtvejwyqid.html

Py:   if not data: return
来源：http://hz.jinqigfzy.top/gtzbmbtfdj.html

PHP:  if (!$data) { return; }
来源：http://hz.xuanzx.com/gtfxmevdhb.html

JS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtwqrrhbzp.html

TS:   if (!data) return;
来源：http://hz.zhijiandao.cn/gtvbjpiwpg.html

Java: if (data == null) return;
来源：http://hz.jinqigufen.top/gtgafqzfkt.html

Go:   if data == nil { return }
来源：http://hz.yuxming.cn/gtxalysfbs.html

Ruby: return if data.nil?
来源：http://hz.zhixingplan.top/gtpnppufzt.html

C#:   if (data == null) return;
来源：http://hz.iojbl.cn/gtbtypffpm.html

================================================================================
来源：http://hz.tian-w.cn/gtqxxgahxf.html

C. 函数与作用域
来源：http://hz.jlsjyb.cn/gtzzkwtome.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuhpzoyhb.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtcellkbnt.html

Py:   def add(a, b): return a + b
来源：http://hz.daxiang520.top/gteybpfquv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gteobnzqix.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.52xcode.cn/gtghmxynog.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtyguxsltx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gthbxwogcu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yonumen.top/gtccknldmt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.fengsongda.top/gtacjorscl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtrhghofjl.html

[C02] 默认参数
来源：http://hz.zhiwuduotai.top/gtymlurqsg.html

Py:   def greet(name="World"): return name
来源：http://hz.fzhhl.top/gtjskwuypo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ehwqpu.com/gtzovanqiv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gttueyeevl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj202588.top/gtivoujndp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.svipenyu.cn/gtgbcsqisy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxinkj.top/gttdrodght.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhixingplan.top/gtmnwntqzz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.daria6918.cn/gtkfjyeesq.html

[C03] 可变参数
来源：http://hz.feifeiyinyue.top/gtdeqjywuy.html

Py:   def total(*args): return sum(args)
来源：http://hz.ywan-chungtsiang.top/gtcikpomyh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenlongwang.top/gtokomdzzt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtzhfwdxtw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtplqveppm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tian-w.cn/gtoxhszowj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhixingplan.top/gtdjkggjfl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.daria6918.cn/gtsirmqpca.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydjk.org.cn/gtlitbfict.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtwexgaukn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yvedp.cn/gtkcipegng.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gtqchmsqku.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtprwscizm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.aibaodan.cn/gtvshpootz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gzhubu.top/gtgaqorenk.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtgkysgigg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtnxdqzpkf.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtlrewlltx.html

[C05] 返回多个值
来源：http://hz.316326.xyz/gticokatjy.html

Py:   return a, b
来源：http://hz.xuanzx.com/gtzvxwvydq.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtdbgcdcup.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ppjwa.cn/gtmjsoxzqt.html

TS:   return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtadkbujlg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ehwqpu.com/gttzgmulhb.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtezvwukli.html

Ruby: return a, b
来源：http://hz.sysykeji.top/gtbmhivbkr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ppjwa.cn/gtiwjsshaa.html

[C06] 匿名函数 / lambda
来源：http://hz.xuetiantiany.cn/gtkgkiuevk.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigufen.top/gtpfzdqcck.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ydjk.org.cn/gtjuvluwpr.html

JS:   const square = x => x * x;
来源：http://hz.hysaishi.cn/gtlhxwlzkj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhijiandao.cn/gtnytuobyv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtqqbalxcf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.meibo888.top/gtnuffyvkd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhijiandao.cn/gtyhgybmsi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yanxiufei.cn/gthfpusvvh.html

[C07] 把函数作为参数传入
来源：http://hz.gaohongyu789.top/gtqyxzljcv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258.top/gtojzoczev.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tanke756.top/gtdwybjqkj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yanxiufei.cn/gtefhhkpwm.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gtcvkpjhay.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangdashe.top/gttegetspe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pycfn.com/gttqaxrnud.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtptkjnozj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.quarkkingdee.top/gtdprgowns.html

[C08] 闭包
来源：http://hz.sysykeji.top/gtylcfmdwe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhiwuduotai.top/gtxmragnvd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigfzy.top/gturtdhdhf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtqnvfptqn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtvxzdihpo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jianghu66.top/gthatjmnsj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gtcroixupg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yueranfly.top/gtjesoymqi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtezxjixsk.html

[C09] 递归
来源：http://hz.zhixingplan.top/gtnaysvodi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.bjfxy.top/gtwjxdgdhh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cashguo.top/gtrthrsdsu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangdashe.top/gtwrfbunoe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtkmuytizj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtzjycopjh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cucudq.cn/gtaqsxctjz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cucudq.cn/gtaimrlahd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.andypj.xyz/gttpisbdpd.html

[C10] 变量作用域
来源：http://hz.yonumen.top/gtncxambjq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.c1oappe.top/gtptlswesy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xingfuxueyuan.xyz/gtpqsmjozg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenzaomai.com/gtvrkjxajo.html

TS:   同 JS
来源：http://hz.ybcxt.top/gtjzknvilj.html

Java: 方法内为块级作用域
来源：http://hz.yj202588.top/gtwuvtuiih.html

Go:   花括号块级作用域
来源：http://hz.zhengqikj.top/gtqktmcsyt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daxiang520.top/gtqjemzvwa.html

C#:   块级作用域
来源：http://hz.smart0.xyz/gtkqfrqvqi.html

[C11] 模块导入与导出
来源：http://hz.shuidangran.top/gtohlcjzcz.html

Py:   from module import func
来源：http://hz.ybcxt.top/gtaeqnrkmg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sxryk.cn/gtkcnvboky.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cheryme.top/gteiuukpks.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtzbkjhrki.html

Java: import java.util.List;
来源：http://hz.cashguo.top/gtbvsbmdly.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ywan-chungtsiang.top/gtfdpvnwvm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxuanxn.top/gtajcbcetc.html

C#:   using System.Text;
来源：http://hz.hfpthk.cn/gthkfjqjvh.html

[C12] 立即执行函数 IIFE
来源：http://hz.vqdsnc.cn/gtkoubhxin.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgufenzy.top/gtnlriihxf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cheryme.top/gtzsbhcxvv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtyipyeuud.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtdtigfvws.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cheryme.top/gtbepisbry.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.vqdsnc.cn/gtyzvlwmhk.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigfzy.top/gtvaqcqqjz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pengpengdd.cyou/gtpnhcwpxz.html

[C13] 类型声明 / 类型注解
来源：http://hz.yanxiufei.cn/gttourilzt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gogol.net.cn/gtctjserxm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gturlegtgi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tian-w.cn/gtdlslhxqt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtevgsdxet.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtgebulgbg.html

Go:   func add(a, b int) int
来源：http://hz.zhiwuduotai.top/gtsgaqxreg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangkeji.top/gtemtogxfo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shuidangran.top/gtnptvhazg.html

[C14] 泛型函数
来源：http://hz.tianlin.xyz/gtxhylhryu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.52xcode.cn/gtoemyzrej.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtwooctydb.html

JS:   // 无泛型
来源：http://hz.nanxuanxn.top/gtlljtwezl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtkagdmkmi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtjmwnotht.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sufxvd.cn/gtymmunktc.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gttlqfmhrj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtissaifsy.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtseikwixo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yonumen.top/gtlzujqyeo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtlzaathgg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtfjhhmplm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ppjwa.cn/gtwztwwwks.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtrhzmmtsa.html

Go:   // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtagsfgytg.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtpvbccbex.html

C#:   var (a, b) = pair;
来源：http://hz.fengsongda.top/gtuhpzarvz.html

[C16] 函数 / 方法重载
来源：http://hz.jqgufenzy.top/gttrjhjyph.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yonumen.top/gtukvgwiyw.html

PHP:  // 无重载
来源：http://hz.hammf.cn/gttwiusudc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jyoumei.cn/gtlgwmxnnl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xingfuxueyuan.xyz/gtjqoxalac.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yongpay.top/gtfrjyqsfo.html

Go:   // 无重载：用不同函数名
来源：http://hz.ehwqpu.com/gtqrpjwvsf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenlongwang.top/gtlfrekczj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aizwys.cn/gtmgrybwkh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtltwnuynz.html

D. 数组 / 列表 / 集合
来源：http://hz.andypj.xyz/gteiaqmbna.html

================================================================================
来源：http://hz.ybcxt.top/gtrdubewhe.html

[D01] 创建数组 / 列表
来源：http://hz.pycfn.com/gtoljyvajm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.aibaodan.cn/gtouhxcszh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nwbrower.top/gtboicipju.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shangyingyoupin.top/gtxfvxbjnk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.svipenyu.cn/gtkrwpwaum.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yonumen.top/gtaahmznbj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuanzhike.top/gtldoieuht.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtplspcswf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhijiandao.cn/gtpvphtftq.html

[D02] 追加元素到末尾
来源：http://hz.sysykeji.top/gthwpbyuhp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.dashuyun.cn/gttxgafkjx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.52xcode.cn/gtqbhzhpuq.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gtkicjzgbt.html

TS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtkjognrdy.html

Java: list.add(4);
来源：http://hz.guannengcc.top/gtlawhbkwf.html

Go:   arr = append(arr, 4)
来源：http://hz.yonumen.top/gtsptuaaiu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pengpengdd.cyou/gtjuethuac.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtmjivupqf.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtdsvpylqp.html

Py:   arr.insert(0, 0)
来源：http://hz.nwbrower.top/gtwiqhuipy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jyoumei.cn/gtxdycqlzo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj202588.top/gthiacndhf.html


<!-- 参考信息 -->