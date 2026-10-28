代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinyuanbaomall.cn/gteuwvtjka.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jianghu66.top/gtnxnqsnjc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yvedp.cn/gthdiwccbz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.smart0.xyz/gtgihbkcbi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.guowangkeji.top/gteqmueqty.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jianghu66.top/gtqpukeqjk.html

[B07] while 循环
来源：http://hz.dashuyun.cn/gtumffgfae.html

Py:   while i < 10: i += 1
来源：http://hz.wangdashe.top/gtsksjpfsi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhoulong.xyz/gtvvvbrcgo.html

JS:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtqyrqbaxt.html

TS:   while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtsqopvfoe.html

Java: while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtrqvyhgzd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jyoumei.cn/gtmzifzvqi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ybcxt.top/gtnqcrtoil.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtgjzxxrdk.html

[B08] do-while（至少执行一次）
来源：http://hz.hongshengwenyu.top/gthnfbkgtc.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yanxiufei.cn/gtfdebxidb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hammf.cn/gtpxoqsszf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtmzobhlvq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gteawoyyxh.html

Java: do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtqbyrmkek.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.feifeiyinyue.top/gtigglurhg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tian-w.cn/gteesdwvgc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtdlmczdxc.html

[B09] break 与 continue
来源：http://hz.andypj.xyz/gtjyzgskkq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hysaishi.cn/gtjlnotfbo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.snrcjt.cn/gthbjsgiay.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtbkugqjdf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgufenzy.top/gtshfhteaq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gttuxjksyv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenzaomai.com/gtkkwsqcpn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jyoumei.cn/gtcasjtdtt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gtrpacradw.html

[B10] 遍历同时拿索引
来源：http://hz.gzhubu.top/gtkyttyaqt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinghuilouyu.cn/gtmdxelpaq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yvedp.cn/gtdegvxlob.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dianchejie.cn/gthkkacmgj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.bjfxy.top/gtvdsynljv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yuxming.cn/gtpnrnbkgc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.redwolf501.top/gtxqivsjlr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sufxvd.cn/gtzlnewpma.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangshuangyany.cn/gtltdeteal.html

[B11] 生成数字序列 / 区间
来源：http://hz.shanyushiyangkeji.top/gtcshoutxf.html

Py:   list(range(0, 10, 2))
来源：http://hz.haohaochexian.top/gtixhhyfvc.html

PHP:  range(0, 10, 2);
来源：http://hz.zhoulong.xyz/gtpcumgikb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhixingplan.top/gtkqmiglnx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yonumen.top/gtepizkztd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jlsjyb.cn/gtyaxfuctz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yanxiufei.cn/gtelswcclc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.andypj.xyz/gtvtbubjvm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xziqi.cn/gtvpuinqov.html

[B12] 跳出多层循环
来源：http://hz.chenjidiqi.icu/gtphpfpouo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shzxlz.cn/gtdtbtklxl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.daxiang520.top/gtgprfdzak.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtfdzthafb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtjdzmssai.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tianlin.xyz/gtsxmbvsqo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tianlin.xyz/gtixrqjdei.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.bjfxy.top/gtmrubozav.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.havefunace.top/gtabxgvnpc.html

[B13] 判断是否为数字
来源：http://hz.zhijiandao.cn/gtrefbkhjt.html

Py:   isinstance(x, (int, float))
来源：http://hz.hammf.cn/gtkcgqugnx.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtgggzpysz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fengsongda.top/gtdptwtbjg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtgfmaenjs.html

Java: x instanceof Number
来源：http://hz.andypj.xyz/gtyyevvwof.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuetiantiany.cn/gtuveohrdq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.smart0.xyz/gttjvrjcve.html

C#:   x is int or double or decimal
来源：http://hz.yueranfly.top/gtsppeegax.html

[B14] 判断值是否在集合内
来源：http://hz.sysykeji.top/gtmqibjyvj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yj202588.top/gtgbglpkmr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sweek.top/gtxlojocnm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtddveedvz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hnxiangtu.top/gttvfyiccz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cheryme.top/gtkgsxgsyh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tianlin.xyz/gthcmaarwv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtfofkhtkp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zdqjudy.top/gtwvtieuvs.html

[B15] 布尔运算与取反
来源：http://hz.aizwys.cn/gtrzmukmvd.html

Py:   a and b or not c
来源：http://hz.feifeiyinyue.top/gtgvcwybij.html

PHP:  $a && $b || !$c
来源：http://hz.aibaodan.cn/gtmknvqkhr.html

JS:   a && b || !c
来源：http://hz.cucudq.cn/gtjvoezxca.html

TS:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtzkhqnqot.html

Java: a && b || !c
来源：http://hz.yongpay.top/gtpnhpzibv.html

Go:   a && b || !c
来源：http://hz.snrcjt.cn/gthljlvmbf.html

Ruby: a && b || !c
来源：http://hz.yonumen.top/gtabkdgycm.html

C#:   a && b || !c
来源：http://hz.ehwqpu.com/gtbxgcwfgp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.aizwys.cn/gtghwjftty.html

Py:   if not data: return
来源：http://hz.nanxuanxn.top/gtjsnrzgyb.html

PHP:  if (!$data) { return; }
来源：http://hz.hysaishi.cn/gtnviamrqp.html

JS:   if (!data) return;
来源：http://hz.tanke756.top/gtdihoapek.html

TS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtcbansgfa.html

Java: if (data == null) return;
来源：http://hz.pengpengdd.cyou/gtqirbfwww.html

Go:   if data == nil { return }
来源：http://hz.yonumen.top/gtezxwjgeu.html

Ruby: return if data.nil?
来源：http://hz.xuetiantiany.cn/gtirolnpzb.html

C#:   if (data == null) return;
来源：http://hz.mhx1999.top/gtyubzwymw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlzcjadrt.html

C. 函数与作用域
来源：http://hz.andypj.xyz/gtpjgupaju.html

================================================================================
来源：http://hz.jqgfzy.top/gtwluyyzpx.html

[C01] 定义函数
来源：http://hz.sysykeji.top/gttnrhgynk.html

Py:   def add(a, b): return a + b
来源：http://hz.yj202588.top/gtibuqgsib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtckcrxqnc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ivvv.top/gtsmuhntbd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtnvtlhujp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jqgfzy.top/gtnwxukrvf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhijiandao.cn/gtdvxacdvg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258.top/gtnvwdrhhb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtajuesffb.html

[C02] 默认参数
来源：http://hz.cqqwz.cn/gtaakdigtr.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtfykdbttk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daxiang520.top/gtnluabfyl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cheryme.top/gtsddrteqo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gtsmgrnuzy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenzaomai.com/gturclegxj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guannengcc.top/gtjwbjvfpc.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigfzy.top/gtdtmxtmzq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aizwys.cn/gtydakohja.html

[C03] 可变参数
来源：http://hz.vqdsnc.cn/gtpsafvbyy.html

Py:   def total(*args): return sum(args)
来源：http://hz.kuanghao11.cn/gtonihwlbo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.9152youxi.cn/gteryytncz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtptojdgpp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtqpsufqlm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ivvv.top/gtsffyfoxz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.birdmap.top/gtivupohmg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ehwqpu.com/gteojjexme.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tianlin.xyz/gtyomzxpjv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ywan-chungtsiang.top/gtaylwpqdt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.andypj.xyz/gtksdpfjht.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuanzhike.top/gtuapyzyph.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtdvoicrtg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sweek.top/gtmgoepovg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnqzz.top/gtucitkycp.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhoulong.xyz/gtxydtdcix.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtfyvjfyeu.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtblaclvoe.html

[C05] 返回多个值
来源：http://hz.xuanzx.com/gtqidqdzlk.html

Py:   return a, b
来源：http://hz.fzhhl.top/gtyszsqcln.html

PHP:  return [$a, $b];
来源：http://hz.yanxiufei.cn/gtkfpqppet.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gtkerlycmb.html

TS:   return { a, b };
来源：http://hz.wangshuangyany.cn/gtxfswkpjx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.quarkkingdee.top/gtnuxnxndu.html

Go:   return a, b
来源：http://hz.shangyingyoupin.top/gtyqvieynz.html

Ruby: return a, b
来源：http://hz.pengpengdd.cyou/gtecxipoky.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.meibo888.top/gtuozfdxpd.html

[C06] 匿名函数 / lambda
来源：http://hz.hongshengwenyu.top/gthxnjrxqf.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gtsfkbymch.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gaohongyu789.top/gtxcsbvvhj.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtwdufafte.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hywenlv.cn/gtueaqltpl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cqqwz.cn/gtlgfpbszz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shuidangran.top/gteuamprvi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nwbrower.top/gtnnspgjdk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cucudq.cn/gtdiqpcnve.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtrbqsntdf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.guowangkeji.top/gtrquchodx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenzaomai.com/gttccyxuwb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinghuilouyu.cn/gthevqznyh.html

TS:   arr.map(String)
来源：http://hz.zhixingplan.top/gtzazknplp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.0kj1m.cn/gtmwszlwsh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jyoumei.cn/gtfxmcqebj.html

Ruby: arr.map(&:upcase)
来源：http://hz.sufxvd.cn/gtcnlhewtr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.pycfn.com/gtxcdxwsmz.html

[C08] 闭包
来源：http://hz.9152youxi.cn/gtdihcptqe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sxryk.cn/gtmnnwokci.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.andypj.xyz/gtqwgfvkis.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtapfnokvb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gthybhbmkn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jyoumei.cn/gtplqpvmsk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pycfn.com/gtsecjgdvg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.0kj1m.cn/gtwlemjgwu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtjzoshnsw.html

[C09] 递归
来源：http://hz.hammf.cn/gtshvstybz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtdhdylopd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.smart0.xyz/gtuydwqtrg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtbdjbhvyy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtxhrnuxap.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigfzy.top/gtoljfaryt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aibaodan.cn/gtxiuqjwoz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtupsangtz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gtprksmwvv.html

[C10] 变量作用域
来源：http://hz.xziqi.cn/gtswlxjabl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gaohongyu789.top/gtpftolkmm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtzwzdzjfu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gtisktloen.html

TS:   同 JS
来源：http://hz.aizwys.cn/gtoxxmsjms.html

Java: 方法内为块级作用域
来源：http://hz.quarkkingdee.top/gtqmksqruw.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtghlruwap.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.havefunace.top/gtukhhxlbd.html

C#:   块级作用域
来源：http://hz.wangdashe.top/gtouqpmhdx.html

[C11] 模块导入与导出
来源：http://hz.cheryme.top/gtxsnlfqor.html

Py:   from module import func
来源：http://hz.52xcode.cn/gtqqbiwrae.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtritjturc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fzhhl.top/gtiwmcaeon.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xingfuxueyuan.xyz/gtpybkumhi.html

Java: import java.util.List;
来源：http://hz.sysykeji.top/gtbxwghfvm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.redwolf501.top/gtzzugqweo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuanzx.com/gtrtvakdbd.html

C#:   using System.Text;
来源：http://hz.jinqigfzy.top/gtkpslzvrg.html

[C12] 立即执行函数 IIFE
来源：http://hz.c1oappe.top/gtambvntgx.html

Py:   (lambda: print("run"))()
来源：http://hz.tianlin.xyz/gtbhyynqvx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigufen.top/gtudcrxbri.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gttmduvbsc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtacbystsp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yuxming.cn/gtgcpzxanm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtmmrluvri.html

Ruby: -> { puts "run" }.call
来源：http://hz.sweek.top/gtwoijxifi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtbalmvcpv.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gtgfcnsgor.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtipvreigg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtafydxybq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guannengcc.top/gtcfrbusgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gtyajwllhh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtfukbblas.html

Go:   func add(a, b int) int
来源：http://hz.kuanghao11.cn/gtyjyemgqq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yonumen.top/gtnjnfgdac.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258.top/gtuhfjigkq.html

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtkcezejiw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtbxlzhhff.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtzjwhcycq.html

JS:   // 无泛型
来源：http://hz.jinqigufen.top/gtubwixpur.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenzaomai.com/gtviodboto.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xziqi.cn/gtemvoveyu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xylfe.cn/gtighfieur.html

Ruby: # 无泛型
来源：http://hz.hammf.cn/gtkpmjucil.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shuidangran.top/gtxfyftjow.html

[C15] 解构 / 展开参数
来源：http://hz.nanxuanxn.top/gtsmjdlalm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinghuilouyu.cn/gtojyevsoz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtzxiufyjt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtppodygek.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yvedp.cn/gtevchsfog.html

Java: // 无解构
来源：http://hz.nwbrower.top/gtueimaigo.html

Go:   // 无解构
来源：http://hz.hywenlv.cn/gtjnkotjso.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gttykgkino.html

C#:   var (a, b) = pair;
来源：http://hz.tian-w.cn/gttqqeijif.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtudsoiiry.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenzaomai.com/gtvadgxzqi.html

PHP:  // 无重载
来源：http://hz.c1oappe.top/gtimqkttib.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtqovvrgar.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigfzy.top/gtvrbgisfh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhijiandao.cn/gtvnxttldw.html

Go:   // 无重载：用不同函数名
来源：http://hz.fengsongda.top/gtxlahpqcd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangdashe.top/gtuqylgcda.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.redwolf501.top/gtunghfmvn.html

================================================================================
来源：http://hz.pycfn.com/gtjpyekpnx.html

D. 数组 / 列表 / 集合
来源：http://hz.feifeiyinyue.top/gthcuvezwd.html

================================================================================
来源：http://hz.xziqi.cn/gtcurgeave.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtzuyfgiot.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtgidjpwto.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fzhhl.top/gtrcbkvyal.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gaohongyu789.top/gtyclotpjd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ybcxt.top/gtnkcvhoos.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daxiang520.top/gtqvrnupmg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtbzfhgrit.html

Ruby: arr = [1, 2, 3]
来源：http://hz.kuanghao11.cn/gtnsevlosr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sufxvd.cn/gtxedjuylq.html

[D02] 追加元素到末尾
来源：http://hz.316326.xyz/gtfqwbxynn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cucudq.cn/gtjrlxnlfj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtmywpqbpw.html

JS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtgqcstemo.html

TS:   arr.push(4);
来源：http://hz.gzhubu.top/gtcoxfedzp.html

Java: list.add(4);
来源：http://hz.jyoumei.cn/gtrmoxmpwq.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtcjbdmnqs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gtjmnnrtic.html

C#:   list.Add(4);
来源：http://hz.pengpengdd.cyou/gtvjginook.html

[D03] 在指定位置插入元素
来源：http://hz.zhiwuduotai.top/gtiiswqodi.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtdmplzkqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.svipenyu.cn/gtttizmgae.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhengqikj.top/gtymezpyeb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yongpay.top/gtmecwxghv.html

Java: list.add(0, 0);
来源：http://hz.ivvv.top/gtervghxzt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gtjnltveff.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gotoacloud.top/gtsqrsxojn.html

C#:   list.Insert(0, 0);
来源：http://hz.jinghuilouyu.cn/gtnxnrlate.html

[D04] 删除元素
来源：http://hz.iojbl.cn/gtotbihmpl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.snrcjt.cn/gtpxlacyzz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jyoumei.cn/gtdjtkuftz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zdqjudy.top/gtpotoxvgd.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gtktyjuise.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jqgufenzy.top/gtgylzyxju.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.52xcode.cn/gtwjqipasb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hnqzz.top/gtcmelbwrl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ppjwa.cn/gteupswrtf.html

[D05] 访问与修改元素
来源：http://hz.guannengcc.top/gtuaswjvnh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtjfoixapi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtfzzehwxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.havefunace.top/gtnxgiesid.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yonumen.top/gtrnqhqmfr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gtebbpmikz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtjuuojjll.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtrtidfvvs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtohnqduob.html

[D06] 数组长度
来源：http://hz.zhongyouzk.top/gtzhptyurq.html

Py:   len(arr)
来源：http://hz.shzxlz.cn/gthbpojzqq.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtysawtdhm.html

JS:   arr.length
来源：http://hz.ydjk.org.cn/gtskxslwil.html

TS:   arr.length
来源：http://hz.hammf.cn/gtffzxllix.html

Java: list.size();
来源：http://hz.yongpay.top/gtvonrapff.html

Go:   len(arr)
来源：http://hz.yangfankeji.com/gtahkfqqmu.html

Ruby: arr.length; arr.size
来源：http://hz.gaohongyu789.top/gtcwgglioa.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtdeaalixh.html


<!-- 参考信息 -->