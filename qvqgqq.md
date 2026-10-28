代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.9152youxi.cn/gtppgxazvi.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gtgaaedlhc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cashguo.top/gtdlxnfdtt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhijiandao.cn/gtwbqzktxn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hongshengwenyu.top/gtwwgjcueg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gtywcqfwoc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.andypj.xyz/gtagmbfbaa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yj202588.top/gtelgaxklf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hywenlv.cn/gtaiyzxbfj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xuanzx.com/gttyypsybd.html

[B07] while 循环
来源：http://hz.chenzaomai.com/gtarvmaigl.html

Py:   while i < 10: i += 1
来源：http://hz.daxiang520.top/gtjqfyjsqr.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xziqi.cn/gtfnphluzm.html

JS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtwzpdurzn.html

TS:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtiibdxvmr.html

Java: while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gtwchfyjgl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.kuanghao11.cn/gtblvwykcx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ppjwa.cn/gtwatavxqy.html

C#:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtpijafyuz.html

[B08] do-while（至少执行一次）
来源：http://hz.ydjk.org.cn/gtasvpsghw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ivvv.top/gtxqtkqpfj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.wangshuangyany.cn/gttydjxghl.html

JS:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtgxwmznmj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtwaprwmme.html

Java: do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtoagojshc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sweek.top/gtwhzsnqoz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhixingplan.top/gtipgvzysa.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtcejyfcdz.html

[B09] break 与 continue
来源：http://hz.jianghu66.top/gtgowulrix.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.9152youxi.cn/gtgjmvbxin.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtzbuoxxkd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtyhxokpcc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtmiaedwjx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtmvhhnscl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258888.top/gtxozzfngt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.meibo888.top/gttezojkmr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gtrfftzewv.html

[B10] 遍历同时拿索引
来源：http://hz.jiagoushi.top/gtnrlqzapd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinyuanbaomall.cn/gtnjuzdbfk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cashguo.top/gtzsordkxm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jianghu66.top/gtqoibwehv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.havefunace.top/gtsxkgcjqj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ppjwa.cn/gtosmbfqkj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hfpthk.cn/gtjixbciwj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.c1oappe.top/gteyibsdep.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.pycfn.com/gtzxmxvgst.html

[B11] 生成数字序列 / 区间
来源：http://hz.nanxuanxn.top/gtynihyfss.html

Py:   list(range(0, 10, 2))
来源：http://hz.birdmap.top/gtuipignnq.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gteucwwapb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtbalimnos.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtvfchempx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.guowangkeji.top/gtncgqsqgz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.mhx1999.top/gtngqibhko.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangtech.top/gtlkdinyrh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cashguo.top/gtqfbwyyaa.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gtoiienuag.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgufenzy.top/gttxscezqr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.haohaochexian.top/gtyfuragmq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenzaomai.com/gtukqlazst.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtxhbzntgq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gtealojnco.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zdqjudy.top/gtkfiowlce.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.bjfxy.top/gtcwkhfhzk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.redwolf501.top/gtzkdztqdf.html

[B13] 判断是否为数字
来源：http://hz.gaohongyu789.top/gtiplewkhp.html

Py:   isinstance(x, (int, float))
来源：http://hz.xinyue.icu/gtwdkbupnt.html

PHP:  is_numeric($x)
来源：http://hz.guannengcc.top/gtzehqtybc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gzhubu.top/gtwyvrduwb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtcilstchq.html

Java: x instanceof Number
来源：http://hz.zhaomingkeji.xyz/gtiapygdcp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtrslupnha.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shzxlz.cn/gtnnbrhmqy.html

C#:   x is int or double or decimal
来源：http://hz.gaohongyu789.top/gtjjofakoq.html

[B14] 判断值是否在集合内
来源：http://hz.shanyushiyangkeji.top/gttcifdnak.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jyoumei.cn/gtsnhnnktq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yangfankeji.com/gtgcunuwkx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gttdhhtjtd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtpyiqmuvv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.quarkkingdee.top/gtncinqnsc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigfzy.top/gtledcybnu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgufenzy.top/gtykwaaeaa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yonumen.top/gtntqxdoiu.html

[B15] 布尔运算与取反
来源：http://hz.ivvv.top/gtluwdrlbg.html

Py:   a and b or not c
来源：http://hz.316326.xyz/gttwjvayfc.html

PHP:  $a && $b || !$c
来源：http://hz.svipenyu.cn/gtocbfgkdc.html

JS:   a && b || !c
来源：http://hz.zhixingplan.top/gtvvireeym.html

TS:   a && b || !c
来源：http://hz.yj20258.top/gtamwdqmvn.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtapfdfoqr.html

Go:   a && b || !c
来源：http://hz.cucudq.cn/gttsrxprhb.html

Ruby: a && b || !c
来源：http://hz.yangfankeji.com/gtnsqwogyw.html

C#:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtweupbpvm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ppjwa.cn/gtjbghexld.html

Py:   if not data: return
来源：http://hz.jinghuilouyu.cn/gtmfxxuxok.html

PHP:  if (!$data) { return; }
来源：http://hz.nwbrower.top/gtfgblfkkz.html

JS:   if (!data) return;
来源：http://hz.havefunace.top/gtrogdrfsu.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtiqvnvoaa.html

Java: if (data == null) return;
来源：http://hz.hongshengwenyu.top/gtefdnfeuz.html

Go:   if data == nil { return }
来源：http://hz.hnxiangtu.top/gthjvguxae.html

Ruby: return if data.nil?
来源：http://hz.hnxiangtu.top/gtroodylqv.html

C#:   if (data == null) return;
来源：http://hz.shuidangran.top/gtnokpmuxm.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfooaahdj.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtvowgknin.html

================================================================================
来源：http://hz.dianchejie.cn/gtilqtceyl.html

[C01] 定义函数
来源：http://hz.smart0.xyz/gtbqenlglb.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxuanxn.top/gtitzxpmmv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtohpxhrth.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ehwqpu.com/gtufxxeybm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.iojbl.cn/gteneeomqd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nwbrower.top/gtwedwtumd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xylfe.cn/gtxkwhbmjy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yongpay.top/gtrahbwjrb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtupcxkblk.html

[C02] 默认参数
来源：http://hz.zhijiandao.cn/gtzedlhtdj.html

Py:   def greet(name="World"): return name
来源：http://hz.cqqwz.cn/gtjcjdliai.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.feifeiyinyue.top/gtnpecsiqj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gturfwqanl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhengqikj.top/gtfdzgbwwt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.smart0.xyz/gtludzgdbr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenlongwang.top/gtrmurlovx.html

Ruby: def greet(name = "World") = name
来源：http://hz.gaohongyu789.top/gtjiigyefe.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.iojbl.cn/gtsjxwtffn.html

[C03] 可变参数
来源：http://hz.cashguo.top/gtimovclcb.html

Py:   def total(*args): return sum(args)
来源：http://hz.yvedp.cn/gtemjcoxmv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinghuilouyu.cn/gtmaqjrisr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtohfzjtpy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtsfjnmkfs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daxiang520.top/gtfhdzztlg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxinkj.top/gttrnueuzh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jqgufenzy.top/gtwnlfyqtn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenjidiqi.icu/gtdwvrposg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtxhvlpkcm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtaoxtoljc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258888.top/gtlsynwrbo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtpdyizqzh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.redwolf501.top/gtyakevzwd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pycfn.com/gtuulbjabe.html

Go:   // 无：用配置结构体参数
来源：http://hz.cqqwz.cn/gtbpqkqhww.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtrnribktn.html

C#:   f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtsuphafvg.html

[C05] 返回多个值
来源：http://hz.quarkkingdee.top/gtjqnzwcyv.html

Py:   return a, b
来源：http://hz.guannengcc.top/gtxapyvlfo.html

PHP:  return [$a, $b];
来源：http://hz.cqqwz.cn/gtzhvqlbua.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.birdmap.top/gtlugekhem.html

TS:   return { a, b };
来源：http://hz.chenlongwang.top/gtwltyugte.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinyuanbaomall.cn/gthfnmztwo.html

Go:   return a, b
来源：http://hz.zhengqikj.top/gtggpimlos.html

Ruby: return a, b
来源：http://hz.hnqzz.top/gthsxjoieb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.52xcode.cn/gtxoenrnyd.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigufen.top/gtrzhzchsx.html

Py:   square = lambda x: x * x
来源：http://hz.ydzc1.top/gtfcxuushr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtfiroglkn.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtbygedqfq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtxdenwrvh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guowangkeji.top/gtowmvpvxl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuetiantiany.cn/gtxbrygaja.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yongpay.top/gtkjhokqre.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhijiandao.cn/gtuuplqkle.html

[C07] 把函数作为参数传入
来源：http://hz.yuxming.cn/gtlyowbkxn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258.top/gtqvpbioso.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.kuanghao11.cn/gtpvmftvqa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jianghu66.top/gthydhuruo.html

TS:   arr.map(String)
来源：http://hz.pycfn.com/gtmftadyoy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dashuyun.cn/gtwvjgeyij.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.316326.xyz/gthkdklclj.html

Ruby: arr.map(&:upcase)
来源：http://hz.cqqwz.cn/gtuvzkmjmq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nwbrower.top/gttswyqydl.html

[C08] 闭包
来源：http://hz.vqdsnc.cn/gtcybuzdxe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtogxynunb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guannengcc.top/gtclinzobm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtrsnfmvnp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gteofwzjei.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtgglswjtv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtnmwzwzpt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gttctgnwvs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtvfgvysay.html

[C09] 递归
来源：http://hz.jianghu66.top/gtdzcdvspf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.birdmap.top/gtlkonklqm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jiagoushi.top/gtnrjbbows.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtisrujuhi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtkudndoyh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yueranfly.top/gtqbhalcov.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sweek.top/gtihhlhzkc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gzhubu.top/gttvfjoxdu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.meibo888.top/gtkngrtgkt.html

[C10] 变量作用域
来源：http://hz.gzhubu.top/gtwvvtcqsb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nanxuanxn.top/gtxglhzerp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pycfn.com/gtdetnrvod.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gzhubu.top/gtilccvzsa.html

TS:   同 JS
来源：http://hz.shuidangran.top/gtlkqpiait.html

Java: 方法内为块级作用域
来源：http://hz.aizwys.cn/gtsvleicuf.html

Go:   花括号块级作用域
来源：http://hz.pycfn.com/gtexpkdsbk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtcfkoyluj.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtubqacmyd.html

[C11] 模块导入与导出
来源：http://hz.gogol.net.cn/gtjazclkdg.html

Py:   from module import func
来源：http://hz.yuxming.cn/gtdybrymdo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258888.top/gtiyqjmrbo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jianghu66.top/gtutqodapa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.dashuyun.cn/gtngzrdcqj.html

Java: import java.util.List;
来源：http://hz.yangfankeji.com/gtsxixanvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cdnleiting.top/gttjolpllq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.52xcode.cn/gtgmtbcpxt.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gtjhdunbbk.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtwbbgpdps.html

Py:   (lambda: print("run"))()
来源：http://hz.jinghuilouyu.cn/gtyrkqpbsr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydzc1.top/gtzhmoqjet.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtjtcyvfjg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtwnrznaea.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hfpthk.cn/gtmmvdfeuy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtgnpzzkwh.html

Ruby: -> { puts "run" }.call
来源：http://hz.andypj.xyz/gtqtfmuqij.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtbwwzkbaz.html

[C13] 类型声明 / 类型注解
来源：http://hz.vqdsnc.cn/gtnlmdvfzv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.mhx1999.top/gtqzuafqon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gthackewnz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.quarkkingdee.top/gtxklktqyq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtnlnmeveh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtgmolipxm.html

Go:   func add(a, b int) int
来源：http://hz.yj20258888.top/gtiugzkbfj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zycfv.cn/gtnskqlesg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gotoacloud.top/gtvhdteqnc.html

[C14] 泛型函数
来源：http://hz.yonumen.top/gtzluwibtx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gthhkrtbbd.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtzfzziuzv.html

JS:   // 无泛型
来源：http://hz.vqdsnc.cn/gthtcqqahv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xinyue.icu/gtgslhgggq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtcjvoimmu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinghuilouyu.cn/gtmfoxicxe.html

Ruby: # 无泛型
来源：http://hz.sufxvd.cn/gtgliuxand.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sufxvd.cn/gtrtxyklbu.html

[C15] 解构 / 展开参数
来源：http://hz.ivvv.top/gtpqbzkqlu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tanke756.top/gtpshqigcr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtegnwwffy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.iojbl.cn/gthjpgwwat.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jiagoushi.top/gthhnhbqmi.html

Java: // 无解构
来源：http://hz.chenzaomai.com/gtepsqcleb.html

Go:   // 无解构
来源：http://hz.jqgfzy.top/gtjvubhsle.html

Ruby: a, b = pair
来源：http://hz.dianchejie.cn/gtgrqzjmdb.html

C#:   var (a, b) = pair;
来源：http://hz.sweek.top/gtkbpitcfw.html

[C16] 函数 / 方法重载
来源：http://hz.zhijiandao.cn/gtpmskgurr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.havefunace.top/gtqzuvsioo.html

PHP:  // 无重载
来源：http://hz.sxryk.cn/gttziqjxuv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.svipenyu.cn/gtxaihylfz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtrthbrudb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtuqqobfvy.html

Go:   // 无重载：用不同函数名
来源：http://hz.svipenyu.cn/gttcfjjijz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.316326.xyz/gtvjonsodq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangkeji.top/gtegbecqqd.html

================================================================================
来源：http://hz.jianghu66.top/gtmfvwyanh.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigufen.top/gtgyamndlp.html

================================================================================
来源：http://hz.daxiang520.top/gtfkplpqnd.html

[D01] 创建数组 / 列表
来源：http://hz.ywan-chungtsiang.top/gtkkwlvmua.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.9152youxi.cn/gtygsvzucf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shuidangran.top/gtxjnqdcwy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gttsqdcdts.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.0kj1m.cn/gtuyavxdey.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jlsjyb.cn/gtcauohdio.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtsnpbrrkp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gzhubu.top/gtjzkkxusi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydzc1.top/gtcphynfxy.html

[D02] 追加元素到末尾
来源：http://hz.gotoacloud.top/gtaccdafqc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.52xcode.cn/gtjdnjshov.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuetiantiany.cn/gtghnpyesu.html

JS:   arr.push(4);
来源：http://hz.yvedp.cn/gttskakkpt.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtplulwdeh.html

Java: list.add(4);
来源：http://hz.chenlongwang.top/gtdjxccdpm.html

Go:   arr = append(arr, 4)
来源：http://hz.zhiwuduotai.top/gtjnlazwvj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guannengcc.top/gtuwktkdee.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtthyvcriw.html

[D03] 在指定位置插入元素
来源：http://hz.andypj.xyz/gtjaegejzp.html

Py:   arr.insert(0, 0)
来源：http://hz.shangyingyoupin.top/gtolkpzvkm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gthkjftrxw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xinyue.icu/gtjnfruwhr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sxryk.cn/gtmhzcciuy.html

Java: list.add(0, 0);
来源：http://hz.0kj1m.cn/gtcdfyzmny.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pengpengdd.cyou/gthlnsyvym.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhongyouzk.top/gtmnukjlkv.html

C#:   list.Insert(0, 0);
来源：http://hz.daxiang520.top/gtduknkvja.html

[D04] 删除元素
来源：http://hz.jqgufenzy.top/gtyzkodzfq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gtbjayxmpr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xuetiantiany.cn/gtzzxnxpnt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yanxiufei.cn/gtveycsnji.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gtjnydkbag.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daxiang520.top/gtpjsfikuk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aibaodan.cn/gterzwtoex.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtxpcrmile.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gtfozmslwu.html

[D05] 访问与修改元素
来源：http://hz.cheryme.top/gtspzfhfpc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtoyawnsaz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtamzdtxqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xziqi.cn/gtwvzjmgcg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydzc1.top/gtzqtfipki.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj202588.top/gtxhcuhpmo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtgipqukhc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtwewcetkp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuxming.cn/gtjrxuuvon.html

[D06] 数组长度
来源：http://hz.mhx1999.top/gtrcjuuewx.html

Py:   len(arr)
来源：http://hz.guannengcc.top/gtcwhckzmj.html

PHP:  count($arr);
来源：http://hz.gzhubu.top/gtgsocqhgg.html

JS:   arr.length
来源：http://hz.pengpengdd.cyou/gtmwronagu.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtnvzhtgft.html


<!-- 参考信息 -->