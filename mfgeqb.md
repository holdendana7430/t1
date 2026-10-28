代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xuanzx.com/gtaomjkngy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.0kj1m.cn/gtiyovmifi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ydjk.org.cn/gtuttbwwox.html

Ruby: arr.each { |item| puts item }
来源：http://hz.wangshuangyany.cn/gtyniotoyg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hywenlv.cn/gtdctmgsgp.html

[B06] 遍历字典 / 对象
来源：http://hz.nanxuanxn.top/gtfckiqnqx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.0kj1m.cn/gtrjjgmmob.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.chenjidiqi.icu/gtjfhmwqrd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnqzz.top/gtvvluwmzr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tianlin.xyz/gtdxttqenr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jqgfzy.top/gtevufxxov.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.iojbl.cn/gtvclgmeql.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jyoumei.cn/gtldxfwdec.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hnxiangtu.top/gtwmavpzir.html

[B07] while 循环
来源：http://hz.jinqigfzy.top/gtjkdyafyw.html

Py:   while i < 10: i += 1
来源：http://hz.gaohongyu789.top/gtesborqsy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinyuanbaomall.cn/gtcjsajhgq.html

JS:   while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gtcaabwknf.html

TS:   while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtkxwhhpck.html

Java: while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtfgrxeogj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhijiandao.cn/gtfjvdeatl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258.top/gtpzlghqjd.html

C#:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtbxuiuutl.html

[B08] do-while（至少执行一次）
来源：http://hz.52xcode.cn/gtznasxwqv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.feifeiyinyue.top/gttdzidhff.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sufxvd.cn/gtvnxutwhm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gturgcsidl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtjwsughtn.html

Java: do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gthewkxday.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yvedp.cn/gtdaktgnku.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hammf.cn/gtfebmbhtp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtidpssvsh.html

[B09] break 与 continue
来源：http://hz.ivvv.top/gtgxirpmjz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xziqi.cn/gtyhlgljiq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jiagoushi.top/gtrpbbpdek.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtnmqzddnb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtoenuaezb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gteyrobapp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.quarkkingdee.top/gthgwnaeom.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jiagoushi.top/gtgnoqncfh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtzomxvcql.html

[B10] 遍历同时拿索引
来源：http://hz.wangshuangyany.cn/gtzuviqjkd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.pycfn.com/gtvmuisksu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.kuanghao11.cn/gtogdpxjav.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.9152youxi.cn/gtoxkyuupf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xylfe.cn/gthapfedkh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.smart0.xyz/gtddcgsgjd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jlsjyb.cn/gtemzypaeb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.quarkkingdee.top/gtmbzxjnag.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cashguo.top/gtitcizloi.html

[B11] 生成数字序列 / 区间
来源：http://hz.cqqwz.cn/gthliqsfgn.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258888.top/gthfwnuson.html

PHP:  range(0, 10, 2);
来源：http://hz.ppjwa.cn/gtfzewpcpg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yangfankeji.com/gtvihzrpha.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gthntscyaq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shanyushiyangkeji.top/gtgfulwxkq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hnqzz.top/gtbrpmlnbh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sufxvd.cn/gthzmjyefh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.birdmap.top/gticjgtgmo.html

[B12] 跳出多层循环
来源：http://hz.guannengcc.top/gtlmhucfnp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ydjk.org.cn/gtuhgtnxoj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.meibo888.top/gtvehsqfqv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtmnuzrijy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtnohfbqtx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gtkohnmumw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydjk.org.cn/gtclfmxjnp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dianchejie.cn/gtxgqeukjp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhongyouzk.top/gthiiimwap.html

[B13] 判断是否为数字
来源：http://hz.shangyingyoupin.top/gtiyqesgkb.html

Py:   isinstance(x, (int, float))
来源：http://hz.shzxlz.cn/gtcmuzeqqe.html

PHP:  is_numeric($x)
来源：http://hz.cucudq.cn/gtluriabuz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hongshengwenyu.top/gtdrrvebhm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yongpay.top/gtucqjzhkz.html

Java: x instanceof Number
来源：http://hz.jinqigfzy.top/gtzlnuvesq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shanyushiyangtech.top/gtzochnlnp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.birdmap.top/gthtjabtlw.html

C#:   x is int or double or decimal
来源：http://hz.andypj.xyz/gtqjcqewvd.html

[B14] 判断值是否在集合内
来源：http://hz.cheryme.top/gtsqybaifi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xingfuxueyuan.xyz/gtiditvckl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shzxlz.cn/gtzeosvakc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtfjvphlsu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.svipenyu.cn/gtdqfqfnxz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dashuyun.cn/gtwppvzbmy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zycfv.cn/gtvtmevfmj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ywan-chungtsiang.top/gtrkauqbzy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dashuyun.cn/gtjkovsmtb.html

[B15] 布尔运算与取反
来源：http://hz.yongpay.top/gthjlzpwam.html

Py:   a and b or not c
来源：http://hz.jinghuilouyu.cn/gtcxsxqshv.html

PHP:  $a && $b || !$c
来源：http://hz.nanxuanxn.top/gtjpneyfml.html

JS:   a && b || !c
来源：http://hz.zycfv.cn/gtfwyfsqcx.html

TS:   a && b || !c
来源：http://hz.yuanzhike.top/gtkgvnfhjw.html

Java: a && b || !c
来源：http://hz.hywenlv.cn/gtstrsrjrz.html

Go:   a && b || !c
来源：http://hz.sxryk.cn/gtalmgbugx.html

Ruby: a && b || !c
来源：http://hz.tanke756.top/gtmtenofae.html

C#:   a && b || !c
来源：http://hz.chenlongwang.top/gtdhyomfdv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ppjwa.cn/gtioqhurcz.html

Py:   if not data: return
来源：http://hz.meibo888.top/gtzzydzfqx.html

PHP:  if (!$data) { return; }
来源：http://hz.yonumen.top/gtgobgbefz.html

JS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtxpikjfor.html

TS:   if (!data) return;
来源：http://hz.zycfv.cn/gtcxdzrccq.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtlfucyumc.html

Go:   if data == nil { return }
来源：http://hz.nwbrower.top/gtjlloxeaz.html

Ruby: return if data.nil?
来源：http://hz.0kj1m.cn/gteppcgrjw.html

C#:   if (data == null) return;
来源：http://hz.tanke756.top/gthbmrobyu.html

================================================================================
来源：http://hz.316326.xyz/gtlfzwzrdh.html

C. 函数与作用域
来源：http://hz.vqdsnc.cn/gtwhjjsqnz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgtvdnfzx.html

[C01] 定义函数
来源：http://hz.aibaodan.cn/gtkckttuux.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxuanxn.top/gtvfguvfyp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtdyfmrtab.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigufen.top/gtwmchceep.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtxibqkvjq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtewzaflmi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.vqdsnc.cn/gtxvpnmamj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cheryme.top/gtnnvcqbfn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gttvlnikbw.html

[C02] 默认参数
来源：http://hz.gzhubu.top/gtnsquqzzs.html

Py:   def greet(name="World"): return name
来源：http://hz.daria6918.cn/gtktijhuim.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sweek.top/gteqfjxkyr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gtofjdrbbl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.kuanghao11.cn/gtattucdyu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhoulong.xyz/gtsaiidvxm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guowangkeji.top/gtkrakkydy.html

Ruby: def greet(name = "World") = name
来源：http://hz.gotoacloud.top/gtprhaznpm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xingfuxueyuan.xyz/gtdqewvcko.html

[C03] 可变参数
来源：http://hz.smart0.xyz/gthlwrcvpg.html

Py:   def total(*args): return sum(args)
来源：http://hz.xziqi.cn/gtjetikkwg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hywenlv.cn/gtfrgoepyk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtdehxzqjx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gttzwyhswe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtrktxxsqv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258888.top/gttlmnuzvo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yanxiufei.cn/gtismatsco.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgufenzy.top/gtbbeokmox.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtucurnifc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hammf.cn/gtlepfgkaz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtfxyewial.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.meibo888.top/gtebwkuzme.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gogol.net.cn/gtnymkjxnd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jlsjyb.cn/gtaxhqdyou.html

Go:   // 无：用配置结构体参数
来源：http://hz.c1oappe.top/gtyysjqcnt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtjwmgqniv.html

C#:   f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtdxtidqkt.html

[C05] 返回多个值
来源：http://hz.birdmap.top/gtrcupiymm.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gttmefdscz.html

PHP:  return [$a, $b];
来源：http://hz.aibaodan.cn/gtkbkaornj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gtwrjoyoak.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtethfokrt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.birdmap.top/gtgeubxoch.html

Go:   return a, b
来源：http://hz.jianghu66.top/gtpvrcqwpq.html

Ruby: return a, b
来源：http://hz.hnxiangtu.top/gtgkcuryil.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xziqi.cn/gtszrwjjql.html

[C06] 匿名函数 / lambda
来源：http://hz.yongpay.top/gtrhfkieiy.html

Py:   square = lambda x: x * x
来源：http://hz.zhengqikj.top/gtxkwznoqw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.smart0.xyz/gtjlhxgbom.html

JS:   const square = x => x * x;
来源：http://hz.shzxlz.cn/gttnrlvjim.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gtesucjlgq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.havefunace.top/gtivtjpywt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hfpthk.cn/gtxgsbvvfv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gtlphxyche.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtuanhpynm.html

[C07] 把函数作为参数传入
来源：http://hz.mhx1999.top/gtuwxjqzkm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.mhx1999.top/gtubgjnlzo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.daxiang520.top/gtdvmgzfqr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtzapegpiq.html

TS:   arr.map(String)
来源：http://hz.zycfv.cn/gtuuaxuxam.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yanxiufei.cn/gtakddfhbc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shzxlz.cn/gtavftkgbb.html

Ruby: arr.map(&:upcase)
来源：http://hz.jqgfzy.top/gtaegelafq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xylfe.cn/gtgkxlxzon.html

[C08] 闭包
来源：http://hz.iojbl.cn/gtlsjmcqxx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yongpay.top/gtpnlcqlxg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.feifeiyinyue.top/gtnfofocuw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtmnsyzxdx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtpycwkojz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.mhx1999.top/gtifwkgesv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258888.top/gtodmzzump.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shuidangran.top/gtvleqeqnw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtqlhgnank.html

[C09] 递归
来源：http://hz.sysykeji.top/gtxfaqfhhf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtszequexq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgfzy.top/gtsufsrhhf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtkygqlkno.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtuzrwmttj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hywenlv.cn/gtzaponnyl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtlqfcdvsl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtklssgbtn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cqqwz.cn/gtspzwwpae.html

[C10] 变量作用域
来源：http://hz.ivvv.top/gtyioyxyby.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhaomingkeji.xyz/gtbprjtpvn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shangyingyoupin.top/gtwhzqlnko.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gthhxmqnnr.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtikuhunhz.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gtjaogbhib.html

Go:   花括号块级作用域
来源：http://hz.ydzc1.top/gtbqfyrbpa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jiagoushi.top/gtpidtjmtl.html

C#:   块级作用域
来源：http://hz.fzhhl.top/gtuiuzllhp.html

[C11] 模块导入与导出
来源：http://hz.nwbrower.top/gtmprhpoue.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gtumleannq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtrrhnfjes.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tanke756.top/gtkgbxqlip.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtneyujifi.html

Java: import java.util.List;
来源：http://hz.pengpengdd.cyou/gtryypbkxg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtfiyuqdeu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtmbuigbaj.html

C#:   using System.Text;
来源：http://hz.smart0.xyz/gtsjittqeg.html

[C12] 立即执行函数 IIFE
来源：http://hz.shuidangran.top/gtcacbboey.html

Py:   (lambda: print("run"))()
来源：http://hz.tian-w.cn/gtfoejbjjj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtdkchbvxs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinyuanbaomall.cn/gtezrzmpnp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtcklecwsf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtgthifryd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guowangkeji.top/gtfnnwfoug.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtrqtalulb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhaomingkeji.xyz/gtcauqdecz.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gtxcdxpeod.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtrcyojqvd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtndiogdqu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sxryk.cn/gtpckhfnjw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtaodprtou.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtndjdkpjv.html

Go:   func add(a, b int) int
来源：http://hz.zycfv.cn/gtpzezuqke.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tianlin.xyz/gtuipamzeq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhixingplan.top/gtxzxuyrsi.html

[C14] 泛型函数
来源：http://hz.meibo888.top/gtxrfpvsfg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtlvyoczoz.html

PHP:  // 无泛型
来源：http://hz.gzhubu.top/gtmceeqthk.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gtvsbbymny.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.snrcjt.cn/gtixuzgswp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hysaishi.cn/gtunxikwzv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ybcxt.top/gtekqhutlo.html

Ruby: # 无泛型
来源：http://hz.jinqigufen.top/gtuadmcnto.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.316326.xyz/gthlqgntpt.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gtviclbmea.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenzaomai.com/gtrayfecat.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gthwbfesxa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtmbgnxtmm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.smart0.xyz/gtqmkkdneb.html

Java: // 无解构
来源：http://hz.yanxiufei.cn/gtwwfnzdzz.html

Go:   // 无解构
来源：http://hz.tian-w.cn/gtwvtrhbvu.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtoahstizr.html

C#:   var (a, b) = pair;
来源：http://hz.jiagoushi.top/gtdmizyyed.html

[C16] 函数 / 方法重载
来源：http://hz.andypj.xyz/gtnzwhahxl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zdqjudy.top/gtyyavjjpx.html

PHP:  // 无重载
来源：http://hz.nanxinkj.top/gtwcducviu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.haohaochexian.top/gtegcdtnsq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxinkj.top/gtopmlcgqx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.316326.xyz/gtdvfuexbd.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydjk.org.cn/gtyiclqdxd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtnqplpzjj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yueranfly.top/gtczrybhqa.html

================================================================================
来源：http://hz.xuanzx.com/gtiytzfjbb.html

D. 数组 / 列表 / 集合
来源：http://hz.hysaishi.cn/gthglchilu.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtainxjqmb.html

[D01] 创建数组 / 列表
来源：http://hz.yongpay.top/gttpnlufuf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gtwclivdvt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtyiyyfvao.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtriowkwkq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenlongwang.top/gtbfdotwtj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.meibo888.top/gtdsmvjidq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dashuyun.cn/gtxqixzcqi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtmxkgkspx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.9152youxi.cn/gtgonjkxqv.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gtkfrceors.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydjk.org.cn/gtguwabpzl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nwbrower.top/gtudqkeppn.html

JS:   arr.push(4);
来源：http://hz.gogol.net.cn/gttyrzfdbm.html

TS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtdgpijpfg.html

Java: list.add(4);
来源：http://hz.jinghuilouyu.cn/gtpmjdyhbo.html

Go:   arr = append(arr, 4)
来源：http://hz.hongshengwenyu.top/gtzfzefwkc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gthcompgqk.html

C#:   list.Add(4);
来源：http://hz.zhixingplan.top/gtoohkfzkf.html

[D03] 在指定位置插入元素
来源：http://hz.0kj1m.cn/gtoeicwhvl.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtrsrvwosz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nanxuanxn.top/gtlfoqpcry.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xinyue.icu/gtstmbkwhs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhengqikj.top/gtyjealajt.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtwrzaqbmh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.9152youxi.cn/gtdrkidujv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtmeixmyuo.html

C#:   list.Insert(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtbzzkjxty.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtuhnoakmw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtvfypwxlz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtrjgbzfns.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtlvamuqsa.html

TS:   arr.splice(0, 1);
来源：http://hz.vqdsnc.cn/gtzenrnplz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtmsnblvql.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtwcuklgbk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhixingplan.top/gtzystaltm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtkdlmpiul.html

[D05] 访问与修改元素
来源：http://hz.yanxiufei.cn/gtpcbdeoxd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtdjjblqyn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258.top/gteqdxkxfi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhixingplan.top/gtgwrsgrmn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtllojxlpu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtcylarhsq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gteyyiuvsx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtpkgnjrdg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtccblefep.html

[D06] 数组长度
来源：http://hz.hnqzz.top/gtnpqliwru.html


<!-- 参考信息 -->