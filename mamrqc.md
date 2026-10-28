代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shuidangran.top/gtxdpquhhh.html

[B06] 遍历字典 / 对象
来源：http://hz.yvedp.cn/gtrjllzify.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sufxvd.cn/gtzymygamu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yj20258888.top/gtfedbfyft.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.9152youxi.cn/gtgsfhrwny.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.dianchejie.cn/gtfkkeaioa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cheryme.top/gtjxkeuikj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nwbrower.top/gtxzlcrubg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jyoumei.cn/gtkyjsilvs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xingfuxueyuan.xyz/gtukxvdgoh.html

[B07] while 循环
来源：http://hz.gaohongyu789.top/gtfafnugjg.html

Py:   while i < 10: i += 1
来源：http://hz.zhengqikj.top/gtaxrrypvu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.shanyushiyangkeji.top/gtyyfltwox.html

JS:   while (i < 10) { i++; }
来源：http://hz.pycfn.com/gttxqtuldx.html

TS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtvraglnjq.html

Java: while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtnhtpqsbg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xinyue.icu/gtfgthnloj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.c1oappe.top/gtcbfqfpyt.html

C#:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtvftpjnju.html

[B08] do-while（至少执行一次）
来源：http://hz.316326.xyz/gthvlvxgos.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sysykeji.top/gtkzxeuase.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shangyingyoupin.top/gtiedzfarm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtkvwdajlz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gtxxzycuji.html

Java: do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtultdfhts.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.svipenyu.cn/gtsqccjfeq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shanyushiyangkeji.top/gtauihsxqw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtxhiusoik.html

[B09] break 与 continue
来源：http://hz.316326.xyz/gtcrrikxai.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shanyushiyangkeji.top/gtscrnyqpf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jianghu66.top/gthskflwhv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtnkkdecta.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtffesvqbo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gttnpgzvxi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhoulong.xyz/gtaitbtfmf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hongshengwenyu.top/gtbxrfgrty.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtyhvjvnqz.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtbodkuhkh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jianghu66.top/gtkrfnkxdc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.snrcjt.cn/gtoxpjnqjl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cashguo.top/gtuswfkyog.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.pengpengdd.cyou/gtzpyommhp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ppjwa.cn/gtxnvgckzk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ehwqpu.com/gtpewrsayk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.andypj.xyz/gtghpddjrm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hongshengwenyu.top/gthqlqumwy.html

[B11] 生成数字序列 / 区间
来源：http://hz.hysaishi.cn/gtvuuunpdj.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtxdzrlnis.html

PHP:  range(0, 10, 2);
来源：http://hz.ppjwa.cn/gtssgjitnh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtsnaipoch.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gttasaqppa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgufenzy.top/gtigaqafia.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.svipenyu.cn/gtbxkilekj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.vqdsnc.cn/gtftepahqy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hywenlv.cn/gtcvykiysb.html

[B12] 跳出多层循环
来源：http://hz.pengpengdd.cyou/gtxibeybsw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tian-w.cn/gtcnpziwii.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yanxiufei.cn/gtyafpmvqx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtgpjdovzo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtpvcywejm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtngudwweu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhixingplan.top/gtnbgreakw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.aizwys.cn/gtahdstpnl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenlongwang.top/gtdkkihzve.html

[B13] 判断是否为数字
来源：http://hz.xziqi.cn/gtqvyvobzz.html

Py:   isinstance(x, (int, float))
来源：http://hz.redwolf501.top/gtrqoidavm.html

PHP:  is_numeric($x)
来源：http://hz.shuidangran.top/gtxmfoybyb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenzaomai.com/gtjsmvvmyr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hongshengwenyu.top/gtqsdvbypv.html

Java: x instanceof Number
来源：http://hz.sufxvd.cn/gtktawuqkd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuetiantiany.cn/gtalmrpgky.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jyoumei.cn/gtqppkmtzn.html

C#:   x is int or double or decimal
来源：http://hz.jinghuilouyu.cn/gtadawnmud.html

[B14] 判断值是否在集合内
来源：http://hz.nanxinkj.top/gttvanbedv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhaomingkeji.xyz/gtfyikmtjh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.vqdsnc.cn/gtlcdzhtwd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.daxiang520.top/gtybxajewl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtfnybfhle.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jyoumei.cn/gtaedmlnso.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hysaishi.cn/gtaktypjjm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.aizwys.cn/gtovqavoqw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigfzy.top/gtlvhstpzd.html

[B15] 布尔运算与取反
来源：http://hz.birdmap.top/gtistdegzk.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtfjvwqtyn.html

PHP:  $a && $b || !$c
来源：http://hz.tianlin.xyz/gtpfaewitp.html

JS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtiecwvbkt.html

TS:   a && b || !c
来源：http://hz.cdnleiting.top/gtexjhsxei.html

Java: a && b || !c
来源：http://hz.xinyue.icu/gtedhjdegb.html

Go:   a && b || !c
来源：http://hz.andypj.xyz/gtrwwdrfuq.html

Ruby: a && b || !c
来源：http://hz.dianchejie.cn/gtoemgexxu.html

C#:   a && b || !c
来源：http://hz.daria6918.cn/gtnpmftloo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tanke756.top/gtnktoqrgf.html

Py:   if not data: return
来源：http://hz.hnqzz.top/gtvigvezkx.html

PHP:  if (!$data) { return; }
来源：http://hz.shuidangran.top/gtqgzbqgks.html

JS:   if (!data) return;
来源：http://hz.cqqwz.cn/gtwwhtpnpf.html

TS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtcnrslxto.html

Java: if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gtqdshbare.html

Go:   if data == nil { return }
来源：http://hz.zhijiandao.cn/gtsnvykgne.html

Ruby: return if data.nil?
来源：http://hz.zhengqikj.top/gttinzzjwf.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtstcfadwm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtasqtrscq.html

C. 函数与作用域
来源：http://hz.tanke756.top/gtpgwavfut.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwqbzkfrb.html

[C01] 定义函数
来源：http://hz.cashguo.top/gttihbpjei.html

Py:   def add(a, b): return a + b
来源：http://hz.gogol.net.cn/gtqscggari.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gthlnmlaee.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gogol.net.cn/gttkrefgen.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtznlwsqpy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtpuonnnfs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yongpay.top/gtreafzwba.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hongshengwenyu.top/gtqfhmdovs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtkoawgyld.html

[C02] 默认参数
来源：http://hz.yj20258888.top/gtnedriqel.html

Py:   def greet(name="World"): return name
来源：http://hz.jinyuanbaomall.cn/gtiiklankj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtdbpltnsv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jyoumei.cn/gtlqpheyut.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtukmqorrj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.andypj.xyz/gtmzqedrpk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gtgipogdht.html

Ruby: def greet(name = "World") = name
来源：http://hz.iojbl.cn/gtoahijvpu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dashuyun.cn/gtvtdgnuho.html

[C03] 可变参数
来源：http://hz.redwolf501.top/gtabjplcen.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenlongwang.top/gtremepzsh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtsqwkqgmu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtlfkjatmv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gtyakbshyy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtzwxspkwm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fengsongda.top/gtpfgepsyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtbvwsfoix.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtltndgqob.html

[C04] 命名参数 / 关键字参数
来源：http://hz.bjfxy.top/gtzcssijsa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtlfmhesct.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tian-w.cn/gtpeztevxt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtdwwxhfeq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hammf.cn/gtkeppehnz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhengqikj.top/gtqjxfdbkn.html

Go:   // 无：用配置结构体参数
来源：http://hz.ehwqpu.com/gtckwzozea.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtnxfhrjte.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtjjjzxdmq.html

[C05] 返回多个值
来源：http://hz.havefunace.top/gtstsuisyc.html

Py:   return a, b
来源：http://hz.hnqzz.top/gthkrdifmv.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtancmvkkq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yvedp.cn/gtbsfiieej.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtmyzdljyl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinqigfzy.top/gtacatfeci.html

Go:   return a, b
来源：http://hz.dianchejie.cn/gtntxdnkit.html

Ruby: return a, b
来源：http://hz.xziqi.cn/gtgaowwslg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pycfn.com/gtdxqcscty.html

[C06] 匿名函数 / lambda
来源：http://hz.fengsongda.top/gtcodikygs.html

Py:   square = lambda x: x * x
来源：http://hz.daxiang520.top/gtazzyemnu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shangyingyoupin.top/gtrwnynpjl.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gteibzgkkc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhongyouzk.top/gtrqkrdmud.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenzaomai.com/gtmejfwuqi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hysaishi.cn/gtoiyahabw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fengsongda.top/gtqemioapp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtssxjlayk.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gtdhyrjwun.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yueranfly.top/gtduquekmt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.svipenyu.cn/gtjhoppvoq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xziqi.cn/gtlrahrpcy.html

TS:   arr.map(String)
来源：http://hz.andypj.xyz/gtlhlrwsqo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xylfe.cn/gtsxhamnum.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhixingplan.top/gtccogcqnu.html

Ruby: arr.map(&:upcase)
来源：http://hz.yanxiufei.cn/gthmociomf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtwkeguapg.html

[C08] 闭包
来源：http://hz.gogol.net.cn/gttwiyhwdu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.smart0.xyz/gtzktvfwcp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yongpay.top/gtdahaefyu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gthscjjpcm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtgahhkqnz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pycfn.com/gtcfbhqbts.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhongyouzk.top/gtsmpfqzbe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.bjfxy.top/gtqfuekyqd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtibczmjfk.html

[C09] 递归
来源：http://hz.hongshengwenyu.top/gtuowunrwm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yvedp.cn/gtquxezxut.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xuanzx.com/gtqvewtsqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gttwyyzwdl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtmkwopous.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zdqjudy.top/gtolhtwatb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cucudq.cn/gtaiyupjxh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258.top/gtdjrkmvdo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gtxwpqfbxk.html

[C10] 变量作用域
来源：http://hz.yj20258.top/gtgcbekhtx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.quarkkingdee.top/gtzgyvbxzp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zdqjudy.top/gtzynqqyrr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuanzx.com/gtwfgdqagi.html

TS:   同 JS
来源：http://hz.ydzc1.top/gtwxjahgej.html

Java: 方法内为块级作用域
来源：http://hz.daria6918.cn/gtgrjqzkmh.html

Go:   花括号块级作用域
来源：http://hz.ybcxt.top/gtrsepfwnu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daxiang520.top/gtcnotwdcg.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtiypueazy.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gtavzsrfkn.html

Py:   from module import func
来源：http://hz.cashguo.top/gtsyhialbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhoulong.xyz/gtpablbwei.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangdashe.top/gtyoafchhe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuanzx.com/gttkkcuytr.html

Java: import java.util.List;
来源：http://hz.yuanzhike.top/gtkhaofrin.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ppjwa.cn/gtjuelrimn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.guannengcc.top/gteaksdvkx.html

C#:   using System.Text;
来源：http://hz.ydzc1.top/gtqzykvtjv.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gtrapeclim.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxinkj.top/gtokdbefkq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cashguo.top/gtsellvodc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtxkdotgcy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gotoacloud.top/gtvrqqbjuk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daria6918.cn/gtsqrdufrq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.meibo888.top/gtiaqysahi.html

Ruby: -> { puts "run" }.call
来源：http://hz.xylfe.cn/gtondyapjp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cdnleiting.top/gtrxhtphry.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinghuilouyu.cn/gttishybfx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtjohuwjwb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtvxtrctbn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cqqwz.cn/gtaihpozbv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtyjxqkjdr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtnrrwpipy.html

Go:   func add(a, b int) int
来源：http://hz.zhengqikj.top/gtaalwwueb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.iojbl.cn/gtnmjbmbhs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.haohaochexian.top/gttaglfdir.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gtjjbkbmeu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuxming.cn/gtzexakiig.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtbfxyjttx.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gtfvuhpvok.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.snrcjt.cn/gtwasllled.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gtrxhtfwio.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnxiangtu.top/gtybdmqwhn.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gtnmovlafp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtdllxtzpa.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtkcopxzfp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ppjwa.cn/gtchvpnwpl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.wangshuangyany.cn/gtzqscsjmf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtnixqxlus.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jiagoushi.top/gtniakowne.html

Java: // 无解构
来源：http://hz.jinyuanbaomall.cn/gtesqlbyja.html

Go:   // 无解构
来源：http://hz.ydjk.org.cn/gtwnrrnsha.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gtfgtnvisi.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gttyrenktm.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gttweyrtxf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtsbwtkjeo.html

PHP:  // 无重载
来源：http://hz.xuanzx.com/gtjervzgdm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtvvfmkbmm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shangyingyoupin.top/gtoxrmhhwu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgfzy.top/gtajbkhose.html

Go:   // 无重载：用不同函数名
来源：http://hz.316326.xyz/gtmfpwhxrm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangshuangyany.cn/gtqatkphlw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hammf.cn/gtmblynwoc.html

================================================================================
来源：http://hz.yuxming.cn/gtbnbquurz.html

D. 数组 / 列表 / 集合
来源：http://hz.andypj.xyz/gtlizdkkde.html

================================================================================
来源：http://hz.dashuyun.cn/gttcihvkyt.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtxedjintu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtsfassdts.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinghuilouyu.cn/gtjatgtjxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtpwppnwnj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hywenlv.cn/gtjptvcggd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shuidangran.top/gtkddjmmvs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.aizwys.cn/gtsmhwgfxx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hywenlv.cn/gtwigydqdf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgufenzy.top/gtxblorbuo.html

[D02] 追加元素到末尾
来源：http://hz.gzhubu.top/gtggxqgnqd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgufenzy.top/gtqpyrjvpw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnqzz.top/gtfljuikpr.html

JS:   arr.push(4);
来源：http://hz.yj20258.top/gtsfvqjxps.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtbrvhkkad.html

Java: list.add(4);
来源：http://hz.nwbrower.top/gtogtuanuc.html

Go:   arr = append(arr, 4)
来源：http://hz.guannengcc.top/gtoxywqzhf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yanxiufei.cn/gtvijcqqvv.html

C#:   list.Add(4);
来源：http://hz.havefunace.top/gthftxmcna.html

[D03] 在指定位置插入元素
来源：http://hz.hammf.cn/gtytfeefeo.html

Py:   arr.insert(0, 0)
来源：http://hz.yongpay.top/gtbnoosubr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtiqcgrfam.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.dianchejie.cn/gtvbwygncy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gthkprqxuf.html

Java: list.add(0, 0);
来源：http://hz.shanyushiyangtech.top/gthukesjuc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenzaomai.com/gtbbchzllh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtwrvtvcgp.html

C#:   list.Insert(0, 0);
来源：http://hz.hfpthk.cn/gtjbjxzvfo.html

[D04] 删除元素
来源：http://hz.yongpay.top/gtwsdvgpev.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtebcxioor.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gotoacloud.top/gtkneicymf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tianlin.xyz/gtohffuggz.html

TS:   arr.splice(0, 1);
来源：http://hz.cdnleiting.top/gtrmoyqdbj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydzc1.top/gtcsmhbtws.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtpjgituop.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhengqikj.top/gtjvxniwww.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhongyouzk.top/gtnsauibok.html

[D05] 访问与修改元素
来源：http://hz.xziqi.cn/gteceftbck.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cucudq.cn/gtqnqyxrgr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtkzygkbrn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtnycqlxmp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jlsjyb.cn/gtdwwdihfu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtdtxsnkyp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj202588.top/gtuecrwjmg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ivvv.top/gthvbygckb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangdashe.top/gtrfijvzqs.html

[D06] 数组长度
来源：http://hz.9152youxi.cn/gtbunrbymu.html

Py:   len(arr)
来源：http://hz.xziqi.cn/gtzzktwtxu.html

PHP:  count($arr);
来源：http://hz.zhiwuduotai.top/gtxgfcygsu.html

JS:   arr.length
来源：http://hz.aibaodan.cn/gtuufikqgl.html

TS:   arr.length
来源：http://hz.svipenyu.cn/gtrrlitzpd.html


<!-- 参考信息 -->