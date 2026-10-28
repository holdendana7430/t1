代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hammf.cn/gttajrzbuq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.iojbl.cn/gtlrghbrey.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj202588.top/gtduvtakon.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinqigfzy.top/gtdgwateij.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhengqikj.top/gtbfdwzaql.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shanyushiyangtech.top/gtytwonskq.html

[B07] while 循环
来源：http://hz.xylfe.cn/gtutcopmem.html

Py:   while i < 10: i += 1
来源：http://hz.guannengcc.top/gtamefhvcs.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jqgfzy.top/gtawdrsfnn.html

JS:   while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gtmfbvuvyc.html

TS:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtyavdhvvt.html

Java: while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtuddlhzbw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jyoumei.cn/gtjkzqzljh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xylfe.cn/gtaxgeukef.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtuwltkrhl.html

[B08] do-while（至少执行一次）
来源：http://hz.quarkkingdee.top/gtfllzluma.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gtpslbkneg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.dianchejie.cn/gtgpsjfopk.html

JS:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtvybpguqb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtbzlnlgmm.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtgdmmftzn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cheryme.top/gtioprpzmi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xziqi.cn/gtznusdfbi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtlnvrojxd.html

[B09] break 与 continue
来源：http://hz.daria6918.cn/gtehtqyzzz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.9152youxi.cn/gtmmcknfle.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtqxnyhxze.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtszokskxn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtirumirli.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtidqkumgo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yvedp.cn/gtbadprpif.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shuidangran.top/gthyqacspp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtusicxsct.html

[B10] 遍历同时拿索引
来源：http://hz.dashuyun.cn/gtnsbmvmrb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinghuilouyu.cn/gtxsvwyslf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fzhhl.top/gtmfrszyer.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgfzy.top/gtlyurpdlx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yongpay.top/gtacwqcfdi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.dashuyun.cn/gtqqsilhev.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cdnleiting.top/gtgdjawvoo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhoulong.xyz/gtpnhgnvod.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.pycfn.com/gtduysczjl.html

[B11] 生成数字序列 / 区间
来源：http://hz.guowangkeji.top/gtffbngvzx.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj202588.top/gtqxwatlkm.html

PHP:  range(0, 10, 2);
来源：http://hz.redwolf501.top/gtifzmxlmg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuxming.cn/gtyuobotbm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxinkj.top/gtskvqyoxm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zdqjudy.top/gthcwqwxvi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yuanzhike.top/gtodzbstff.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhijiandao.cn/gtkxrdpyvh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigufen.top/gtlravghld.html

[B12] 跳出多层循环
来源：http://hz.birdmap.top/gtvxhsioud.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cucudq.cn/gthxollqxu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.haohaochexian.top/gtbzhlnzjj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtwjlegwad.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtcromcupk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtzzbppaus.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zycfv.cn/gtyzjmfsxd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.pengpengdd.cyou/gtzolmairj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shuidangran.top/gthaffqmly.html

[B13] 判断是否为数字
来源：http://hz.dianchejie.cn/gtxtgbwcna.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtlhhlxjsy.html

PHP:  is_numeric($x)
来源：http://hz.yj202588.top/gtrpyqdqrd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhoulong.xyz/gtqrdoiuvf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tian-w.cn/gtlwoskbwl.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtncdejpmh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.aizwys.cn/gtxoefwvty.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xinyue.icu/gtmbhgshru.html

C#:   x is int or double or decimal
来源：http://hz.gaohongyu789.top/gtrrxpcbsz.html

[B14] 判断值是否在集合内
来源：http://hz.pycfn.com/gteyshtzfy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.9152youxi.cn/gtmapncofk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shzxlz.cn/gtphsjrlri.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtegmhzaqv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtjuffdajt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xinyue.icu/gtnddynqoa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zycfv.cn/gtufkxcmvu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhijiandao.cn/gtvsvbxdwj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dianchejie.cn/gthatccbic.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gthnwxlhfz.html

Py:   a and b or not c
来源：http://hz.cucudq.cn/gtyxpxhjuk.html

PHP:  $a && $b || !$c
来源：http://hz.xinyue.icu/gttghszxto.html

JS:   a && b || !c
来源：http://hz.ehwqpu.com/gtxoseyriy.html

TS:   a && b || !c
来源：http://hz.gaohongyu789.top/gtsqueaukd.html

Java: a && b || !c
来源：http://hz.pycfn.com/gtrpyoxdti.html

Go:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtgtvunaju.html

Ruby: a && b || !c
来源：http://hz.ydjk.org.cn/gteifnkbnn.html

C#:   a && b || !c
来源：http://hz.hnxiangtu.top/gtlkibcimh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigufen.top/gtcjtoopjw.html

Py:   if not data: return
来源：http://hz.xylfe.cn/gtgzgfaiuz.html

PHP:  if (!$data) { return; }
来源：http://hz.52xcode.cn/gtmevzassd.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtaccgtvmu.html

TS:   if (!data) return;
来源：http://hz.yonumen.top/gtklyaiumk.html

Java: if (data == null) return;
来源：http://hz.hammf.cn/gtulmcpwxl.html

Go:   if data == nil { return }
来源：http://hz.jianghu66.top/gtgwdugjnt.html

Ruby: return if data.nil?
来源：http://hz.sysykeji.top/gtbeqhazfm.html

C#:   if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gtnvltukdv.html

================================================================================
来源：http://hz.xuanzx.com/gtkdoqizby.html

C. 函数与作用域
来源：http://hz.tianlin.xyz/gtyttfalmc.html

================================================================================
来源：http://hz.aizwys.cn/gtuxsexzik.html

[C01] 定义函数
来源：http://hz.guannengcc.top/gtdijhhaea.html

Py:   def add(a, b): return a + b
来源：http://hz.birdmap.top/gthiggrirq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtfrxemkyg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtkfwoclbx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtcmqbahkw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ivvv.top/gtmyywcfyn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shangyingyoupin.top/gtvatzkmse.html

Ruby: def add(a, b); a + b; end
来源：http://hz.havefunace.top/gtazbgwyzw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtywesqpnt.html

[C02] 默认参数
来源：http://hz.hongshengwenyu.top/gtcnaxhsmq.html

Py:   def greet(name="World"): return name
来源：http://hz.fengsongda.top/gtkjuepzeg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigufen.top/gtuvlrwbhx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.sxryk.cn/gtaqwcsgks.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.guowangkeji.top/gtqlpmqguq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydzc1.top/gtqpwrntwc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhongyouzk.top/gtwpxufsii.html

Ruby: def greet(name = "World") = name
来源：http://hz.zdqjudy.top/gtwbhjqixm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.svipenyu.cn/gtmlpjnvfy.html

[C03] 可变参数
来源：http://hz.jinyuanbaomall.cn/gtiquwvdjk.html

Py:   def total(*args): return sum(args)
来源：http://hz.hongshengwenyu.top/gtwzpodiwa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.smart0.xyz/gtvtpolalm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtuoqwvnxv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtbccbiria.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinqigufen.top/gtxdzlkwcj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sufxvd.cn/gtzvftwgcq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenlongwang.top/gtnaqajqxf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gtnfacfkmj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhixingplan.top/gtviuzeipd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.52xcode.cn/gtpqpgnmwp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yanxiufei.cn/gtpuivmztp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtoxrunijb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.pycfn.com/gtxsvtwtps.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258.top/gtfdsoikgv.html

Go:   // 无：用配置结构体参数
来源：http://hz.jlsjyb.cn/gtujmhkxes.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtnhxxtsrq.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gteperkwkq.html

[C05] 返回多个值
来源：http://hz.hnqzz.top/gtbyjohzyn.html

Py:   return a, b
来源：http://hz.jqgufenzy.top/gtsgfluloc.html

PHP:  return [$a, $b];
来源：http://hz.cashguo.top/gtmfnhiita.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gaohongyu789.top/gtzmdlomqv.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gtpyzgtigv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yonumen.top/gtofpnoqxy.html

Go:   return a, b
来源：http://hz.pengpengdd.cyou/gtvabvfngd.html

Ruby: return a, b
来源：http://hz.quarkkingdee.top/gtohkvtqni.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj202588.top/gtvocmgkcv.html

[C06] 匿名函数 / lambda
来源：http://hz.shzxlz.cn/gtpalfmaou.html

Py:   square = lambda x: x * x
来源：http://hz.yongpay.top/gtbkuajvjs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jianghu66.top/gtssffhuvn.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtcxbhnnnb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtxommwkcz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pengpengdd.cyou/gtdaznvkjm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guowangkeji.top/gthpfqqvrg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtezqjkzla.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj202588.top/gtmcrapewk.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangkeji.top/gtammlmoyr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hongshengwenyu.top/gtvqzbakms.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haohaochexian.top/gtteytgqtv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sufxvd.cn/gtecctpjgk.html

TS:   arr.map(String)
来源：http://hz.feifeiyinyue.top/gtfjdyehcu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shuidangran.top/gtscvzseyh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yongpay.top/gthwltmkuf.html

Ruby: arr.map(&:upcase)
来源：http://hz.redwolf501.top/gtldwneaeh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gtmsdskcmo.html

[C08] 闭包
来源：http://hz.hnxiangtu.top/gtzixisaqi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daria6918.cn/gtsjnsyrdn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guowangkeji.top/gthfgtimzd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtjjytlony.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtqyzyazuk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtfuvyjpxv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.9152youxi.cn/gtgmtowxxm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhijiandao.cn/gtiztkvpmt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtsnunkxpp.html

[C09] 递归
来源：http://hz.zhoulong.xyz/gtftimincn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yueranfly.top/gtbdihwqaf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xylfe.cn/gtzkmgthjr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gtrfklctgk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigfzy.top/gtmcmzrjbd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xziqi.cn/gtnojsshif.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ywan-chungtsiang.top/gtxrrwcjct.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtgymroccj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yvedp.cn/gtzbawitfg.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gtbunvhsct.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtrmmdnwcc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yj20258.top/gtsajgticf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuetiantiany.cn/gtfliwgxaj.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtwfogbecr.html

Java: 方法内为块级作用域
来源：http://hz.xinyue.icu/gtaenbrpwp.html

Go:   花括号块级作用域
来源：http://hz.yj20258.top/gtyeucngrh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.smart0.xyz/gtoiynsizv.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtlygvihrx.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtowzgiiea.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gtokjijarf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtqyprjjze.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.316326.xyz/gthrhnqjkd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zdqjudy.top/gtqexhtfrr.html

Java: import java.util.List;
来源：http://hz.hammf.cn/gtwseyrztu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yanxiufei.cn/gtmgfywxiw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shuidangran.top/gtojvyqrcf.html

C#:   using System.Text;
来源：http://hz.daxiang520.top/gtxfndecqb.html

[C12] 立即执行函数 IIFE
来源：http://hz.aizwys.cn/gtdrhjawek.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gthseiflps.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtvztgswod.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtqlyhxsum.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtnqcavxgc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ehwqpu.com/gtdzowyqpt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.vqdsnc.cn/gtdnczxjqi.html

Ruby: -> { puts "run" }.call
来源：http://hz.daria6918.cn/gtlhgvupgc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gthgvmbpgl.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhiwuduotai.top/gtycczeygf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigufen.top/gtsqnhpuam.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtixyuazhg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tanke756.top/gtoyvtkhgo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gtubjdhlcg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gthcnnbtok.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtdfsaiipj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cheryme.top/gtrukuhcpo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cheryme.top/gtulhnghew.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtjgbdkbyi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shzxlz.cn/gtebmpprni.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtarqvzpzz.html

JS:   // 无泛型
来源：http://hz.chenlongwang.top/gttglkcxfl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.mhx1999.top/gtyqlblpdf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pengpengdd.cyou/gtlfvesfge.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.bjfxy.top/gtvihvrjnt.html

Ruby: # 无泛型
来源：http://hz.quarkkingdee.top/gttxfivygy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gttxjkhoqa.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtdfxpwwxw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.svipenyu.cn/gtycsuomaw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuetiantiany.cn/gtqovcvhyp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.haohaochexian.top/gtljmbqwpg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtbgyrzihq.html

Java: // 无解构
来源：http://hz.feifeiyinyue.top/gteigwqhzq.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtkycwtojb.html

Ruby: a, b = pair
来源：http://hz.hnxiangtu.top/gtyzetzixe.html

C#:   var (a, b) = pair;
来源：http://hz.zhaomingkeji.xyz/gtwenflvny.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gtutihdiyi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhiwuduotai.top/gtdtcjwjmk.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtzzejfakj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhiwuduotai.top/gtytprypmq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yongpay.top/gtveadmhla.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hysaishi.cn/gtwsgzburt.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtwdnnaxyz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gaohongyu789.top/gtvetcsqar.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ivvv.top/gtxabtzwts.html

================================================================================
来源：http://hz.hfpthk.cn/gtfpwxemvj.html

D. 数组 / 列表 / 集合
来源：http://hz.meibo888.top/gtpuowtoma.html

================================================================================
来源：http://hz.daxiang520.top/gtbqrfobhu.html

[D01] 创建数组 / 列表
来源：http://hz.zdqjudy.top/gtxblkyngl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangdashe.top/gtsqeathea.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.redwolf501.top/gtkahmfuxm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pengpengdd.cyou/gtuzturywc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.c1oappe.top/gtrjegcopp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.birdmap.top/gtbhrmyhgu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gzhubu.top/gtabndtqxu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yvedp.cn/gtewgzhfsu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shangyingyoupin.top/gtotgfidog.html

[D02] 追加元素到末尾
来源：http://hz.yueranfly.top/gtoyrieynp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aizwys.cn/gtusuddlvr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zycfv.cn/gtpwujxpob.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gthdjouzfe.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtsgbesqar.html

Java: list.add(4);
来源：http://hz.zhoulong.xyz/gtadwqdhji.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gteqcrvggp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.redwolf501.top/gtivkfcrwj.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gteqarycer.html

[D03] 在指定位置插入元素
来源：http://hz.yueranfly.top/gtqmqbtqxe.html

Py:   arr.insert(0, 0)
来源：http://hz.nanxuanxn.top/gtfcarivru.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.9152youxi.cn/gtkpyhwbyg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aibaodan.cn/gtvsvptots.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sysykeji.top/gtvtxuijfk.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtjeqcljdv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yanxiufei.cn/gtknmuddoh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.andypj.xyz/gtdsnkdpxn.html

C#:   list.Insert(0, 0);
来源：http://hz.jinghuilouyu.cn/gttycfauwn.html

[D04] 删除元素
来源：http://hz.tian-w.cn/gtpzlcljkn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shzxlz.cn/gtsncpgehq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtthwolbte.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.vqdsnc.cn/gtgqpckrtk.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtkbogzowk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hammf.cn/gtxlywehww.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fzhhl.top/gtxottvtfq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtkqhkxkfo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gtfanurtpk.html

[D05] 访问与修改元素
来源：http://hz.cucudq.cn/gtdjtqrqou.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtdhmhtbvr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.redwolf501.top/gttctmshii.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gttqpnfvrf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtyesrjupz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhoulong.xyz/gtkmhkhcvo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtbkvabsag.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtfdxmodqt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.0kj1m.cn/gtlkdupgiv.html

[D06] 数组长度
来源：http://hz.cucudq.cn/gtnstynguy.html

Py:   len(arr)
来源：http://hz.yuxming.cn/gtnnksbuzw.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtqnopyefr.html

JS:   arr.length
来源：http://hz.yj20258.top/gtiffbnopr.html

TS:   arr.length
来源：http://hz.chenjidiqi.icu/gtsyzvayjb.html

Java: list.size();
来源：http://hz.dashuyun.cn/gtntlmykin.html

Go:   len(arr)
来源：http://hz.9152youxi.cn/gtsawyzakp.html

Ruby: arr.length; arr.size
来源：http://hz.gogol.net.cn/gtntucskre.html

C#:   list.Count;
来源：http://hz.smart0.xyz/gtagfnltns.html


<!-- 参考信息 -->