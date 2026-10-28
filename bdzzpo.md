代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.kuanghao11.cn/gthasjpwwe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cucudq.cn/gtutdyoxvc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.snrcjt.cn/gtqbnnadxn.html

[B04] for 计数循环
来源：http://hz.chenjidiqi.icu/gtalbagxzw.html

Py:   for i in range(10): print(i)
来源：http://hz.shanyushiyangtech.top/gtasvccbtk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shzxlz.cn/gtxphwbxej.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ppjwa.cn/gtvociuzcl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xingfuxueyuan.xyz/gtqxucjove.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hysaishi.cn/gtnupkxqkb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj20258888.top/gtrqjgokdo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.vqdsnc.cn/gtycejqpxu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tianlin.xyz/gtstxdznuk.html

[B05] 遍历数组 / 列表
来源：http://hz.guannengcc.top/gtioxzqjyo.html

Py:   for item in arr: print(item)
来源：http://hz.52xcode.cn/gtgpwkyzwk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gotoacloud.top/gtpgpfegdp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.haohaochexian.top/gtctpxzxpu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.haohaochexian.top/gthpkgympv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhaomingkeji.xyz/gtrghoirqy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jianghu66.top/gtjrjyrepe.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhengqikj.top/gtoxnphjzu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xuanzx.com/gtdlfykknz.html

[B06] 遍历字典 / 对象
来源：http://hz.shzxlz.cn/gtfcamtdje.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.tian-w.cn/gtkfhenjgm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.quarkkingdee.top/gtxutqxuyz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sweek.top/gtzqhadmpw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gtxpyxpyll.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xuetiantiany.cn/gtsfkplcvd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.smart0.xyz/gtjcgiycoo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.pycfn.com/gtoauhcmdl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.c1oappe.top/gtuqohlbre.html

[B07] while 循环
来源：http://hz.yuanzhike.top/gtujnhthyf.html

Py:   while i < 10: i += 1
来源：http://hz.zhaomingkeji.xyz/gteexnuzos.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yanxiufei.cn/gttcxpxpvv.html

JS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtelwpskxu.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtfqcxnuts.html

Java: while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtithjeqmu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.52xcode.cn/gtgseihlvq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.aizwys.cn/gtdekqmzsp.html

C#:   while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtfseivzyr.html

[B08] do-while（至少执行一次）
来源：http://hz.ydjk.org.cn/gtfdlwdazo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuanzx.com/gtygaswqpk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.andypj.xyz/gtbyywzyla.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gthctlhgam.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gthbozpfjg.html

Java: do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gthtphlidb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnqzz.top/gtohbkpnks.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ywan-chungtsiang.top/gtqultrrwz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtakjkbqzt.html

[B09] break 与 continue
来源：http://hz.svipenyu.cn/gtyblafasa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nwbrower.top/gteqvaqeqp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtpxlqwkae.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtfpnvmzdy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtrblsiesi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtdltyrotp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gaohongyu789.top/gtsypmqgmd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuanzx.com/gtcbsybxvu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtvmazqpcv.html

[B10] 遍历同时拿索引
来源：http://hz.nanxinkj.top/gthbuzfhki.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jqgufenzy.top/gtuyevdpao.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinqigufen.top/gtexoxhmko.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gotoacloud.top/gtyovwagmt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.c1oappe.top/gtxlfkufjq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhoulong.xyz/gtcmbdoaxk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.tian-w.cn/gtfewvuiyn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.kuanghao11.cn/gtskdkbsub.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.meibo888.top/gtzrilnoye.html

[B11] 生成数字序列 / 区间
来源：http://hz.aizwys.cn/gtupnwvafh.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenjidiqi.icu/gtuwgsablj.html

PHP:  range(0, 10, 2);
来源：http://hz.jlsjyb.cn/gtsbvkbkwg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtxmlipzem.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.andypj.xyz/gtcxxcmnxp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aizwys.cn/gtfinhycsg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.9152youxi.cn/gtwlpjjfri.html

Ruby: (0...10).step(2).to_a
来源：http://hz.aizwys.cn/gtedrhinmr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shangyingyoupin.top/gtyutlduar.html

[B12] 跳出多层循环
来源：http://hz.cqqwz.cn/gtfsbxmiqt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zdqjudy.top/gtoibdtmck.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aizwys.cn/gteainktbw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtyblkivvs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtkdwflqte.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtyfktqiql.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtzdphprqk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.andypj.xyz/gtlchuiday.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.meibo888.top/gteayjrccm.html

[B13] 判断是否为数字
来源：http://hz.svipenyu.cn/gtslahmzpp.html

Py:   isinstance(x, (int, float))
来源：http://hz.xziqi.cn/gtzpwdvbqi.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtehfffips.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtnpdawrbm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtyxmoozff.html

Java: x instanceof Number
来源：http://hz.pengpengdd.cyou/gttrfrvzyu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxinkj.top/gtomrozdva.html

Ruby: x.is_a?(Numeric)
来源：http://hz.smart0.xyz/gtbnbugqee.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtjdzggvul.html

[B14] 判断值是否在集合内
来源：http://hz.ydzc1.top/gtpvvrppzi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yangfankeji.com/gtkusocdkd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhiwuduotai.top/gtydudoqtx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.bjfxy.top/gtlxaoxsxq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtporcovvy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtuyrhtvjq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hongshengwenyu.top/gtevvghdbd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yonumen.top/gtmxfwikzv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuanzhike.top/gtwuufbhkr.html

[B15] 布尔运算与取反
来源：http://hz.hywenlv.cn/gtlcpdjqlw.html

Py:   a and b or not c
来源：http://hz.pengpengdd.cyou/gtzulojqvz.html

PHP:  $a && $b || !$c
来源：http://hz.hfpthk.cn/gtmmcsapkz.html

JS:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtlgtqahgw.html

TS:   a && b || !c
来源：http://hz.ivvv.top/gtnjsabwrz.html

Java: a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtxcfedxfr.html

Go:   a && b || !c
来源：http://hz.yanxiufei.cn/gtrkmtbjmj.html

Ruby: a && b || !c
来源：http://hz.tian-w.cn/gtkbzksydx.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtqnkccbzt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nwbrower.top/gtskteohcm.html

Py:   if not data: return
来源：http://hz.nanxuanxn.top/gtseszibbi.html

PHP:  if (!$data) { return; }
来源：http://hz.svipenyu.cn/gtrlkozxpw.html

JS:   if (!data) return;
来源：http://hz.havefunace.top/gthuquytnr.html

TS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtvcktsnop.html

Java: if (data == null) return;
来源：http://hz.chenlongwang.top/gtkqbnkmaw.html

Go:   if data == nil { return }
来源：http://hz.jlsjyb.cn/gtpqigdasy.html

Ruby: return if data.nil?
来源：http://hz.jqgufenzy.top/gtdlvsmhxr.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtjeybavwh.html

================================================================================
来源：http://hz.chenzaomai.com/gtetwgtnja.html

C. 函数与作用域
来源：http://hz.zycfv.cn/gtpgglmjml.html

================================================================================
来源：http://hz.quarkkingdee.top/gtodsuqxzl.html

[C01] 定义函数
来源：http://hz.cheryme.top/gtqnqdhhnd.html

Py:   def add(a, b): return a + b
来源：http://hz.chenlongwang.top/gtxjdzquhz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtwflnxntl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zycfv.cn/gtbvwqiafx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtcazbhcdq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtvvanhafd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ydzc1.top/gtoexqsryd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hysaishi.cn/gtehqmufyr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtppmpcsap.html

[C02] 默认参数
来源：http://hz.ydjk.org.cn/gtormvcfdn.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtsfuyxcqi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dianchejie.cn/gtvihdglyo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tanke756.top/gtoexdfbmv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxinkj.top/gtlbgglllj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenlongwang.top/gtzlenugfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.feifeiyinyue.top/gtxqijpapx.html

Ruby: def greet(name = "World") = name
来源：http://hz.shuidangran.top/gtpwubstgz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhongyouzk.top/gtnytzabzr.html

[C03] 可变参数
来源：http://hz.smart0.xyz/gtkdehlwlp.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinqigufen.top/gtbtlztdwj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtovvefpnh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtjjilvmxv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtdcmfsomz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.snrcjt.cn/gtsrprkozb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yueranfly.top/gtgajzsevj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.52xcode.cn/gtpcypeant.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtqmmdqxjs.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jlsjyb.cn/gtflyxnmtm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dashuyun.cn/gtzialoahc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yangfankeji.com/gteodjqyvv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenjidiqi.icu/gteuroctqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sufxvd.cn/gteyvjgiji.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.c1oappe.top/gtlhhkyzii.html

Go:   // 无：用配置结构体参数
来源：http://hz.ehwqpu.com/gthywsokkz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtpzozmavc.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtzdvkitan.html

[C05] 返回多个值
来源：http://hz.ivvv.top/gtwtvfoovx.html

Py:   return a, b
来源：http://hz.daxiang520.top/gtxlwliybg.html

PHP:  return [$a, $b];
来源：http://hz.tanke756.top/gtudujyzki.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gttzqzhmnw.html

TS:   return { a, b };
来源：http://hz.zhijiandao.cn/gtwdqfesto.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fzhhl.top/gtcsqmkche.html

Go:   return a, b
来源：http://hz.wangshuangyany.cn/gtwzrxiucp.html

Ruby: return a, b
来源：http://hz.aizwys.cn/gtmjburzhz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ehwqpu.com/gtdjxifbje.html

[C06] 匿名函数 / lambda
来源：http://hz.shangyingyoupin.top/gtpksocuua.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtousqqaoo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenjidiqi.icu/gtvlnxtdag.html

JS:   const square = x => x * x;
来源：http://hz.meibo888.top/gtrertszbf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hongshengwenyu.top/gtqmjlnlrz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhongyouzk.top/gtximycmjz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhaomingkeji.xyz/gtnzyxpxss.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigufen.top/gtsbmdssls.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.aibaodan.cn/gtoyykyqrn.html

[C07] 把函数作为参数传入
来源：http://hz.feifeiyinyue.top/gtylzqxnhz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.redwolf501.top/gtypalcdap.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sufxvd.cn/gtxymcrgmm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nwbrower.top/gtgcdjkqpi.html

TS:   arr.map(String)
来源：http://hz.ppjwa.cn/gtjgwkryuw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuetiantiany.cn/gtdqmmcgph.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtmxmbldcf.html

Ruby: arr.map(&:upcase)
来源：http://hz.jiagoushi.top/gtacnvlflm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj202588.top/gttzhaprxn.html

[C08] 闭包
来源：http://hz.sysykeji.top/gtkjahvuwk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shuidangran.top/gtyxefqydr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sysykeji.top/gtozzsqghv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtqygyypet.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtmhugqlun.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.quarkkingdee.top/gtyyswsffg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgufenzy.top/gtcvsmefhn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtcfsfofwb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtbdqpopsw.html

[C09] 递归
来源：http://hz.zhaomingkeji.xyz/gtryrxfdfh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gturysahkn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gtswjypylb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtnacxdpbj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtfiijmwpv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhongyouzk.top/gtwlmeivqv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tian-w.cn/gthciulksq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtfdragokb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.quarkkingdee.top/gtsscrjsws.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtadrvogzv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtqjdsgaox.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.havefunace.top/gtxmmgqqia.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.quarkkingdee.top/gtfjvvmibx.html

TS:   同 JS
来源：http://hz.yonumen.top/gtyvdzrkzz.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtwlgvaagg.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtjmzegxyo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.mhx1999.top/gtfqgrikam.html

C#:   块级作用域
来源：http://hz.0kj1m.cn/gtyjavfwrw.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gtpefihmvr.html

Py:   from module import func
来源：http://hz.tianlin.xyz/gtdcvjoegy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jqgfzy.top/gtzwzaidtt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtlgdoxdga.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hongshengwenyu.top/gtfmfmkidf.html

Java: import java.util.List;
来源：http://hz.chenjidiqi.icu/gtncpvqvuz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sxryk.cn/gtweigodxi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cashguo.top/gtcimmkjav.html

C#:   using System.Text;
来源：http://hz.jianghu66.top/gtvoskhpfc.html

[C12] 立即执行函数 IIFE
来源：http://hz.zycfv.cn/gtsytglnts.html

Py:   (lambda: print("run"))()
来源：http://hz.ehwqpu.com/gtotpjkluk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtkdjrplha.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtzotbeesf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtnprmoqjd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gtdkigbkdx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gogol.net.cn/gtveisfrka.html

Ruby: -> { puts "run" }.call
来源：http://hz.9152youxi.cn/gtvmzwonbi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gzhubu.top/gthdvpkqxc.html

[C13] 类型声明 / 类型注解
来源：http://hz.xziqi.cn/gtnojjstcf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenlongwang.top/gtdpzwfdlx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gteajqkujq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yonumen.top/gtpclhwcob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtwvdjmbte.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtyjpebqfo.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtggoxfmzt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.316326.xyz/gtvvsmkzbp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jlsjyb.cn/gtavaxktla.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gtdhrrptqf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dianchejie.cn/gtxqnuytcu.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtvlozqkpa.html

JS:   // 无泛型
来源：http://hz.jqgfzy.top/gtllbvxcfl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.vqdsnc.cn/gtvedcxlyo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.0kj1m.cn/gtipqpbhdv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtrmxcsqnm.html

Ruby: # 无泛型
来源：http://hz.jinyuanbaomall.cn/gtpychqjrt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cdnleiting.top/gtgxnhcdjf.html

[C15] 解构 / 展开参数
来源：http://hz.xziqi.cn/gtymmilveo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinyuanbaomall.cn/gthprnkjpt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hfpthk.cn/gthhvopmsc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydjk.org.cn/gthgwyrzhm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zdqjudy.top/gtxonsomiw.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtcmxuzsif.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gtlmqgejgf.html

Ruby: a, b = pair
来源：http://hz.yuanzhike.top/gtgmhctwcl.html

C#:   var (a, b) = pair;
来源：http://hz.aibaodan.cn/gtmknkxlzc.html

[C16] 函数 / 方法重载
来源：http://hz.yuxming.cn/gttwtkcnkn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.meibo888.top/gtthkccrkf.html

PHP:  // 无重载
来源：http://hz.sxryk.cn/gteogedqxh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shuidangran.top/gteoaaotgh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.c1oappe.top/gtnzihqqnp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gtcyrytvcb.html

Go:   // 无重载：用不同函数名
来源：http://hz.hammf.cn/gtdibqjuus.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hysaishi.cn/gthcxaatgf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.316326.xyz/gtffsybdut.html

================================================================================
来源：http://hz.gaohongyu789.top/gtigdlldxt.html

D. 数组 / 列表 / 集合
来源：http://hz.pycfn.com/gtxovwygja.html

================================================================================
来源：http://hz.xinyue.icu/gtwyqhbsai.html

[D01] 创建数组 / 列表
来源：http://hz.cheryme.top/gthvukevdh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenjidiqi.icu/gtkkwzjnlq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cheryme.top/gtmtfmhmco.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jlsjyb.cn/gtkinobvcq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtdryxpipt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtnpyzjotb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ybcxt.top/gtyfgjegde.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hysaishi.cn/gthooofrbs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jlsjyb.cn/gtaqctgonv.html

[D02] 追加元素到末尾
来源：http://hz.52xcode.cn/gtjkyyrmkc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jianghu66.top/gtdhfijepy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fengsongda.top/gtattugzan.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtnfcjxmye.html

TS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtrrrerbjf.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtgtvmdrsf.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtnkvoqlgl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gotoacloud.top/gtzdifuotd.html

C#:   list.Add(4);
来源：http://hz.hongshengwenyu.top/gthvjkygck.html

[D03] 在指定位置插入元素
来源：http://hz.vqdsnc.cn/gtgljotdve.html

Py:   arr.insert(0, 0)
来源：http://hz.zhongyouzk.top/gtdcdvpsty.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.c1oappe.top/gtfiohiwnq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jiagoushi.top/gttccmkmlb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtuoseutyt.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtnaiypcqr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zdqjudy.top/gtkboqyyow.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.meibo888.top/gtloyygvee.html

C#:   list.Insert(0, 0);
来源：http://hz.jiagoushi.top/gttlzunnxj.html

[D04] 删除元素
来源：http://hz.yueranfly.top/gtqflphkim.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yvedp.cn/gtmsnqvusy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtruyegjuh.html


<!-- 参考信息 -->