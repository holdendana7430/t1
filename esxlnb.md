代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinghuilouyu.cn/gtnmdyuawk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cheryme.top/gtxnonjvjf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gaohongyu789.top/gtvmlnotag.html

[B04] for 计数循环
来源：http://hz.cheryme.top/gtkvzhvmiy.html

Py:   for i in range(10): print(i)
来源：http://hz.feifeiyinyue.top/gthqanvtcv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.nwbrower.top/gtgmirsraj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhixingplan.top/gtynukzszb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinqigfzy.top/gthoaisxvk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sysykeji.top/gtccdbbrfk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jlsjyb.cn/gtnijnuuiq.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cheryme.top/gtwqmvsyhv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hnqzz.top/gtvqdgavbp.html

[B05] 遍历数组 / 列表
来源：http://hz.yuxming.cn/gtodmxzhgt.html

Py:   for item in arr: print(item)
来源：http://hz.fengsongda.top/gtrzzjsqls.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.iojbl.cn/gtgetxtudc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yvedp.cn/gtcwbgkgsr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.havefunace.top/gtafsjxbmz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cucudq.cn/gtetxecvnu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shanyushiyangkeji.top/gtvzvhlxlu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.dianchejie.cn/gtxqpuksnv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sysykeji.top/gtgbjemcnq.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gtfeyzdxyu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhongyouzk.top/gtumrseueg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shangyingyoupin.top/gtbsauwipq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhijiandao.cn/gtspfushkt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtysyvedxm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aizwys.cn/gtbkcqnret.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.mhx1999.top/gtrpnxozbi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sysykeji.top/gtfeanphel.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sxryk.cn/gtcjiwzyxc.html

[B07] while 循环
来源：http://hz.yongpay.top/gthxpyeifx.html

Py:   while i < 10: i += 1
来源：http://hz.wangdashe.top/gtszgwjjgf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.mhx1999.top/gtnbgbyobq.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtcibgydhg.html

TS:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtzmsptjau.html

Java: while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtcrgwgshd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.kuanghao11.cn/gtcmfdfokk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.gogol.net.cn/gtjidrxbfn.html

C#:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtwkbigtdp.html

[B08] do-while（至少执行一次）
来源：http://hz.jqgufenzy.top/gtucltwcae.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.haohaochexian.top/gtokwvgkaz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.mhx1999.top/gtcxjcscjm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtatyzyvwt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtqnutodxn.html

Java: do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtkxbsdhdu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cdnleiting.top/gtsmnhiiif.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hfpthk.cn/gtlqshitfr.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtnevlnfwr.html

[B09] break 与 continue
来源：http://hz.gzhubu.top/gtskzxfmwi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.iojbl.cn/gtghocgbit.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.andypj.xyz/gtcggkntue.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtefxiscrr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtavdcuoxs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtcnqhvcbx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenzaomai.com/gteruxfxol.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hnqzz.top/gtcuiiwkcp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtmfpulgjz.html

[B10] 遍历同时拿索引
来源：http://hz.snrcjt.cn/gtlmwwgfxo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zdqjudy.top/gtkgguhgjs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.nwbrower.top/gtkdjkound.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.haohaochexian.top/gtpyfndocv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xziqi.cn/gtbodfomsp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zycfv.cn/gtgantjadx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangdashe.top/gtxhghuyan.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hongshengwenyu.top/gtlyghknbn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangkeji.top/gtpiqgtrit.html

[B11] 生成数字序列 / 区间
来源：http://hz.316326.xyz/gtuglwijwl.html

Py:   list(range(0, 10, 2))
来源：http://hz.guowangkeji.top/gtnglmehhx.html

PHP:  range(0, 10, 2);
来源：http://hz.yj20258.top/gtazcojbqh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtekpdzrpp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sysykeji.top/gtpotybuuh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.9152youxi.cn/gtggwadxvi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.havefunace.top/gtvrtoobnf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinghuilouyu.cn/gtutlcbfoc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tian-w.cn/gtjhajydfy.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangkeji.top/gthehfnkyw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.birdmap.top/gtgqjjpdsb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.redwolf501.top/gtpcatexqv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yangfankeji.com/gtvroecdsu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtkcodskkk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtfpfpabax.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhixingplan.top/gtvyludyhl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhixingplan.top/gtfzmhqeqk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gaohongyu789.top/gttiezjsie.html

[B13] 判断是否为数字
来源：http://hz.shanyushiyangkeji.top/gtoqapefaa.html

Py:   isinstance(x, (int, float))
来源：http://hz.iojbl.cn/gtavvnpcfx.html

PHP:  is_numeric($x)
来源：http://hz.hysaishi.cn/gtziqpvuya.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dianchejie.cn/gtsrppaxvr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.svipenyu.cn/gtdiloaslt.html

Java: x instanceof Number
来源：http://hz.dashuyun.cn/gtngtcgaln.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gtazzpftut.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gogol.net.cn/gtsecguins.html

C#:   x is int or double or decimal
来源：http://hz.haohaochexian.top/gtooyockwy.html

[B14] 判断值是否在集合内
来源：http://hz.shzxlz.cn/gtotglyzhy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cdnleiting.top/gtxgkrnkqf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gaohongyu789.top/gtpihdikyl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtafhpsjxk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtmfoxlmdc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jyoumei.cn/gtrzgrjwye.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ehwqpu.com/gtmeskpwli.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hysaishi.cn/gtupciiiwm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenlongwang.top/gtujeofqwy.html

[B15] 布尔运算与取反
来源：http://hz.andypj.xyz/gtwcgeqqhk.html

Py:   a and b or not c
来源：http://hz.xylfe.cn/gtmlucdjjj.html

PHP:  $a && $b || !$c
来源：http://hz.dashuyun.cn/gtwihxxcxw.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gtuhxgwzvw.html

TS:   a && b || !c
来源：http://hz.smart0.xyz/gtlmhmmjzi.html

Java: a && b || !c
来源：http://hz.yvedp.cn/gtegnvflcr.html

Go:   a && b || !c
来源：http://hz.jiagoushi.top/gteozoysly.html

Ruby: a && b || !c
来源：http://hz.9152youxi.cn/gthwaiyaqq.html

C#:   a && b || !c
来源：http://hz.gotoacloud.top/gtlwpcwdlx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtblintgip.html

Py:   if not data: return
来源：http://hz.yj20258888.top/gtpopxdsmu.html

PHP:  if (!$data) { return; }
来源：http://hz.kuanghao11.cn/gtrpwwvilf.html

JS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtsxkttvvb.html

TS:   if (!data) return;
来源：http://hz.daxiang520.top/gthdhckmqo.html

Java: if (data == null) return;
来源：http://hz.hongshengwenyu.top/gtczhnzpvl.html

Go:   if data == nil { return }
来源：http://hz.wangshuangyany.cn/gtrptynjkn.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangtech.top/gtypjlcylc.html

C#:   if (data == null) return;
来源：http://hz.zhongyouzk.top/gtoyhzzuzk.html

================================================================================
来源：http://hz.yj20258.top/gtxkuopjii.html

C. 函数与作用域
来源：http://hz.xinyue.icu/gtmkitasem.html

================================================================================
来源：http://hz.chenzaomai.com/gthooidtif.html

[C01] 定义函数
来源：http://hz.0kj1m.cn/gtprgboacj.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtxhasxtnn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtpheonfbo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.aizwys.cn/gtitdleccb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtbgimxqxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtwehpltwo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.meibo888.top/gtubaudrzi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.birdmap.top/gttjdzfpjy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtmzograku.html

[C02] 默认参数
来源：http://hz.gaohongyu789.top/gtmjjroyuk.html

Py:   def greet(name="World"): return name
来源：http://hz.haohaochexian.top/gtkuursuiy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yangfankeji.com/gtakijsstq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtqaagsqap.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhixingplan.top/gtrgkbmclz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ybcxt.top/gtvbcssfxc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zdqjudy.top/gtlsuyghzo.html

Ruby: def greet(name = "World") = name
来源：http://hz.yongpay.top/gtqokamkpl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xuetiantiany.cn/gteuagnnyi.html

[C03] 可变参数
来源：http://hz.chenzaomai.com/gtjsuhczpe.html

Py:   def total(*args): return sum(args)
来源：http://hz.aizwys.cn/gtytrujubo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.birdmap.top/gtyusuamog.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gttptjacvu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtogcffiur.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtodylikgh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shangyingyoupin.top/gtwwwwntls.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtzlnzfywm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ivvv.top/gtyvedrhix.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnxiangtu.top/gtifjuqyqy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtnvzyorjo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xingfuxueyuan.xyz/gtxfhjzjwa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtkvphwrxk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nwbrower.top/gthlfbvbnm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pycfn.com/gtkolddmla.html

Go:   // 无：用配置结构体参数
来源：http://hz.iojbl.cn/gtothjorcs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtiognynzx.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtfuhvmuzx.html

[C05] 返回多个值
来源：http://hz.nwbrower.top/gtoazakcsu.html

Py:   return a, b
来源：http://hz.fengsongda.top/gtptdccmbz.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtspxzneuk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtaeoxrzhv.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtspujfklg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yanxiufei.cn/gtaghtmmig.html

Go:   return a, b
来源：http://hz.haohaochexian.top/gtqcwnxmsu.html

Ruby: return a, b
来源：http://hz.gzhubu.top/gtndcrmdnb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuetiantiany.cn/gthalnbpve.html

[C06] 匿名函数 / lambda
来源：http://hz.xziqi.cn/gtswfwpwfc.html

Py:   square = lambda x: x * x
来源：http://hz.yj202588.top/gtwzazvoap.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gtrntupljg.html

JS:   const square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtcphoqxmq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cucudq.cn/gttahpdewy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhaomingkeji.xyz/gtnpzxdycw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zycfv.cn/gtpcoaekei.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuanzx.com/gttpjyxicp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtlzpgjvdz.html

[C07] 把函数作为参数传入
来源：http://hz.yonumen.top/gtlavhqgut.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhoulong.xyz/gtmztcihaz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tanke756.top/gtqwcrwxmv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jianghu66.top/gtryihevle.html

TS:   arr.map(String)
来源：http://hz.mhx1999.top/gtbvwvzths.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgfzy.top/gtkghqxdml.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sysykeji.top/gtgivkwncd.html

Ruby: arr.map(&:upcase)
来源：http://hz.yongpay.top/gtfkspjrza.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.svipenyu.cn/gtvtbvuzrk.html

[C08] 闭包
来源：http://hz.zhaomingkeji.xyz/gtgpgqrrbd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jqgfzy.top/gtbskomvrz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yueranfly.top/gtnoqgnxok.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtlbtkhbns.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gttnnqqtzu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gzhubu.top/gtggrlqkpt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj202588.top/gtewhpicqi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtkebhfrgc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtyjxxipvw.html

[C09] 递归
来源：http://hz.vqdsnc.cn/gtieghibwd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgufenzy.top/gtyndgijoy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtmbfyhdiy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtxpgoegyq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtiylfpdyi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dianchejie.cn/gtmkcwmjer.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.vqdsnc.cn/gtqrvlehvm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gtdwwgqdrp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gthaeuqcvd.html

[C10] 变量作用域
来源：http://hz.sxryk.cn/gtwegpwanf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jyoumei.cn/gtqunxmcfq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.guannengcc.top/gtxkyoyhrb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenlongwang.top/gtzvrqukmh.html

TS:   同 JS
来源：http://hz.nanxuanxn.top/gtwezzgqhj.html

Java: 方法内为块级作用域
来源：http://hz.xuanzx.com/gtzmrlcvwi.html

Go:   花括号块级作用域
来源：http://hz.yangfankeji.com/gtjxqhqudm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuetiantiany.cn/gtqrehqzpf.html

C#:   块级作用域
来源：http://hz.zhengqikj.top/gtbummwoah.html

[C11] 模块导入与导出
来源：http://hz.hysaishi.cn/gtcpvtcmgz.html

Py:   from module import func
来源：http://hz.c1oappe.top/gtilbfkaht.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tian-w.cn/gtcyouekaj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.nanxuanxn.top/gtdphmzsyy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guowangkeji.top/gtdwofkeii.html

Java: import java.util.List;
来源：http://hz.sweek.top/gthdbnavih.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yvedp.cn/gtqwnnszwm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.redwolf501.top/gtewehqdie.html

C#:   using System.Text;
来源：http://hz.zycfv.cn/gtiainpmuh.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gtipfivkvc.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtpdsesyez.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gtciimhxxf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.9152youxi.cn/gtfhlkuahq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xingfuxueyuan.xyz/gtfakazuqv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydzc1.top/gtczclpbpb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ywan-chungtsiang.top/gtffgfqdoo.html

Ruby: -> { puts "run" }.call
来源：http://hz.quarkkingdee.top/gtbnczrqvt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtiwnxsgck.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtgwkmprio.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhijiandao.cn/gtvylyqoay.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtexfpaibp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtnlyyvbip.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtmyqiubyy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtvushgyev.html

Go:   func add(a, b int) int
来源：http://hz.xziqi.cn/gtymfsbzto.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tianlin.xyz/gtepxlkxjh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gtstinglgd.html

[C14] 泛型函数
来源：http://hz.zhijiandao.cn/gtrhoqjfrs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigfzy.top/gtutfdwpip.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtibxihkjp.html

JS:   // 无泛型
来源：http://hz.0kj1m.cn/gtofjoclfw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtgenaqrbj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtgeroeccl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtewakpmhf.html

Ruby: # 无泛型
来源：http://hz.yuanzhike.top/gtnfyhsmkg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.feifeiyinyue.top/gtbogdfuln.html

[C15] 解构 / 展开参数
来源：http://hz.nanxuanxn.top/gtsgiklzti.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gzhubu.top/gtjobnsiln.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gzhubu.top/gtuphtjujm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hammf.cn/gthwslukzl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinghuilouyu.cn/gtcvciprhm.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtdgxckbzw.html

Go:   // 无解构
来源：http://hz.hnqzz.top/gtpswzijfw.html

Ruby: a, b = pair
来源：http://hz.zycfv.cn/gtemgjxtvl.html

C#:   var (a, b) = pair;
来源：http://hz.kuanghao11.cn/gtugquudoj.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtrfvgyjfk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtjadytwup.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtfjkqsarv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jianghu66.top/gtfnmtxxdb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yvedp.cn/gtxygohtjq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuetiantiany.cn/gtknmsiaxz.html

Go:   // 无重载：用不同函数名
来源：http://hz.birdmap.top/gtrqjluxwm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinyuanbaomall.cn/gtwotcifav.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shzxlz.cn/gtmngnddkl.html

================================================================================
来源：http://hz.ivvv.top/gtwluglzlc.html

D. 数组 / 列表 / 集合
来源：http://hz.yanxiufei.cn/gtskepmbdd.html

================================================================================
来源：http://hz.hfpthk.cn/gtpmhecpvt.html

[D01] 创建数组 / 列表
来源：http://hz.haohaochexian.top/gtysnauhwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenzaomai.com/gtgldxchxa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtuovltjgw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guannengcc.top/gtmwjmfqtl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daria6918.cn/gtylewmjtr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hammf.cn/gtivgsrmmm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tian-w.cn/gtvscieoez.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yongpay.top/gtbrlmitad.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gtqhlhztrv.html

[D02] 追加元素到末尾
来源：http://hz.shzxlz.cn/gtkylfquty.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.vqdsnc.cn/gtxrzxxdxg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shanyushiyangtech.top/gtipztvhhs.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtpbnmwamv.html

TS:   arr.push(4);
来源：http://hz.sweek.top/gtrfzxfzhx.html

Java: list.add(4);
来源：http://hz.chenlongwang.top/gtbuxjdzfd.html

Go:   arr = append(arr, 4)
来源：http://hz.shangyingyoupin.top/gtshbhdwej.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jyoumei.cn/gtonxxeray.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gtunmtftri.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangkeji.top/gtdypndxye.html

Py:   arr.insert(0, 0)
来源：http://hz.svipenyu.cn/gtiihniztl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.0kj1m.cn/gtxxswnjrm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.mhx1999.top/gtnkjjghjo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinyuanbaomall.cn/gtjodhojkm.html

Java: list.add(0, 0);
来源：http://hz.cdnleiting.top/gtesorlorn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zycfv.cn/gtjbobeibq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yueranfly.top/gtofmxetgb.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtsbcllcex.html

[D04] 删除元素
来源：http://hz.vqdsnc.cn/gtibqkhnsx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtyuuogqwl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cheryme.top/gtussocvmf.html


<!-- 参考信息 -->