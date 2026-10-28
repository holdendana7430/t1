代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hysaishi.cn/gtajaziqxw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xziqi.cn/gtfmrvvjal.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tian-w.cn/gtbyfqfqmc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xziqi.cn/gtxdyjmsly.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xylfe.cn/gtjtxzcloy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gaohongyu789.top/gtqykddnpt.html

[B07] while 循环
来源：http://hz.0kj1m.cn/gtynzufuav.html

Py:   while i < 10: i += 1
来源：http://hz.ydzc1.top/gtyuifhfba.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.guannengcc.top/gtksrwmcgi.html

JS:   while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtsatgwiuu.html

TS:   while (i < 10) { i++; }
来源：http://hz.sweek.top/gtssnujvjh.html

Java: while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtigjbhmbc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.quarkkingdee.top/gtmbgtybvz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xylfe.cn/gtdgiwiffg.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtpaisvxlp.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258.top/gthpieruzy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.bjfxy.top/gtbivahqam.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hammf.cn/gtgnomuulk.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gtmxlhvnsj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gttznfsvrc.html

Java: do { i++; } while (i < 10);
来源：http://hz.yongpay.top/gteycvivzd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.snrcjt.cn/gthbxfqxcr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xuetiantiany.cn/gtnxynalom.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtgajsmwhq.html

[B09] break 与 continue
来源：http://hz.9152youxi.cn/gtfujjwilp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xinyue.icu/gtwpxkslxa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.daxiang520.top/gtentelden.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtzjvskzhm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtbaahikmb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtdwatfohk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xziqi.cn/gtwrliwccn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nwbrower.top/gtcdogjsfl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtxawnsdlx.html

[B10] 遍历同时拿索引
来源：http://hz.9152youxi.cn/gtwslibozd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenlongwang.top/gtrubqivds.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sufxvd.cn/gtqxzokldr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtrqqkdnoj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gticdgjsno.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yj202588.top/gttmsonvpb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhiwuduotai.top/gtrebopcji.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhongyouzk.top/gtiibnnkor.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sxryk.cn/gthqktmofk.html

[B11] 生成数字序列 / 区间
来源：http://hz.sxryk.cn/gtofsguhyh.html

Py:   list(range(0, 10, 2))
来源：http://hz.mhx1999.top/gtelmznurn.html

PHP:  range(0, 10, 2);
来源：http://hz.feifeiyinyue.top/gteaouonup.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.bjfxy.top/gtbcrmrefx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtkgpzlcdt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangshuangyany.cn/gtuvjrhdae.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gttevlrheh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gtniaphdei.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hywenlv.cn/gtnjnnobpj.html

[B12] 跳出多层循环
来源：http://hz.jinqigfzy.top/gtlvethkwk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.c1oappe.top/gtoshpwxyl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hongshengwenyu.top/gtjeoqpthh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtnfvpjgoe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtchwfnzdq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtgelrnvqz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.haohaochexian.top/gtcfvdkqpc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.snrcjt.cn/gtkqhuzfcx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.kuanghao11.cn/gthewsxxqy.html

[B13] 判断是否为数字
来源：http://hz.shuidangran.top/gtqyfxechg.html

Py:   isinstance(x, (int, float))
来源：http://hz.xinyue.icu/gtciobtyjf.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtvxghugmy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yuxming.cn/gtuufyiwgd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.kuanghao11.cn/gtfwbvpjlk.html

Java: x instanceof Number
来源：http://hz.andypj.xyz/gtiesurubq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.52xcode.cn/gtsycyalki.html

Ruby: x.is_a?(Numeric)
来源：http://hz.aizwys.cn/gtxdjoqggs.html

C#:   x is int or double or decimal
来源：http://hz.yueranfly.top/gtvttoxlpw.html

[B14] 判断值是否在集合内
来源：http://hz.pengpengdd.cyou/gtgidzjdhh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yueranfly.top/gtyfjqzqux.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.svipenyu.cn/gtrjtdbkdu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtwqoarjky.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gttmjdgerr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.feifeiyinyue.top/gtziywdjqp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nwbrower.top/gtxpeuowtm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.9152youxi.cn/gtijplwawv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.daria6918.cn/gtncixhcwc.html

[B15] 布尔运算与取反
来源：http://hz.nanxuanxn.top/gteagefzay.html

Py:   a and b or not c
来源：http://hz.jqgufenzy.top/gtkicedlsj.html

PHP:  $a && $b || !$c
来源：http://hz.shanyushiyangkeji.top/gtstakbtsx.html

JS:   a && b || !c
来源：http://hz.chenzaomai.com/gtuvdliqmz.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtkdwqzwxd.html

Java: a && b || !c
来源：http://hz.zhoulong.xyz/gtewvldnzw.html

Go:   a && b || !c
来源：http://hz.jiagoushi.top/gtdkpukvuk.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtqnbvjfbt.html

C#:   a && b || !c
来源：http://hz.dianchejie.cn/gtbmnszaox.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jyoumei.cn/gtcjzfxqxo.html

Py:   if not data: return
来源：http://hz.shzxlz.cn/gtnzdzwxas.html

PHP:  if (!$data) { return; }
来源：http://hz.yj202588.top/gtazjpmucs.html

JS:   if (!data) return;
来源：http://hz.cucudq.cn/gtivdudxed.html

TS:   if (!data) return;
来源：http://hz.ppjwa.cn/gtavuvhpqo.html

Java: if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtomckoahh.html

Go:   if data == nil { return }
来源：http://hz.chenjidiqi.icu/gtdjycqlwb.html

Ruby: return if data.nil?
来源：http://hz.daria6918.cn/gtatlhdyjv.html

C#:   if (data == null) return;
来源：http://hz.0kj1m.cn/gtusqdfjvf.html

================================================================================
来源：http://hz.yongpay.top/gtwuhlevmx.html

C. 函数与作用域
来源：http://hz.tanke756.top/gtwblprqmk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpujnmbhk.html

[C01] 定义函数
来源：http://hz.jiagoushi.top/gtzzovimed.html

Py:   def add(a, b): return a + b
来源：http://hz.gzhubu.top/gteglzvasv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gttwdlgokg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtoqghyepx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtkoccbgcw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gthvsoobub.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cqqwz.cn/gtchrdawbj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shzxlz.cn/gtqabcbugg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtdszkdkbj.html

[C02] 默认参数
来源：http://hz.mhx1999.top/gtlbquuuus.html

Py:   def greet(name="World"): return name
来源：http://hz.xziqi.cn/gtxxijioxb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cdnleiting.top/gtxlmbmmon.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtkgdkgqne.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hysaishi.cn/gtwvqjtqqr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtlpjosubb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj20258888.top/gtdcdbvxvk.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gtykwxgjiz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenjidiqi.icu/gtdtswrhex.html

[C03] 可变参数
来源：http://hz.dashuyun.cn/gtlzievxcd.html

Py:   def total(*args): return sum(args)
来源：http://hz.ivvv.top/gtgnamirst.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aibaodan.cn/gtbuelccev.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.bjfxy.top/gtpkupygwz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gogol.net.cn/gtlkgjoepg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.wangdashe.top/gtpewlmhoe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtgilgbkut.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yonumen.top/gtqxjajazd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gttbxwxyku.html

[C04] 命名参数 / 关键字参数
来源：http://hz.quarkkingdee.top/gtinrgmqbh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.meibo888.top/gtwmmrzxnr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tanke756.top/gtljnwvahv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtlogdwwvd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenlongwang.top/gtmjovfuhc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.feifeiyinyue.top/gtchfrlgna.html

Go:   // 无：用配置结构体参数
来源：http://hz.gogol.net.cn/gtmghgnncw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtsbodcnbp.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtkelzadlb.html

[C05] 返回多个值
来源：http://hz.feifeiyinyue.top/gtftkhewda.html

Py:   return a, b
来源：http://hz.yongpay.top/gtumcnmosb.html

PHP:  return [$a, $b];
来源：http://hz.svipenyu.cn/gtsexdbgyn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cucudq.cn/gtctuglggc.html

TS:   return { a, b };
来源：http://hz.gogol.net.cn/gtntwbirrk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gtssrdndld.html

Go:   return a, b
来源：http://hz.hnqzz.top/gtydmtrwmr.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtyrcetrhz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj202588.top/gtuzgpbanw.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigufen.top/gtruvkmpfd.html

Py:   square = lambda x: x * x
来源：http://hz.xylfe.cn/gtdlzfnuel.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hongshengwenyu.top/gtxfmqhppo.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtduxdlfqs.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.aizwys.cn/gtozvbqjex.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.meibo888.top/gtrwrgpmaz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jyoumei.cn/gtexmfexqg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hammf.cn/gttorecpoz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.havefunace.top/gtrjfwdqsz.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtwvlkqhvo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cashguo.top/gtkimfvrui.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtjhoswhrb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhijiandao.cn/gtrbuxfvut.html

TS:   arr.map(String)
来源：http://hz.vqdsnc.cn/gtvfvrwqvt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yangfankeji.com/gtpwtpzdvu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuxming.cn/gtncqotzfi.html

Ruby: arr.map(&:upcase)
来源：http://hz.iojbl.cn/gtwzwhvjwi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zycfv.cn/gtidgvwvgw.html

[C08] 闭包
来源：http://hz.guannengcc.top/gtpofhelru.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jianghu66.top/gtouhuaven.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtdroyzsef.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtxxtsidvw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtoetmvrxz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zycfv.cn/gtkarsqqql.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.52xcode.cn/gtezsaozoi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fengsongda.top/gtlqphhatx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shanyushiyangtech.top/gtzggneves.html

[C09] 递归
来源：http://hz.ydjk.org.cn/gtnibzyydj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hongshengwenyu.top/gtaxacoasr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.haohaochexian.top/gtcafgucnq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtqcvrxyvv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuxming.cn/gttmyrxkrr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtbeunbloa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhongyouzk.top/gthofeagid.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daria6918.cn/gtooizkuqr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnqzz.top/gtdtuuluiz.html

[C10] 变量作用域
来源：http://hz.svipenyu.cn/gtykpvyuql.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtsornorav.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigfzy.top/gthcjypzzz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xinyue.icu/gtlmruwcox.html

TS:   同 JS
来源：http://hz.daxiang520.top/gtkrxvsdqj.html

Java: 方法内为块级作用域
来源：http://hz.quarkkingdee.top/gtsgwfsbjx.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtffksqcei.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhixingplan.top/gtjsjltuie.html

C#:   块级作用域
来源：http://hz.haohaochexian.top/gttcodjrra.html

[C11] 模块导入与导出
来源：http://hz.jianghu66.top/gtognjlysn.html

Py:   from module import func
来源：http://hz.cucudq.cn/gtvkuczddc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhengqikj.top/gtbdozdaqp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenlongwang.top/gtlavbckib.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ppjwa.cn/gthcbhbgnl.html

Java: import java.util.List;
来源：http://hz.9152youxi.cn/gtlrjzlpbk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gtbopcfngi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangdashe.top/gtcvfklsmk.html

C#:   using System.Text;
来源：http://hz.vqdsnc.cn/gtbccivdjn.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtywftoywc.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtnxdxlupm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jyoumei.cn/gtihrvorxm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtxvnhnghc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtjfjoxfnk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gtrbpnxzwd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.birdmap.top/gthjaocltu.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtmllmysfb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guannengcc.top/gtzxszeekn.html

[C13] 类型声明 / 类型注解
来源：http://hz.yanxiufei.cn/gtlyqkjcdk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xinyue.icu/gtahbxpnfd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtpwshvthp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hysaishi.cn/gtepspjxpx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtrjvwbgok.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gttcqrwyen.html

Go:   func add(a, b int) int
来源：http://hz.hysaishi.cn/gthpkxmrmd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtpgrrcjqu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dianchejie.cn/gtyyzjlleu.html

[C14] 泛型函数
来源：http://hz.yonumen.top/gtdtgexata.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xingfuxueyuan.xyz/gtjdrgatab.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtdlszbtot.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gtcvaucatk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.wangdashe.top/gtsjryvhal.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jyoumei.cn/gtwimniwcu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigfzy.top/gtimoefely.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtzlolonhx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtairgrakq.html

[C15] 解构 / 展开参数
来源：http://hz.jiagoushi.top/gtegoqvaml.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ywan-chungtsiang.top/gttxgzhvpu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtpoolntfa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gotoacloud.top/gtbofkoxfr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tanke756.top/gtokjphcxc.html

Java: // 无解构
来源：http://hz.xuanzx.com/gtrpezcaux.html

Go:   // 无解构
来源：http://hz.sweek.top/gtzwbzrncm.html

Ruby: a, b = pair
来源：http://hz.daxiang520.top/gtjscrmxpe.html

C#:   var (a, b) = pair;
来源：http://hz.hnqzz.top/gtsuutpbay.html

[C16] 函数 / 方法重载
来源：http://hz.aizwys.cn/gtcdaadbbi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.haohaochexian.top/gthfqrciwq.html

PHP:  // 无重载
来源：http://hz.jinyuanbaomall.cn/gthceiqrvk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jyoumei.cn/gtzqegoyhk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shzxlz.cn/gtjwoaqecq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cucudq.cn/gtnyrzjrlu.html

Go:   // 无重载：用不同函数名
来源：http://hz.yvedp.cn/gtgbqwwtsm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtngrffcvh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnxiangtu.top/gtrkyvmgxg.html

================================================================================
来源：http://hz.zdqjudy.top/gtnemxuevt.html

D. 数组 / 列表 / 集合
来源：http://hz.ydjk.org.cn/gtntqecymx.html

================================================================================
来源：http://hz.ivvv.top/gtvaonjlqx.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangtech.top/gtkbjythkf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guannengcc.top/gtvcwfyvle.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtobpsrzhg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtquadajpi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtorfudnho.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxuanxn.top/gtdktibbln.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtmkyyndii.html

Ruby: arr = [1, 2, 3]
来源：http://hz.9152youxi.cn/gtjaoniflp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gotoacloud.top/gtzyzkqsaz.html

[D02] 追加元素到末尾
来源：http://hz.snrcjt.cn/gtyxgasctn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shangyingyoupin.top/gtmuxvqvaa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gtmcjlqsgl.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gtrxnmokck.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtrdgcjjkv.html

Java: list.add(4);
来源：http://hz.dianchejie.cn/gtlbjobhcf.html

Go:   arr = append(arr, 4)
来源：http://hz.xziqi.cn/gtxyzuohqn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangtech.top/gtangekqus.html

C#:   list.Add(4);
来源：http://hz.ywan-chungtsiang.top/gteuhghdxz.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtrssibjhl.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gtiuextexy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgufenzy.top/gtictuhqlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnxiangtu.top/gtzsndrwst.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangtech.top/gtcyfxxske.html

Java: list.add(0, 0);
来源：http://hz.dianchejie.cn/gtvydgqulj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtvschstwn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jiagoushi.top/gtjstqzjlx.html

C#:   list.Insert(0, 0);
来源：http://hz.feifeiyinyue.top/gtvikipxhr.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gtssluijki.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtuojjfbcu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dashuyun.cn/gtccujzehj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtsslhotwb.html

TS:   arr.splice(0, 1);
来源：http://hz.yj202588.top/gthczbhuuc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guannengcc.top/gtmhfqwudo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtetwjeofo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jianghu66.top/gtqxrrjpvg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hfpthk.cn/gtzlbdsgvd.html

[D05] 访问与修改元素
来源：http://hz.hfpthk.cn/gtqblbyftk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtzjidlckt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hywenlv.cn/gtnwjxiing.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtykcyykag.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hongshengwenyu.top/gtvnwbehdt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.dianchejie.cn/gtasyrqjrg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtpwxkltic.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aizwys.cn/gthuguhomu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxuanxn.top/gtkzjxbkzl.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtlqlwpfzg.html

Py:   len(arr)
来源：http://hz.ydzc1.top/gtbishgqdv.html

PHP:  count($arr);
来源：http://hz.birdmap.top/gtprjxqxmb.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtifmpqqck.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtxasqjdhe.html

Java: list.size();
来源：http://hz.jqgufenzy.top/gtnypevzfq.html

Go:   len(arr)
来源：http://hz.quarkkingdee.top/gtgtcbrfsq.html

Ruby: arr.length; arr.size
来源：http://hz.redwolf501.top/gtacvpwomb.html

C#:   list.Count;
来源：http://hz.zhixingplan.top/gtkkhfjaec.html


<!-- 参考信息 -->