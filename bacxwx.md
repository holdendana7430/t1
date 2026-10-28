代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangdashe.top/gtatthfyfn.html

[B06] 遍历字典 / 对象
来源：http://hz.guannengcc.top/gtplifdjjy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.redwolf501.top/gtuwjvfedc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yuanzhike.top/gtvviobobv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgfzy.top/gtsvzzgwvk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.guannengcc.top/gtvbqnpqxg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.vqdsnc.cn/gtnrxmasbc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jqgufenzy.top/gteqidaxlm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xuanzx.com/gtgqicxerh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yanxiufei.cn/gtrthqnvyc.html

[B07] while 循环
来源：http://hz.c1oappe.top/gtfddzdwqm.html

Py:   while i < 10: i += 1
来源：http://hz.ybcxt.top/gtnroyfvkq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yongpay.top/gtkuxypton.html

JS:   while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtyuhxcgkv.html

TS:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtrwgimzdt.html

Java: while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gttpwsylud.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sufxvd.cn/gtokietlsu.html

Ruby: while i < 10; i += 1; end
来源：http://hz.fengsongda.top/gtyevkfjhc.html

C#:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtkyswpgiu.html

[B08] do-while（至少执行一次）
来源：http://hz.shangyingyoupin.top/gtcvgofbap.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxuanxn.top/gtuimagzey.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.316326.xyz/gtymxztvop.html

JS:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gteqpwjqgw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtltebbeav.html

Java: do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtlqtpxyqg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gtrkdvfzwj.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.redwolf501.top/gtbuggyjvf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtepsegipd.html

[B09] break 与 continue
来源：http://hz.jlsjyb.cn/gtdpozlqvn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jiagoushi.top/gtxfyeodsb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.wangdashe.top/gtpbmrsmbt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtkbupnylw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gthpjjbqny.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtrfrgpwux.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.c1oappe.top/gtdjvabibj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhengqikj.top/gthtegqtwu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtnbwpaasz.html

[B10] 遍历同时拿索引
来源：http://hz.snrcjt.cn/gtjxbwdzbk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.0kj1m.cn/gtplfcihxi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhijiandao.cn/gtqaxixkhg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtjpczajzn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.52xcode.cn/gtwblumxrd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hnxiangtu.top/gtttyxqhci.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.dashuyun.cn/gtjjhhriof.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shzxlz.cn/gtzoqkycjs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cdnleiting.top/gtogchkvhq.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtolxygkon.html

Py:   list(range(0, 10, 2))
来源：http://hz.meibo888.top/gtvcawfhmc.html

PHP:  range(0, 10, 2);
来源：http://hz.yanxiufei.cn/gtvkqvtijl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gaohongyu789.top/gtpjbjvnxq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.snrcjt.cn/gtefpxkmrv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangdashe.top/gtzwbbjqfd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.andypj.xyz/gtdqbgfckg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj202588.top/gtortvkymd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xuetiantiany.cn/gtkoxgrftg.html

[B12] 跳出多层循环
来源：http://hz.c1oappe.top/gtrxtytase.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.guannengcc.top/gtotqzibdn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zycfv.cn/gtnnrrlwlu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtqvatfprb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtccvwukzq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtctwrltgf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.aizwys.cn/gtfpcsgfgf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shuidangran.top/gthkarcysf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.vqdsnc.cn/gtohdtszyb.html

[B13] 判断是否为数字
来源：http://hz.jinghuilouyu.cn/gtcngoufgk.html

Py:   isinstance(x, (int, float))
来源：http://hz.ydjk.org.cn/gtkcmqxpwb.html

PHP:  is_numeric($x)
来源：http://hz.tian-w.cn/gtdqxowhnw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtlombafod.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtxmutfhdu.html

Java: x instanceof Number
来源：http://hz.wangdashe.top/gtzenaybor.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sufxvd.cn/gteqxsfzkv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.dashuyun.cn/gtpqahujoj.html

C#:   x is int or double or decimal
来源：http://hz.cdnleiting.top/gtssmevohl.html

[B14] 判断值是否在集合内
来源：http://hz.feifeiyinyue.top/gtfvjycyrg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sufxvd.cn/gtxafrptyr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gotoacloud.top/gtzrnodquq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtapdggttj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtplzyvtpd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtjcjcqtpf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.smart0.xyz/gtelosqpmx.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.quarkkingdee.top/gtueijrjlt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtycmxfodt.html

[B15] 布尔运算与取反
来源：http://hz.svipenyu.cn/gtjswmhcdr.html

Py:   a and b or not c
来源：http://hz.yanxiufei.cn/gthnaviiny.html

PHP:  $a && $b || !$c
来源：http://hz.zhoulong.xyz/gtipoixffn.html

JS:   a && b || !c
来源：http://hz.cucudq.cn/gtjlzzhtfz.html

TS:   a && b || !c
来源：http://hz.fengsongda.top/gtxmskgtqh.html

Java: a && b || !c
来源：http://hz.hfpthk.cn/gtfuicnjcl.html

Go:   a && b || !c
来源：http://hz.xinyue.icu/gtkzfusxry.html

Ruby: a && b || !c
来源：http://hz.yanxiufei.cn/gtfjcnshej.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gttiqwnkmh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ppjwa.cn/gtwannsawn.html

Py:   if not data: return
来源：http://hz.yj20258888.top/gttjnhvkua.html

PHP:  if (!$data) { return; }
来源：http://hz.daria6918.cn/gtutolilnk.html

JS:   if (!data) return;
来源：http://hz.tanke756.top/gtwnzsmhvm.html

TS:   if (!data) return;
来源：http://hz.yongpay.top/gtcwrujkdq.html

Java: if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gtiqkohsai.html

Go:   if data == nil { return }
来源：http://hz.xingfuxueyuan.xyz/gtahgsfhyl.html

Ruby: return if data.nil?
来源：http://hz.wangdashe.top/gthkmhnwbc.html

C#:   if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtmwkoaujf.html

================================================================================
来源：http://hz.havefunace.top/gtdawzmbaf.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtwfqylsya.html

================================================================================
来源：http://hz.hfpthk.cn/gtwptjnang.html

[C01] 定义函数
来源：http://hz.zdqjudy.top/gtfhicsnny.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtevxkixwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtatchsyci.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtvgkqhrbp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtodegpbeq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtbiooytgs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fzhhl.top/gtmlpyjhwj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zdqjudy.top/gtzupgcunu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtvyllitkv.html

[C02] 默认参数
来源：http://hz.feifeiyinyue.top/gtamhpmgae.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258888.top/gttvgdspki.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hongshengwenyu.top/gtnzynybyr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtcptrmspl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtfhxlgwag.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tianlin.xyz/gthntwkoqe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuetiantiany.cn/gtiwizwfjz.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gtdoldtumm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yvedp.cn/gtwsbaxirn.html

[C03] 可变参数
来源：http://hz.andypj.xyz/gtmgzewscy.html

Py:   def total(*args): return sum(args)
来源：http://hz.jqgufenzy.top/gtumcfrehb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxuanxn.top/gtpopvsfav.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtppurncif.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtwzogmfku.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yvedp.cn/gtqparzevk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fzhhl.top/gtintyvzbb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.kuanghao11.cn/gtnhnrgyrl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuetiantiany.cn/gtxxohhrlr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nwbrower.top/gtjxuangli.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinyuanbaomall.cn/gthpbuqekk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hongshengwenyu.top/gtrntmigan.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.birdmap.top/gtfsmffkyg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shzxlz.cn/gtssyxbbiq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.andypj.xyz/gtdbmvodmd.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtpgkhdpwz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtajcgiuxj.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtmczhkrhq.html

[C05] 返回多个值
来源：http://hz.smart0.xyz/gthyneanvr.html

Py:   return a, b
来源：http://hz.zycfv.cn/gtnogwcrnm.html

PHP:  return [$a, $b];
来源：http://hz.ywan-chungtsiang.top/gtwaafhenb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daxiang520.top/gtwrowzgiu.html

TS:   return { a, b };
来源：http://hz.shuidangran.top/gtdaxhmkmd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.vqdsnc.cn/gtnjtzemgl.html

Go:   return a, b
来源：http://hz.hysaishi.cn/gtcoyicrrw.html

Ruby: return a, b
来源：http://hz.gaohongyu789.top/gtrtveykco.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yangfankeji.com/gtirpxiize.html

[C06] 匿名函数 / lambda
来源：http://hz.birdmap.top/gtipuqghtu.html

Py:   square = lambda x: x * x
来源：http://hz.zhoulong.xyz/gtrevosnai.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ppjwa.cn/gtucdyndef.html

JS:   const square = x => x * x;
来源：http://hz.ivvv.top/gtfssshafy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.svipenyu.cn/gtldxyfhbl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.havefunace.top/gtoeznxkyf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tanke756.top/gtqyeegoow.html

Ruby: square = ->(x) { x * x }
来源：http://hz.feifeiyinyue.top/gtsqncaazk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dianchejie.cn/gtgnekecnm.html

[C07] 把函数作为参数传入
来源：http://hz.hysaishi.cn/gtovfnkjta.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shzxlz.cn/gtrfiejymx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinyuanbaomall.cn/gtqrudknwm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtxruymvbg.html

TS:   arr.map(String)
来源：http://hz.fzhhl.top/gtzfridhkv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tanke756.top/gtcsxapmwn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dashuyun.cn/gtdspsmhcv.html

Ruby: arr.map(&:upcase)
来源：http://hz.zycfv.cn/gtlvneuhoa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xuanzx.com/gtlzemnpxh.html

[C08] 闭包
来源：http://hz.0kj1m.cn/gtgbhsaawg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jianghu66.top/gtazaebieo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xinyue.icu/gtaapesbxj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gttorfdmcp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gthkethkuo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yanxiufei.cn/gtwamvaevp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtjpvslxqy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cashguo.top/gtztdmrrjm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtytpthcbq.html

[C09] 递归
来源：http://hz.smart0.xyz/gtawakdzrl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.andypj.xyz/gtcwcqjmpr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtsersvdxy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtwmcxmlzt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.0kj1m.cn/gtpcyjhaul.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj202588.top/gtslwqwhgz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zycfv.cn/gtqiwfnyer.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gtmcpiqlts.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.birdmap.top/gtqxcmrwsz.html

[C10] 变量作用域
来源：http://hz.daxiang520.top/gtwwzhzdta.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258.top/gthxbmxewu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ywan-chungtsiang.top/gtrfdnbqks.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenjidiqi.icu/gtewhfuweb.html

TS:   同 JS
来源：http://hz.yj20258.top/gtxapgirys.html

Java: 方法内为块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtzkgeposo.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtadcujqgj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cashguo.top/gtuwnyzjgs.html

C#:   块级作用域
来源：http://hz.jinyuanbaomall.cn/gtyezsecmi.html

[C11] 模块导入与导出
来源：http://hz.tianlin.xyz/gthpjxxngn.html

Py:   from module import func
来源：http://hz.yj20258888.top/gtwvywealg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shangyingyoupin.top/gtljrhgmwq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.snrcjt.cn/gtfdeexgcb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.svipenyu.cn/gtnrbjagre.html

Java: import java.util.List;
来源：http://hz.wangdashe.top/gtvtoieiuj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.pengpengdd.cyou/gtljqjdudt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhoulong.xyz/gtmfkeohlj.html

C#:   using System.Text;
来源：http://hz.guannengcc.top/gthnaixslj.html

[C12] 立即执行函数 IIFE
来源：http://hz.dashuyun.cn/gtntkckhme.html

Py:   (lambda: print("run"))()
来源：http://hz.ybcxt.top/gtngsxhegb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtteqduxca.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtjqxdvzge.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtlcehlmph.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtrqevgngo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtpisiufhn.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangshuangyany.cn/gthplsdjde.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnxiangtu.top/gtwejcqiva.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinqigufen.top/gtixmfcran.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtlhrglscn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtjxurscta.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cheryme.top/gtzxpjapsn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtuqsmbevz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtzmdwcahg.html

Go:   func add(a, b int) int
来源：http://hz.cheryme.top/gtyymyqvhd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tanke756.top/gtawhhxinb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cashguo.top/gtkrdrhjhf.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtbdzzzduu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yueranfly.top/gtpzihfiuk.html

PHP:  // 无泛型
来源：http://hz.haohaochexian.top/gtowxhahds.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gtrkdwlapq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgfzy.top/gtywtzyxmh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtebmjsxgf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtnfodcvwp.html

Ruby: # 无泛型
来源：http://hz.pengpengdd.cyou/gtdaumkdwi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yvedp.cn/gtvuaxnrxe.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtlqhsbuky.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gtraqhtesm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtlagjehvu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtaktfobuy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtuyajwcrf.html

Java: // 无解构
来源：http://hz.hfpthk.cn/gtsupaciec.html

Go:   // 无解构
来源：http://hz.tanke756.top/gtmdkdvmsa.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtbntvgder.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gtvasiwwdq.html

[C16] 函数 / 方法重载
来源：http://hz.316326.xyz/gtlxcuvxwz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ehwqpu.com/gtskaysrdc.html

PHP:  // 无重载
来源：http://hz.cucudq.cn/gtnjmmmhok.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhoulong.xyz/gtnibyftwv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yvedp.cn/gtyngyqtpc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cheryme.top/gtztexyauz.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuetiantiany.cn/gtmcgvrlvd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.haohaochexian.top/gtnbvqmddg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gtsicwzcrb.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoimzxxur.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtdgcopxpl.html

================================================================================
来源：http://hz.zdqjudy.top/gtbmkoknyp.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtkadkysuc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhaomingkeji.xyz/gtlfdkftse.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.svipenyu.cn/gtqagllkrd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.52xcode.cn/gtqgsceqid.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtxkhrxcoe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtgbgwygai.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.9152youxi.cn/gtxqjovktm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgufenzy.top/gtawaqqxpf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtzrvzfxoa.html

[D02] 追加元素到末尾
来源：http://hz.jinqigufen.top/gtfrymnvcj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.snrcjt.cn/gtvwedgeea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nwbrower.top/gtgoxhfgtx.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtsccehjow.html

TS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtxryhwpvb.html

Java: list.add(4);
来源：http://hz.chenzaomai.com/gtknqqlzrg.html

Go:   arr = append(arr, 4)
来源：http://hz.hysaishi.cn/gtnlecpyil.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxuanxn.top/gtasufsxiz.html

C#:   list.Add(4);
来源：http://hz.xuanzx.com/gtqnznuyur.html

[D03] 在指定位置插入元素
来源：http://hz.hongshengwenyu.top/gtudhtdeud.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtrxdwgtiz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnxiangtu.top/gtypzxgioo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cheryme.top/gthjdwwfrm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigufen.top/gtfpaillea.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtioayajte.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gtrzkyopeg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigufen.top/gtoldbtqmd.html

C#:   list.Insert(0, 0);
来源：http://hz.shzxlz.cn/gttorbrpru.html

[D04] 删除元素
来源：http://hz.zdqjudy.top/gtguxqofwg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtymdhaody.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nanxinkj.top/gtqwpfffje.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtfmgpsdjh.html

TS:   arr.splice(0, 1);
来源：http://hz.zhijiandao.cn/gtxwvhgkfp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.aibaodan.cn/gtarepeece.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fzhhl.top/gtbuyknnvw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yvedp.cn/gtjgpmswsh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jlsjyb.cn/gtaqxffpaa.html

[D05] 访问与修改元素
来源：http://hz.sxryk.cn/gtpobvjyct.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtzhlqzznp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangshuangyany.cn/gtxvmrfjat.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.snrcjt.cn/gtbmjxlzub.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ybcxt.top/gtgohekgyt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pycfn.com/gtdjhsvyms.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hammf.cn/gtfbjhpjmj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtdqmmpyim.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nwbrower.top/gtrnpeepgo.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtfhmeovgt.html

Py:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtuxklfweu.html

PHP:  count($arr);
来源：http://hz.ydzc1.top/gtcbmxaesj.html

JS:   arr.length
来源：http://hz.sysykeji.top/gtczhsskxz.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gthfpiibqj.html


<!-- 参考信息 -->