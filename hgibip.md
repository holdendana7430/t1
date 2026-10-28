代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangshuangyany.cn/gtxinbpsqj.html

[B06] 遍历字典 / 对象
来源：http://hz.daria6918.cn/gtjmjznkrq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cucudq.cn/gtksckzlbk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.havefunace.top/gtgdqrwdjo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aizwys.cn/gtvmetagjv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gthcyzfegs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.dashuyun.cn/gtwtnoncgb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.fengsongda.top/gtboccsgbf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxuanxn.top/gtwhunwehq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.vqdsnc.cn/gtwdkfntuk.html

[B07] while 循环
来源：http://hz.zhiwuduotai.top/gtctvqxipu.html

Py:   while i < 10: i += 1
来源：http://hz.zhixingplan.top/gteexbpmax.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.daxiang520.top/gtrwzqcqvw.html

JS:   while (i < 10) { i++; }
来源：http://hz.svipenyu.cn/gtcqbqxqnk.html

TS:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtiaqnptfo.html

Java: while (i < 10) { i++; }
来源：http://hz.xziqi.cn/gtcntmdtyq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangshuangyany.cn/gtwprxhotc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ppjwa.cn/gtmbkfrysa.html

C#:   while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtddwspsyd.html

[B08] do-while（至少执行一次）
来源：http://hz.sweek.top/gtgivdoozl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.havefunace.top/gtqrimzykg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hysaishi.cn/gtabcimiwb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtjlcusrut.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtiuxguyka.html

Java: do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtesstamgl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nanxuanxn.top/gtlrbrykek.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zycfv.cn/gtnqhiiixo.html

C#:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtcdvgcoiw.html

[B09] break 与 continue
来源：http://hz.zhoulong.xyz/gtorhfgbcl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zycfv.cn/gtjpvojqix.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtccevomix.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtjakujjph.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtgayjbysf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtzdwfpyay.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.birdmap.top/gthiawihha.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gtcxlweblu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtejxbukdf.html

[B10] 遍历同时拿索引
来源：http://hz.yonumen.top/gtgoyaozpr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hammf.cn/gtncnfzgka.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gogol.net.cn/gtuyquwvvj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenzaomai.com/gtzjdtmoof.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.316326.xyz/gtpodlzjei.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sysykeji.top/gtxpxajbup.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xziqi.cn/gtzuoorzus.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.dianchejie.cn/gtkmetrmlr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nanxinkj.top/gtecydeqnc.html

[B11] 生成数字序列 / 区间
来源：http://hz.nwbrower.top/gtggepgxer.html

Py:   list(range(0, 10, 2))
来源：http://hz.aizwys.cn/gttjtpfczo.html

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtomogyzgl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxuanxn.top/gtuxrqdpex.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtewipanny.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenzaomai.com/gtzjvrmdii.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.snrcjt.cn/gtwiflqoid.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gtdhnnaulo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xziqi.cn/gtxihiggsv.html

[B12] 跳出多层循环
来源：http://hz.pengpengdd.cyou/gtreunckbg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.aibaodan.cn/gtvcolgjgm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tianlin.xyz/gtsftwmhld.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gthjbjcpyh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtuivjixxf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tianlin.xyz/gttjbdkcjy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.mhx1999.top/gtrrcujcmh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jianghu66.top/gtufqghpsr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ivvv.top/gtzgpossrw.html

[B13] 判断是否为数字
来源：http://hz.zhiwuduotai.top/gtjmkxllfo.html

Py:   isinstance(x, (int, float))
来源：http://hz.yanxiufei.cn/gtuvvmkglk.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gtmdffpefi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtpjdpmgov.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ppjwa.cn/gtegwrbuws.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gtiwzmhqnt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.iojbl.cn/gtehdqaryw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.andypj.xyz/gttfzffnnh.html

C#:   x is int or double or decimal
来源：http://hz.ehwqpu.com/gtewjjbaqm.html

[B14] 判断值是否在集合内
来源：http://hz.ivvv.top/gtzmmmbmyr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.52xcode.cn/gtxvmzvzzb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydjk.org.cn/gtuntrmtak.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtfzkinule.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtndfnrbpj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.52xcode.cn/gtvrhstnrq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.9152youxi.cn/gtaegcnlsb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.smart0.xyz/gtnelzfolj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gthrmdmedk.html

[B15] 布尔运算与取反
来源：http://hz.gotoacloud.top/gtlnzqgesv.html

Py:   a and b or not c
来源：http://hz.yuxming.cn/gtjmzoctni.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gthslboyfj.html

JS:   a && b || !c
来源：http://hz.zhengqikj.top/gtbfhobdiu.html

TS:   a && b || !c
来源：http://hz.jqgufenzy.top/gtvkguzsuc.html

Java: a && b || !c
来源：http://hz.9152youxi.cn/gtqfedyysr.html

Go:   a && b || !c
来源：http://hz.havefunace.top/gtwizvknod.html

Ruby: a && b || !c
来源：http://hz.quarkkingdee.top/gtyixhfjpg.html

C#:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtpvmjdtqi.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jiagoushi.top/gtwpzeykww.html

Py:   if not data: return
来源：http://hz.sweek.top/gtwrhasyiu.html

PHP:  if (!$data) { return; }
来源：http://hz.redwolf501.top/gtjupqvjuk.html

JS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtffqrjxvd.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtxwodlthy.html

Java: if (data == null) return;
来源：http://hz.ivvv.top/gtotokorru.html

Go:   if data == nil { return }
来源：http://hz.shangyingyoupin.top/gtqewxnjmq.html

Ruby: return if data.nil?
来源：http://hz.daxiang520.top/gtarryrfcy.html

C#:   if (data == null) return;
来源：http://hz.nwbrower.top/gtihslfxlh.html

================================================================================
来源：http://hz.zhixingplan.top/gtfolrdkfd.html

C. 函数与作用域
来源：http://hz.316326.xyz/gtncgoghtd.html

================================================================================
来源：http://hz.sysykeji.top/gtjikuoiik.html

[C01] 定义函数
来源：http://hz.feifeiyinyue.top/gtexkjwsfi.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangtech.top/gtlxloglly.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtiljluscc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gteqhvamwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtkyworzeu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtucozzvfw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hnxiangtu.top/gtlruirbik.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daria6918.cn/gttsgtxvki.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gttrjjztib.html

[C02] 默认参数
来源：http://hz.smart0.xyz/gtzvzbprsw.html

Py:   def greet(name="World"): return name
来源：http://hz.52xcode.cn/gtbvcnflul.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.smart0.xyz/gtygwhlsvc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtwmkfxuak.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tanke756.top/gtgzaicjyz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ivvv.top/gtrdhqwfhx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtsesvttbv.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtijcmlvan.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cheryme.top/gtsvifdopx.html

[C03] 可变参数
来源：http://hz.tianlin.xyz/gtdxmukyon.html

Py:   def total(*args): return sum(args)
来源：http://hz.fzhhl.top/gtslrrixdy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.svipenyu.cn/gtsyvrtwmm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtnramkubu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gthljdktur.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.feifeiyinyue.top/gtxxfduaov.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgufenzy.top/gtpzsajkdz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhengqikj.top/gtdyaroesm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gtphzesgxw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtmsoewkhq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yangfankeji.com/gtdxvrmkjd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jianghu66.top/gtntpvwnro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yongpay.top/gtgdsbqynb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigufen.top/gtjlzfdnbw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gtmixvxdpa.html

Go:   // 无：用配置结构体参数
来源：http://hz.hnqzz.top/gtuxiofwns.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtpxmvasbc.html

C#:   f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gtmesbzplr.html

[C05] 返回多个值
来源：http://hz.jinghuilouyu.cn/gtwvbndgvp.html

Py:   return a, b
来源：http://hz.sufxvd.cn/gthvyottdf.html

PHP:  return [$a, $b];
来源：http://hz.xylfe.cn/gtlfxfockd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gogol.net.cn/gtaofxyhrh.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtulktqndj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fzhhl.top/gtheaevacy.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtwytjklwi.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtfejzlfuh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tianlin.xyz/gtvdcyvhop.html

[C06] 匿名函数 / lambda
来源：http://hz.gzhubu.top/gtttgiwnci.html

Py:   square = lambda x: x * x
来源：http://hz.cucudq.cn/gtfjpynemw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ybcxt.top/gtkelqkear.html

JS:   const square = x => x * x;
来源：http://hz.iojbl.cn/gtgccdpowd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj202588.top/gtrkevxusw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shuidangran.top/gtridzaarj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgufenzy.top/gtfkpuqbzk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtsjnktrmb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtfgkcdcek.html

[C07] 把函数作为参数传入
来源：http://hz.xziqi.cn/gtsrgjfydx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuetiantiany.cn/gtsccyvtki.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.birdmap.top/gtndvqwuex.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtclcbkdxp.html

TS:   arr.map(String)
来源：http://hz.0kj1m.cn/gtlhubrbjf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.9152youxi.cn/gtdjgqmxug.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtocryktnv.html

Ruby: arr.map(&:upcase)
来源：http://hz.daxiang520.top/gtfibykuyf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sufxvd.cn/gtoukttvcg.html

[C08] 闭包
来源：http://hz.zhongyouzk.top/gtfyglwgom.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtpiovjwkd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dianchejie.cn/gtiepmkehl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtxvazcgzl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gttrkyfiag.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sxryk.cn/gtjgqefmlq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jianghu66.top/gtkqivygap.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangdashe.top/gtyvxffgyt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtxnzannty.html

[C09] 递归
来源：http://hz.52xcode.cn/gtvaasdfgi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xylfe.cn/gtifhehcdz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hnqzz.top/gttxlxaqpq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jianghu66.top/gtqifxswjv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fengsongda.top/gthaebqemn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.daria6918.cn/gtxhjkbhax.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnqzz.top/gtddzsffjr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtcizlmdxm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guannengcc.top/gtvdzhnqhm.html

[C10] 变量作用域
来源：http://hz.cdnleiting.top/gtgtmexgbf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.snrcjt.cn/gtmhhnkgxb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zycfv.cn/gtzkugewvz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigfzy.top/gtdebvzkik.html

TS:   同 JS
来源：http://hz.kuanghao11.cn/gtwhfuvrdl.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtzoqgslrc.html

Go:   花括号块级作用域
来源：http://hz.feifeiyinyue.top/gtroxaessk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinyuanbaomall.cn/gtcpujgebj.html

C#:   块级作用域
来源：http://hz.zhongyouzk.top/gtlrxulreb.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtlqiqvtdq.html

Py:   from module import func
来源：http://hz.meibo888.top/gtxgbtenap.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yanxiufei.cn/gtibmlgpaz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinqigfzy.top/gtxrjfbiog.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnqzz.top/gtmdtspjfo.html

Java: import java.util.List;
来源：http://hz.daria6918.cn/gtvyxdrvdw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinghuilouyu.cn/gtaernmdbe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sysykeji.top/gttbtkvncq.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gtjcucnegu.html

[C12] 立即执行函数 IIFE
来源：http://hz.dashuyun.cn/gtjkhblzyl.html

Py:   (lambda: print("run"))()
来源：http://hz.xingfuxueyuan.xyz/gtcikldlif.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aibaodan.cn/gtnjwyowdu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtjxsbbahf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxuanxn.top/gtoeyidgqv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangdashe.top/gtninpofcd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangtech.top/gtyoodldzt.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhengqikj.top/gtwnhgrvhn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtwjqkxtwa.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtjunupmez.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gtzxwrvuwd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtsakwxbgv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.havefunace.top/gtoobqvpaz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cdnleiting.top/gtpydqttoq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtfvknxjib.html

Go:   func add(a, b int) int
来源：http://hz.fzhhl.top/gtvioihbro.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnqzz.top/gtaolzkyxf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xylfe.cn/gtxysjrnaz.html

[C14] 泛型函数
来源：http://hz.gzhubu.top/gtimjrbqru.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gttvxxvcro.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gtrwyejnhq.html

JS:   // 无泛型
来源：http://hz.yongpay.top/gtudlcuvsl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tianlin.xyz/gtpwqnvece.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gthwktgntu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gotoacloud.top/gtmvdlxzyw.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtujnmnvaj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gogol.net.cn/gtbsrgcilr.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtsolgroxp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuanzhike.top/gtjgctseyb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yanxiufei.cn/gtyhagvtid.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtpcrzxipd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenzaomai.com/gtmvkbruuh.html

Java: // 无解构
来源：http://hz.ywan-chungtsiang.top/gthldcedrh.html

Go:   // 无解构
来源：http://hz.shanyushiyangtech.top/gtuxpkjdie.html

Ruby: a, b = pair
来源：http://hz.xingfuxueyuan.xyz/gtncensdid.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gtvmxaqenz.html

[C16] 函数 / 方法重载
来源：http://hz.fengsongda.top/gtpbyuzkrc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aibaodan.cn/gtsuxjbhcy.html

PHP:  // 无重载
来源：http://hz.yonumen.top/gtllcnixua.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jlsjyb.cn/gtqotsxany.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gthjaollvc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ppjwa.cn/gtrfwrvhjr.html

Go:   // 无重载：用不同函数名
来源：http://hz.tanke756.top/gthxjwxrav.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxuanxn.top/gtsrkmpclu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shzxlz.cn/gtqiagofgz.html

================================================================================
来源：http://hz.xziqi.cn/gtkgnmigdp.html

D. 数组 / 列表 / 集合
来源：http://hz.cucudq.cn/gtyxwcnjph.html

================================================================================
来源：http://hz.jinqigfzy.top/gtslygpimt.html

[D01] 创建数组 / 列表
来源：http://hz.zhiwuduotai.top/gtskeoaemo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yangfankeji.com/gtqpvgnzkq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtqvisbege.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnxiangtu.top/gtwmslkkqj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenzaomai.com/gtncepvhex.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gtnmltsvhw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fengsongda.top/gtawzmdxrw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtlxcmoyvk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuetiantiany.cn/gttrdgpoga.html

[D02] 追加元素到末尾
来源：http://hz.guannengcc.top/gtqlbdpxrz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.feifeiyinyue.top/gtujqummbi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinghuilouyu.cn/gtucsykwsq.html

JS:   arr.push(4);
来源：http://hz.guowangkeji.top/gtplyhhzob.html

TS:   arr.push(4);
来源：http://hz.ybcxt.top/gtjzmlwfot.html

Java: list.add(4);
来源：http://hz.cdnleiting.top/gtfqqbftan.html

Go:   arr = append(arr, 4)
来源：http://hz.shangyingyoupin.top/gtrvvyqlip.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cashguo.top/gtmecvgfzr.html

C#:   list.Add(4);
来源：http://hz.zhengqikj.top/gtcplnkyvj.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtciclkbyt.html

Py:   arr.insert(0, 0)
来源：http://hz.shangyingyoupin.top/gtcjpwfnjf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gtvrprhafs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yongpay.top/gtfhvzndlz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ivvv.top/gtanisxkvw.html

Java: list.add(0, 0);
来源：http://hz.daria6918.cn/gtwjfaydli.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnxiangtu.top/gtieikqpxg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.vqdsnc.cn/gtsifneskl.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtoyixrhav.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtfpxrzttm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cucudq.cn/gtadyqfcfw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.redwolf501.top/gtqmzpiahg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtpgtrrbqz.html

TS:   arr.splice(0, 1);
来源：http://hz.jlsjyb.cn/gtypsuhmrr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jqgfzy.top/gtzbzthlwn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtkplgzili.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hywenlv.cn/gtyoospldt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aizwys.cn/gtemqowode.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtvslpkqwq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtdllpirvn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtqlauzdiy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nwbrower.top/gthxuyodvi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sysykeji.top/gtvxvcwouu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtrmhyqtwj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtczrbqeuz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtmsxmfcth.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxuanxn.top/gtjspfkwha.html

[D06] 数组长度
来源：http://hz.feifeiyinyue.top/gtmkgjmhcl.html

Py:   len(arr)
来源：http://hz.meibo888.top/gtjphyxznh.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtpbgesndp.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtoaqsjgdx.html

TS:   arr.length
来源：http://hz.nwbrower.top/gtbqiilrld.html


<!-- 参考信息 -->