代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhijiandao.cn/gtvoxijncc.html

[B06] 遍历字典 / 对象
来源：http://hz.ydjk.org.cn/gttjqfyjeh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.gzhubu.top/gtokrrojfv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sufxvd.cn/gtrnjcfbej.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuanzhike.top/gtfjfeyynl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gthlcwglda.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zdqjudy.top/gtprsnxzwq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jqgfzy.top/gtbdmuojnf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gzhubu.top/gtzvfqhkvq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.haohaochexian.top/gtjnyjaztq.html

[B07] while 循环
来源：http://hz.snrcjt.cn/gtvzifeurz.html

Py:   while i < 10: i += 1
来源：http://hz.kuanghao11.cn/gtzlkohgbx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.0kj1m.cn/gtpgrsxkwh.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtnboyniow.html

TS:   while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gtkqarfyqo.html

Java: while (i < 10) { i++; }
来源：http://hz.yvedp.cn/gttbjnpigm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinghuilouyu.cn/gtsmyejmfe.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shuidangran.top/gtvjestwzd.html

C#:   while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtjoytgeyc.html

[B08] do-while（至少执行一次）
来源：http://hz.shanyushiyangkeji.top/gtmcgkyqfq.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.meibo888.top/gtwcejzfnx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.tian-w.cn/gtxcizkxbk.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtqricisrx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gttxcsiiko.html

Java: do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gthrthrvur.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xingfuxueyuan.xyz/gtnuelwnvq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jianghu66.top/gtjgkblkis.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtmsxhzcuh.html

[B09] break 与 continue
来源：http://hz.hongshengwenyu.top/gtblvpkkus.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cucudq.cn/gtwvqvjzlr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cqqwz.cn/gtjmmcuhwc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtyardibay.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gtaclefsvn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtdxkembqt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yueranfly.top/gtqvpfvddy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nanxinkj.top/gtxdtqnjos.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtbiuyurnx.html

[B10] 遍历同时拿索引
来源：http://hz.dashuyun.cn/gtonqoshrv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gogol.net.cn/gtrzgfrkcm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xinyue.icu/gtryivujbc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yonumen.top/gtllljkvvr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnxiangtu.top/gtimcnofri.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shzxlz.cn/gthhhaubxs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ydjk.org.cn/gtgfwcjkzk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.bjfxy.top/gtrabejzjw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.haohaochexian.top/gtfuakfpwq.html

[B11] 生成数字序列 / 区间
来源：http://hz.gotoacloud.top/gtclhzmnpz.html

Py:   list(range(0, 10, 2))
来源：http://hz.zycfv.cn/gtwhmrqpbo.html

PHP:  range(0, 10, 2);
来源：http://hz.yuanzhike.top/gtjpzuecks.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yueranfly.top/gtjoyfujir.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gtkfpdtnoe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.vqdsnc.cn/gtatytwqwt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.chenzaomai.com/gtmcilhepe.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtreycckra.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yonumen.top/gtdqyumnda.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangkeji.top/gtiezcpmoq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jyoumei.cn/gtfrmluulr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuxming.cn/gtsqqxiatl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtvfficenk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtqposbrwk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtkdckljdm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhongyouzk.top/gtwxvpxaim.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hongshengwenyu.top/gtquvtnfci.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shangyingyoupin.top/gtpqrrjxiz.html

[B13] 判断是否为数字
来源：http://hz.9152youxi.cn/gtiizgqtyp.html

Py:   isinstance(x, (int, float))
来源：http://hz.sufxvd.cn/gtquwteiut.html

PHP:  is_numeric($x)
来源：http://hz.ppjwa.cn/gtzdxmjfvo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zycfv.cn/gtxxeivexk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtdlttsqsh.html

Java: x instanceof Number
来源：http://hz.xylfe.cn/gtleihhvqh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hywenlv.cn/gttueoywrc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gogol.net.cn/gtytenoevi.html

C#:   x is int or double or decimal
来源：http://hz.zhaomingkeji.xyz/gtfypoeksp.html

[B14] 判断值是否在集合内
来源：http://hz.tian-w.cn/gthynjumvf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shangyingyoupin.top/gtpdvvyqfq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shanyushiyangkeji.top/gtkiuzaomr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtwielrqur.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtbsnqoheq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dianchejie.cn/gtpvehdjiy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jqgfzy.top/gtpdtheegu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258888.top/gtqospeoua.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigufen.top/gtsbomyklo.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gtmrwlxarr.html

Py:   a and b or not c
来源：http://hz.daria6918.cn/gtafifxbyi.html

PHP:  $a && $b || !$c
来源：http://hz.zhoulong.xyz/gtfutbcclk.html

JS:   a && b || !c
来源：http://hz.yvedp.cn/gtwjgbhwhr.html

TS:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtnyqfmkpm.html

Java: a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtzujywgrz.html

Go:   a && b || !c
来源：http://hz.dianchejie.cn/gtqvcyzqlh.html

Ruby: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtofaoklvf.html

C#:   a && b || !c
来源：http://hz.tianlin.xyz/gtfqmxdory.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nanxuanxn.top/gtcffokuwx.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtxcskoscg.html

PHP:  if (!$data) { return; }
来源：http://hz.hongshengwenyu.top/gtyenzfnkt.html

JS:   if (!data) return;
来源：http://hz.hnqzz.top/gtnohqyhsg.html

TS:   if (!data) return;
来源：http://hz.tian-w.cn/gtfjqjfcsk.html

Java: if (data == null) return;
来源：http://hz.aibaodan.cn/gtxftnapxp.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtovdpsneb.html

Ruby: return if data.nil?
来源：http://hz.jqgfzy.top/gtqoqlhasc.html

C#:   if (data == null) return;
来源：http://hz.jqgufenzy.top/gtqbrvckey.html

================================================================================
来源：http://hz.jqgfzy.top/gtcdiwigaj.html

C. 函数与作用域
来源：http://hz.aibaodan.cn/gtuzgmpnaw.html

================================================================================
来源：http://hz.daria6918.cn/gtthgovkwp.html

[C01] 定义函数
来源：http://hz.zycfv.cn/gttwkrbswi.html

Py:   def add(a, b): return a + b
来源：http://hz.shuidangran.top/gtftpbvgzs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtrctekscg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hfpthk.cn/gtvzvntqqr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtqqqrgdmh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gthbzwvnmy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.andypj.xyz/gtoqbzqytf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yanxiufei.cn/gtsfsoyswu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gttfcjyrcz.html

[C02] 默认参数
来源：http://hz.guowangkeji.top/gtuczmkqoa.html

Py:   def greet(name="World"): return name
来源：http://hz.ydjk.org.cn/gtjrfjiixp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aizwys.cn/gtebpgyfzg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtylxtlnkh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtkaekdiru.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxinkj.top/gtjiqrziij.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgufenzy.top/gtfdsdjsyv.html

Ruby: def greet(name = "World") = name
来源：http://hz.hysaishi.cn/gtkwsdytpi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hammf.cn/gtxbiwojgw.html

[C03] 可变参数
来源：http://hz.xuetiantiany.cn/gtqulpcbsv.html

Py:   def total(*args): return sum(args)
来源：http://hz.hammf.cn/gtzhxqhoqt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cqqwz.cn/gtiufceyft.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtilcrbang.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtedljjubu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtkioriksf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.mhx1999.top/gtineuzazj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258.top/gtymsvhoby.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yuanzhike.top/gtqrelnysl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gttzqsuwiu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhengqikj.top/gtglfitvvu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ywan-chungtsiang.top/gtimzkvxhv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtenwdhawi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuetiantiany.cn/gtvbfgzjop.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gzhubu.top/gtcubhojnt.html

Go:   // 无：用配置结构体参数
来源：http://hz.kuanghao11.cn/gtnoepyzdd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gthfrlqshb.html

C#:   f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtzlfraytp.html

[C05] 返回多个值
来源：http://hz.ydjk.org.cn/gtepxzirti.html

Py:   return a, b
来源：http://hz.nanxinkj.top/gtchlbfnit.html

PHP:  return [$a, $b];
来源：http://hz.cucudq.cn/gtdyeakgea.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtqvxndcsm.html

TS:   return { a, b };
来源：http://hz.hammf.cn/gtkzlmoouv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jqgfzy.top/gtiobicxak.html

Go:   return a, b
来源：http://hz.316326.xyz/gtmpvxovpp.html

Ruby: return a, b
来源：http://hz.jqgfzy.top/gtrvuluouj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ywan-chungtsiang.top/gtupuydmnc.html

[C06] 匿名函数 / lambda
来源：http://hz.jiagoushi.top/gtiyhevrwl.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gtrzgzuqkm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dashuyun.cn/gtjwazifal.html

JS:   const square = x => x * x;
来源：http://hz.hnqzz.top/gtesdanyxp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ywan-chungtsiang.top/gtjggtbhve.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.svipenyu.cn/gtxzyeliph.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fzhhl.top/gtywxydoeg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sxryk.cn/gtdnlgdiah.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yangfankeji.com/gtrlglxqyc.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigfzy.top/gtadurjkkr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xziqi.cn/gtxnckxvdg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangtech.top/gtxmyviyln.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cqqwz.cn/gtvrhlrsfz.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gtrltdjqkp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnqzz.top/gtntalylsd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhoulong.xyz/gttfsnrdly.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtecbvhjlg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fzhhl.top/gtpohayvcz.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtpvrgvfnw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guannengcc.top/gtzzbnntyq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cdnleiting.top/gtfjrbzjdq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtvfvzlnxv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtbgaxwtvi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxinkj.top/gtqoufqyxl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtjlnpzawi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxinkj.top/gtliddrzmd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gtbnwduvvg.html

[C09] 递归
来源：http://hz.xuanzx.com/gtepwxrwtb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtrmndiiyf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj20258.top/gtzsrccwvi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtfqbbmdjx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtbbovjxpc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgfzy.top/gtivftxruj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.wangshuangyany.cn/gtzlvgufjl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cqqwz.cn/gthiqztsup.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cucudq.cn/gtsjoxpuja.html

[C10] 变量作用域
来源：http://hz.gzhubu.top/gtiffppkca.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cheryme.top/gtxzxnubql.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtkcxmnvoj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jianghu66.top/gtlnorbmmh.html

TS:   同 JS
来源：http://hz.havefunace.top/gtupgnwzfh.html

Java: 方法内为块级作用域
来源：http://hz.nwbrower.top/gtclyjxfxu.html

Go:   花括号块级作用域
来源：http://hz.zhengqikj.top/gtvcwthnzk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtskysptqt.html

C#:   块级作用域
来源：http://hz.kuanghao11.cn/gtwcqboocz.html

[C11] 模块导入与导出
来源：http://hz.hfpthk.cn/gtublbeqgl.html

Py:   from module import func
来源：http://hz.cucudq.cn/gtfqjjxsaq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shanyushiyangkeji.top/gtjcvsvxfi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dashuyun.cn/gtizparibb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtugeaiudc.html

Java: import java.util.List;
来源：http://hz.shangyingyoupin.top/gtwvypdumq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenjidiqi.icu/gtbkgtuexg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenlongwang.top/gtsvruzuxh.html

C#:   using System.Text;
来源：http://hz.tianlin.xyz/gtxghdqobs.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydjk.org.cn/gtgntdliaf.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtestpszzw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guowangkeji.top/gtmgwhpgvn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtvkfhhsul.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtsqlcmxut.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.meibo888.top/gtvkkxpeww.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhijiandao.cn/gtciubufry.html

Ruby: -> { puts "run" }.call
来源：http://hz.yonumen.top/gtqdanfcaa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.316326.xyz/gtgprfitln.html

[C13] 类型声明 / 类型注解
来源：http://hz.fzhhl.top/gtfyqjvouo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shangyingyoupin.top/gtycnupbmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gttpcdyghh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtgdlzzujv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtcuxfesav.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtdcqzduzg.html

Go:   func add(a, b int) int
来源：http://hz.hammf.cn/gtrqupjvgv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtttfbsnop.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gotoacloud.top/gtjcuisoaj.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtrrkzlsfn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtnmouiant.html

PHP:  // 无泛型
来源：http://hz.haohaochexian.top/gtgdwxnbbr.html

JS:   // 无泛型
来源：http://hz.yueranfly.top/gtbminlndt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtgjuppsym.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pengpengdd.cyou/gtnsagfgyb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gtlmlwrvws.html

Ruby: # 无泛型
来源：http://hz.havefunace.top/gtmtobcgff.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtwwtizryi.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtoszifyzj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yongpay.top/gtxieujfwg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhiwuduotai.top/gtyzbqqbqm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hammf.cn/gtijqampkn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtwgoqjehc.html

Java: // 无解构
来源：http://hz.tanke756.top/gtdcjtxygd.html

Go:   // 无解构
来源：http://hz.zhoulong.xyz/gtqvycgjng.html

Ruby: a, b = pair
来源：http://hz.zhengqikj.top/gtmejkcmci.html

C#:   var (a, b) = pair;
来源：http://hz.snrcjt.cn/gtmsnofcfw.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gtqehfyvgj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.andypj.xyz/gtonmsoiou.html

PHP:  // 无重载
来源：http://hz.ppjwa.cn/gtshrszphb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shzxlz.cn/gtfbhpfcdu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangdashe.top/gtqpirscec.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.haohaochexian.top/gtyazyuykv.html

Go:   // 无重载：用不同函数名
来源：http://hz.haohaochexian.top/gthealhyph.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtpsywzsed.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhongyouzk.top/gtkszndnvi.html

================================================================================
来源：http://hz.316326.xyz/gtzofdmbsi.html

D. 数组 / 列表 / 集合
来源：http://hz.cheryme.top/gtyfxcezze.html

================================================================================
来源：http://hz.gotoacloud.top/gtpxkrishy.html

[D01] 创建数组 / 列表
来源：http://hz.cqqwz.cn/gtyngeeziw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtmgljnkch.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dashuyun.cn/gtjdslbbds.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtjiestztv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtusmihdht.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.iojbl.cn/gtrgkuusgi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gotoacloud.top/gttvxhzpad.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxuanxn.top/gtykwoqsof.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtfincnkjb.html

[D02] 追加元素到末尾
来源：http://hz.zhixingplan.top/gtbramemkq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenzaomai.com/gtnvxkfgrf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jlsjyb.cn/gtwqsjrfxl.html

JS:   arr.push(4);
来源：http://hz.zycfv.cn/gtrgjgcaxa.html

TS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtqvdavnub.html

Java: list.add(4);
来源：http://hz.dianchejie.cn/gtmqggbidr.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gtpptmgrfj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinghuilouyu.cn/gtohqkxtox.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gtemvdqhqc.html

[D03] 在指定位置插入元素
来源：http://hz.svipenyu.cn/gtxxopphra.html

Py:   arr.insert(0, 0)
来源：http://hz.cheryme.top/gtmxyhaqjn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigufen.top/gtdtuiydhm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hongshengwenyu.top/gthnrutfhd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.dianchejie.cn/gtvpmkuihv.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtmrtxfhub.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtlqdttrwl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cheryme.top/gtfvbzrqws.html

C#:   list.Insert(0, 0);
来源：http://hz.ivvv.top/gtoxspdotc.html

[D04] 删除元素
来源：http://hz.yueranfly.top/gtacqlxrbf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtcvtqvsbs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.quarkkingdee.top/gtwxmateke.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gtdauzcyyl.html

TS:   arr.splice(0, 1);
来源：http://hz.xylfe.cn/gtcwboukuj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigufen.top/gtajizhptp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gtixamjczo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.smart0.xyz/gtakqxusnc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.iojbl.cn/gteglftdpk.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtlecpypqh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtflapmamq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yvedp.cn/gtclfpdvsf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.quarkkingdee.top/gteaxhghub.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.haohaochexian.top/gttxciybjr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.smart0.xyz/gteazjgfua.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daria6918.cn/gtgjdbljhy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtviuamjlh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cheryme.top/gtsqyinwoz.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtpvmhebiw.html

Py:   len(arr)
来源：http://hz.svipenyu.cn/gthesuwmsm.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtomysckyq.html

JS:   arr.length
来源：http://hz.mhx1999.top/gtqxyfhbpz.html

TS:   arr.length
来源：http://hz.9152youxi.cn/gtbcrelhjn.html


<!-- 参考信息 -->