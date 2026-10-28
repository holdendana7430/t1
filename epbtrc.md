代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangkeji.top/gtryliehlu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sweek.top/gtivfzqaak.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cucudq.cn/gtxczqsnkt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ivvv.top/gtxmkwduqu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.guowangkeji.top/gtfmxqljgd.html

[B06] 遍历字典 / 对象
来源：http://hz.fzhhl.top/gttypfrtfd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ppjwa.cn/gttegqbhcw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.pengpengdd.cyou/gtmgzsoujg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yueranfly.top/gthnwauvbl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhixingplan.top/gthsexkeef.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xinyue.icu/gtdywodzhf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.kuanghao11.cn/gtkghigjrh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xinyue.icu/gtizplewcm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.snrcjt.cn/gtrcpernly.html

[B07] while 循环
来源：http://hz.dianchejie.cn/gtrhrswhor.html

Py:   while i < 10: i += 1
来源：http://hz.cashguo.top/gtqpmvzipw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.52xcode.cn/gtkkjggxpq.html

JS:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtuaxmpayl.html

TS:   while (i < 10) { i++; }
来源：http://hz.dashuyun.cn/gtncyxakvj.html

Java: while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtbxckbglr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hammf.cn/gtfegcymcc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenlongwang.top/gtwyneezdo.html

C#:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtordcvxyv.html

[B08] do-while（至少执行一次）
来源：http://hz.xuanzx.com/gtziafwyck.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.bjfxy.top/gtnseowoha.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.tianlin.xyz/gtvugltrcy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtdjbrhaci.html

TS:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtlnrbzpml.html

Java: do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtkxaqhvbj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.fengsongda.top/gtauqrwpaf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gotoacloud.top/gtnokxjyip.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtfemeijfv.html

[B09] break 与 continue
来源：http://hz.xuetiantiany.cn/gtxptcshqm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yj20258888.top/gtaubbybxx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.aizwys.cn/gtxcbkapjz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtdntzixfg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtmtynigqh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtaxvoqmrc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xinyue.icu/gtsdjjhnxq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tanke756.top/gtqeuwmkzg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtqpxrjalh.html

[B10] 遍历同时拿索引
来源：http://hz.ivvv.top/gttpwqtfui.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dianchejie.cn/gtdebphmji.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ybcxt.top/gtzzdntwxz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xuetiantiany.cn/gtbrpbuxjg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.haohaochexian.top/gtsbbgsihs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sufxvd.cn/gtdsdattkv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.tianlin.xyz/gtrvyefuie.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cucudq.cn/gtgirjoxsb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cheryme.top/gtxaqwiwur.html

[B11] 生成数字序列 / 区间
来源：http://hz.nanxuanxn.top/gtncizipjr.html

Py:   list(range(0, 10, 2))
来源：http://hz.c1oappe.top/gtqgvmobts.html

PHP:  range(0, 10, 2);
来源：http://hz.xuanzx.com/gtferkotie.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtqqkkmjze.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gtfniaouku.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.9152youxi.cn/gttjrwywku.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yongpay.top/gtopxgenhj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cashguo.top/gtkhjgqbol.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.0kj1m.cn/gtindtpbfd.html

[B12] 跳出多层循环
来源：http://hz.gzhubu.top/gtlczccqog.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sysykeji.top/gtpwmeiipo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtotpdbjmh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtowpoxnmr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtfthrknvq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gtchyvmbbs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cucudq.cn/gtlejfvqyz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.kuanghao11.cn/gtyumjbojl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jiagoushi.top/gtevarlors.html

[B13] 判断是否为数字
来源：http://hz.hnqzz.top/gtknyibppk.html

Py:   isinstance(x, (int, float))
来源：http://hz.feifeiyinyue.top/gtaofqobzq.html

PHP:  is_numeric($x)
来源：http://hz.hnqzz.top/gtdxwohkpo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhijiandao.cn/gtlgmqjauy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtnuhghhmd.html

Java: x instanceof Number
来源：http://hz.jinyuanbaomall.cn/gtqgbnfefb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hammf.cn/gtfdhugcom.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ywan-chungtsiang.top/gtkvaavpny.html

C#:   x is int or double or decimal
来源：http://hz.jinghuilouyu.cn/gtrnsahnkp.html

[B14] 判断值是否在集合内
来源：http://hz.xziqi.cn/gtmoayqveb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gaohongyu789.top/gtzekzdjoa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenlongwang.top/gtniipzbss.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ppjwa.cn/gttthijprr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gttmustojb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.fengsongda.top/gtswxsdbjt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hywenlv.cn/gtzemonjef.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pycfn.com/gtysotrfcr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yonumen.top/gtlsnxywdo.html

[B15] 布尔运算与取反
来源：http://hz.shzxlz.cn/gtjnolrlgz.html

Py:   a and b or not c
来源：http://hz.yanxiufei.cn/gtrhvggsaj.html

PHP:  $a && $b || !$c
来源：http://hz.xinyue.icu/gtmbeiawvi.html

JS:   a && b || !c
来源：http://hz.cqqwz.cn/gtxhdliplo.html

TS:   a && b || !c
来源：http://hz.jianghu66.top/gtogvpjqss.html

Java: a && b || !c
来源：http://hz.aibaodan.cn/gtyazabfjx.html

Go:   a && b || !c
来源：http://hz.sweek.top/gtfxtsleds.html

Ruby: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtcjkdwhnc.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gtiytejigw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.52xcode.cn/gtebormtfi.html

Py:   if not data: return
来源：http://hz.shanyushiyangtech.top/gtdjcjmope.html

PHP:  if (!$data) { return; }
来源：http://hz.yonumen.top/gtcgdjsxhg.html

JS:   if (!data) return;
来源：http://hz.nwbrower.top/gtfvakfeyf.html

TS:   if (!data) return;
来源：http://hz.wangdashe.top/gtqtpkrcuv.html

Java: if (data == null) return;
来源：http://hz.jinqigufen.top/gthojdirmi.html

Go:   if data == nil { return }
来源：http://hz.tianlin.xyz/gtifeoozkp.html

Ruby: return if data.nil?
来源：http://hz.fzhhl.top/gtwpjvmplx.html

C#:   if (data == null) return;
来源：http://hz.hnqzz.top/gtwdcuvabu.html

================================================================================
来源：http://hz.meibo888.top/gtmfoxxuyd.html

C. 函数与作用域
来源：http://hz.zhongyouzk.top/gtckztkfyz.html

================================================================================
来源：http://hz.52xcode.cn/gtogryqcmy.html

[C01] 定义函数
来源：http://hz.chenlongwang.top/gtnulyzcvp.html

Py:   def add(a, b): return a + b
来源：http://hz.shuidangran.top/gtwxlkcvvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtyurltcat.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtwotvqujd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtcrfuymkt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtdkbrqjtn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hywenlv.cn/gtwcazcloe.html

Ruby: def add(a, b); a + b; end
来源：http://hz.bjfxy.top/gtlcioario.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gthjystzeb.html

[C02] 默认参数
来源：http://hz.cashguo.top/gthuwgdizv.html

Py:   def greet(name="World"): return name
来源：http://hz.wangdashe.top/gthcelxjsm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zdqjudy.top/gtxalvoiyg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangkeji.top/gtdwombjrd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.birdmap.top/gtdanvvedb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.kuanghao11.cn/gtqdueyudc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ywan-chungtsiang.top/gthwavmevw.html

Ruby: def greet(name = "World") = name
来源：http://hz.52xcode.cn/gtctotdsec.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenlongwang.top/gtewkivszc.html

[C03] 可变参数
来源：http://hz.jyoumei.cn/gtiiwrwezy.html

Py:   def total(*args): return sum(args)
来源：http://hz.jlsjyb.cn/gttlpgsavt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtksmzaphf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jyoumei.cn/gtxdbthjnj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtowdxwcrd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jyoumei.cn/gtcypoggaa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gtiodtudcp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shanyushiyangkeji.top/gthmjwfvwx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtfakheuom.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnxiangtu.top/gtauslnoxi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.bjfxy.top/gtlqxqecqy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tian-w.cn/gtbowzhunz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtmkknrihm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuanzx.com/gtvddlnbhx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258888.top/gtyfyqyjjb.html

Go:   // 无：用配置结构体参数
来源：http://hz.gotoacloud.top/gtrtymmexx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtqemzfpxh.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gteikyvkkv.html

[C05] 返回多个值
来源：http://hz.jianghu66.top/gtajaznbir.html

Py:   return a, b
来源：http://hz.hfpthk.cn/gtjxpjvfdx.html

PHP:  return [$a, $b];
来源：http://hz.iojbl.cn/gtgpmxodzb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnxiangtu.top/gtknvucmvd.html

TS:   return { a, b };
来源：http://hz.hfpthk.cn/gtfefoyxft.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtfelzoejc.html

Go:   return a, b
来源：http://hz.chenlongwang.top/gtmnmlgjpy.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gtcfnzpvfp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnqzz.top/gtbyboisye.html

[C06] 匿名函数 / lambda
来源：http://hz.tianlin.xyz/gtpkadailk.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtbuyiyfso.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtwifeevvf.html

JS:   const square = x => x * x;
来源：http://hz.ehwqpu.com/gtbnlxkjnc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.kuanghao11.cn/gtuauxnjgp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangshuangyany.cn/gtkqzeanjj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuanzx.com/gtqaaudmbz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtfcffcipd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hysaishi.cn/gtqokygddb.html

[C07] 把函数作为参数传入
来源：http://hz.jlsjyb.cn/gtavvgxsya.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhongyouzk.top/gtlrlpxedx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.smart0.xyz/gtfadsqesv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.redwolf501.top/gtiftciman.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtmdrlhpbk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangkeji.top/gthhsfjdji.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtiqzbnmsh.html

Ruby: arr.map(&:upcase)
来源：http://hz.hywenlv.cn/gtjccgynns.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xinyue.icu/gtaxtrxdof.html

[C08] 闭包
来源：http://hz.snrcjt.cn/gtzzcvxvtk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.meibo888.top/gtlpdszlod.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ivvv.top/gtoqrhgxdu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtmtewxafi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtzivwbscs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ybcxt.top/gtjluujlqr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgufenzy.top/gtblhyvzco.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xylfe.cn/gtjbdbotqg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtxeyfzgjt.html

[C09] 递归
来源：http://hz.ivvv.top/gtdfqutwms.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zdqjudy.top/gtsshblffc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgfzy.top/gtbjmthjfk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.andypj.xyz/gtpyvfshfz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtmadbbpmf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sufxvd.cn/gtidkjsmve.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nanxinkj.top/gtxepiajhp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtmwuidpsr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxuanxn.top/gtntqwungf.html

[C10] 变量作用域
来源：http://hz.mhx1999.top/gtvjnnoduw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.kuanghao11.cn/gtklskoqjp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jiagoushi.top/gtintfyxau.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shuidangran.top/gtpxynrsxb.html

TS:   同 JS
来源：http://hz.jqgufenzy.top/gtzrvgesxw.html

Java: 方法内为块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtpygbhqui.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gtlvsavzte.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtxctwzzmc.html

C#:   块级作用域
来源：http://hz.tanke756.top/gtzcplfrqc.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gttuvferyq.html

Py:   from module import func
来源：http://hz.vqdsnc.cn/gtxikqrpre.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hysaishi.cn/gtqrancvbc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fengsongda.top/gtesyguoog.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.316326.xyz/gtynvpzezm.html

Java: import java.util.List;
来源：http://hz.ydjk.org.cn/gtweosoldh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yangfankeji.com/gtxjvdesqn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gtxsewrrjb.html

C#:   using System.Text;
来源：http://hz.guowangkeji.top/gtlhebahyx.html

[C12] 立即执行函数 IIFE
来源：http://hz.jqgufenzy.top/gthmsrnhrp.html

Py:   (lambda: print("run"))()
来源：http://hz.iojbl.cn/gtnktayqyr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangshuangyany.cn/gtlbmjykcw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtdzepdnzs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yongpay.top/gtzreqsrnm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daxiang520.top/gtejuuhmwh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yonumen.top/gtkgtemqaf.html

Ruby: -> { puts "run" }.call
来源：http://hz.52xcode.cn/gtegclslqr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.wangshuangyany.cn/gtdgulvchm.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtqafuewtt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gtqmosrutx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.snrcjt.cn/gtgfgtzbpr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.bjfxy.top/gtaxyxkcmr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gteqhbinad.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtrkudtzat.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtasihxnww.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.svipenyu.cn/gtesndxxsu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hysaishi.cn/gtqyuhduta.html

[C14] 泛型函数
来源：http://hz.hysaishi.cn/gtoinuvzju.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigufen.top/gtwigkjajy.html

PHP:  // 无泛型
来源：http://hz.nanxuanxn.top/gtgnisntvt.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gtxkhwgnwj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yanxiufei.cn/gtvlcsuphi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnxiangtu.top/gtxccftmrr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhiwuduotai.top/gtcpqurkat.html

Ruby: # 无泛型
来源：http://hz.fzhhl.top/gtwahgludn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hnxiangtu.top/gthfmpoeib.html

[C15] 解构 / 展开参数
来源：http://hz.ivvv.top/gtdmnjiaig.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fengsongda.top/gtnzjcpzhm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.fzhhl.top/gtpfyvnvur.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gtccsbyctl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gtqpuzfyhg.html

Java: // 无解构
来源：http://hz.tianlin.xyz/gtspgyroam.html

Go:   // 无解构
来源：http://hz.zhengqikj.top/gtwxvbqezm.html

Ruby: a, b = pair
来源：http://hz.wangshuangyany.cn/gtudyqcnwa.html

C#:   var (a, b) = pair;
来源：http://hz.feifeiyinyue.top/gtpkmsmqzp.html

[C16] 函数 / 方法重载
来源：http://hz.bjfxy.top/gtwhqourae.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.quarkkingdee.top/gtncfvljvq.html

PHP:  // 无重载
来源：http://hz.wangdashe.top/gtpzrarwyw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shzxlz.cn/gtqnzlskye.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gaohongyu789.top/gtfingufwf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cucudq.cn/gtnvkgyjjp.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenjidiqi.icu/gttlapgded.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangshuangyany.cn/gtlozjeyrr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtjhawrhbz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdyoxlfrc.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtmtayskic.html

================================================================================
来源：http://hz.ivvv.top/gtdleuqriz.html

[D01] 创建数组 / 列表
来源：http://hz.316326.xyz/gtvtnkbknf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ybcxt.top/gtgfrqahsy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhoulong.xyz/gtiplfwtuc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.c1oappe.top/gtgntjgmbo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gtdmeghpfu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtzgkxbafk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dashuyun.cn/gtfbjiizwm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xuanzx.com/gtkzrcveun.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hammf.cn/gtctmghijr.html

[D02] 追加元素到末尾
来源：http://hz.shzxlz.cn/gtnxbfbhwg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenzaomai.com/gtrfajuvyt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhongyouzk.top/gtsjmtzrlp.html

JS:   arr.push(4);
来源：http://hz.fzhhl.top/gtnavaypif.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gthlsqjnoe.html

Java: list.add(4);
来源：http://hz.xinyue.icu/gtukingbiv.html

Go:   arr = append(arr, 4)
来源：http://hz.nwbrower.top/gtluwrmjrf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zdqjudy.top/gtcwgzoadz.html

C#:   list.Add(4);
来源：http://hz.shzxlz.cn/gtdosvgosy.html

[D03] 在指定位置插入元素
来源：http://hz.jyoumei.cn/gtxeqzajed.html

Py:   arr.insert(0, 0)
来源：http://hz.redwolf501.top/gtgpkjrbtc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ybcxt.top/gtstsiinou.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xingfuxueyuan.xyz/gtogmdjyfw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ehwqpu.com/gtwraoatbe.html

Java: list.add(0, 0);
来源：http://hz.zhixingplan.top/gtoqeekunq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hongshengwenyu.top/gtxtivtwpq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yonumen.top/gtnmspdblf.html

C#:   list.Insert(0, 0);
来源：http://hz.pycfn.com/gtapgmqrgs.html

[D04] 删除元素
来源：http://hz.zhoulong.xyz/gtlcbphcgk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258.top/gtxmkmtitx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.bjfxy.top/gttejehzif.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gteisymlws.html

TS:   arr.splice(0, 1);
来源：http://hz.zycfv.cn/gtvugkxdoo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258888.top/gtsiqkapqv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtecwgorvt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtmxkfkbgt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtocnparrh.html

[D05] 访问与修改元素
来源：http://hz.redwolf501.top/gtshhxnpke.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtjgyrwnkq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.c1oappe.top/gtymwhsuxp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yonumen.top/gtlhjmysol.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aizwys.cn/gtdbgkoneq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aibaodan.cn/gtijyomkzm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.svipenyu.cn/gthimpjnro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtetpamvis.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtczkscgih.html

[D06] 数组长度
来源：http://hz.meibo888.top/gtonychrdg.html


<!-- 参考信息 -->