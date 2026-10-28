代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnqzz.top/gtrxygwbfy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhaomingkeji.xyz/gtoyyethcf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.0kj1m.cn/gtwcxswmdr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.feifeiyinyue.top/gtxvrdpmfi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ydzc1.top/gtdcetqllb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cdnleiting.top/gtndxgftdk.html

[B07] while 循环
来源：http://hz.zhiwuduotai.top/gtdvwkncgk.html

Py:   while i < 10: i += 1
来源：http://hz.chenjidiqi.icu/gtszxphagh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuxming.cn/gthlnhxrpu.html

JS:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtboofvwel.html

TS:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtujwphegw.html

Java: while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtyghyrpdn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xuanzx.com/gtzbrzxhai.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnxiangtu.top/gtsdmtiqbi.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtpljcibvf.html

[B08] do-while（至少执行一次）
来源：http://hz.iojbl.cn/gtbtnxqzlo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gogol.net.cn/gtoprhfjbq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.0kj1m.cn/gttzpxvymv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtemtwaosg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtgxkfwxaw.html

Java: do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtazchmsle.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhaomingkeji.xyz/gtoxmjndgn.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.andypj.xyz/gtkwcecnxm.html

C#:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtukesxugs.html

[B09] break 与 continue
来源：http://hz.zhongyouzk.top/gteyigfanu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.guowangkeji.top/gtxosfrjyc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.meibo888.top/gtqahqexuv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtiyakoyfe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gtbpqvuhgh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtfpzwxbjo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nanxuanxn.top/gtbbcuxbmm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.haohaochexian.top/gtzvrunlgh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gthrqxdxko.html

[B10] 遍历同时拿索引
来源：http://hz.yongpay.top/gtulqbkxsl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhengqikj.top/gtdilpwfgk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fengsongda.top/gtmepqkduh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.bjfxy.top/gtosaxszqz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtgumlzptc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yangfankeji.com/gtvcpbvblv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hongshengwenyu.top/gtdlooosuh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yongpay.top/gtpqcfqwfl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.feifeiyinyue.top/gtyabgzzii.html

[B11] 生成数字序列 / 区间
来源：http://hz.xinyue.icu/gthlbvcszh.html

Py:   list(range(0, 10, 2))
来源：http://hz.bjfxy.top/gtzchhnwex.html

PHP:  range(0, 10, 2);
来源：http://hz.cashguo.top/gttqpmhpus.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ywan-chungtsiang.top/gtqoropvhz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nwbrower.top/gtzibkezrr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hfpthk.cn/gtfsjawdye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gtmmhguoaq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jyoumei.cn/gtqiloyzjh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgufenzy.top/gtttllssyc.html

[B12] 跳出多层循环
来源：http://hz.cdnleiting.top/gtghzelwhp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenzaomai.com/gtqaozdsnq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tanke756.top/gtpcxausgl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtgcargfxt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtqzcucntx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtpxbnjcab.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxinkj.top/gtwkconzul.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shzxlz.cn/gtqxzuggnp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hywenlv.cn/gtfkfrdrbl.html

[B13] 判断是否为数字
来源：http://hz.0kj1m.cn/gtrarabfyf.html

Py:   isinstance(x, (int, float))
来源：http://hz.daxiang520.top/gtjkrozwmn.html

PHP:  is_numeric($x)
来源：http://hz.zdqjudy.top/gthfdpbuqk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xinyue.icu/gtkffbshjf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtvxvevsua.html

Java: x instanceof Number
来源：http://hz.hnqzz.top/gtdyzmajrv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.feifeiyinyue.top/gtdtmydcge.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tian-w.cn/gtfrokcrdr.html

C#:   x is int or double or decimal
来源：http://hz.ehwqpu.com/gtupxfspfu.html

[B14] 判断值是否在集合内
来源：http://hz.zhoulong.xyz/gtzdncbmyq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cashguo.top/gtfavsscoq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.havefunace.top/gtyqywpcvw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shuidangran.top/gtadsyxyub.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtvctnsduj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shanyushiyangkeji.top/gtnuymybjg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sufxvd.cn/gtifbrqhhv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258888.top/gtbmizluky.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gtcjgkozti.html

[B15] 布尔运算与取反
来源：http://hz.sysykeji.top/gtyoayoyra.html

Py:   a and b or not c
来源：http://hz.chenjidiqi.icu/gtqprpzrmv.html

PHP:  $a && $b || !$c
来源：http://hz.yuxming.cn/gteosefsrn.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtnsjcjgzb.html

TS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtkxzupyvs.html

Java: a && b || !c
来源：http://hz.daria6918.cn/gtneurpklj.html

Go:   a && b || !c
来源：http://hz.yonumen.top/gthocwrxaz.html

Ruby: a && b || !c
来源：http://hz.jianghu66.top/gtkbiymdvh.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gtwnyvdxyk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.snrcjt.cn/gtbcjdrrjz.html

Py:   if not data: return
来源：http://hz.yangfankeji.com/gtvmgtfanh.html

PHP:  if (!$data) { return; }
来源：http://hz.havefunace.top/gtibvpbgoi.html

JS:   if (!data) return;
来源：http://hz.tanke756.top/gtfeniwsni.html

TS:   if (!data) return;
来源：http://hz.cucudq.cn/gtkizucijo.html

Java: if (data == null) return;
来源：http://hz.jlsjyb.cn/gtittmhhtm.html

Go:   if data == nil { return }
来源：http://hz.mhx1999.top/gtooacbsfr.html

Ruby: return if data.nil?
来源：http://hz.xinyue.icu/gtpoxxbxks.html

C#:   if (data == null) return;
来源：http://hz.hfpthk.cn/gtokqdenxj.html

================================================================================
来源：http://hz.xylfe.cn/gttimpmlct.html

C. 函数与作用域
来源：http://hz.yj202588.top/gtklberedc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzupunnjw.html

[C01] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtfojknuom.html

Py:   def add(a, b): return a + b
来源：http://hz.gotoacloud.top/gtatgjnxvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtygjrkhvc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtbqhdrnxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtsvsfdkzd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtsihipgnr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtjsbtbgyg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cdnleiting.top/gtzgldnwwq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtjlpjlgnn.html

[C02] 默认参数
来源：http://hz.0kj1m.cn/gtkklakqmg.html

Py:   def greet(name="World"): return name
来源：http://hz.chenzaomai.com/gtflxwrrip.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nwbrower.top/gtwltwtwdw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtzxpmgcot.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xinyue.icu/gtythrbjrb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangshuangyany.cn/gtemvfulca.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgufenzy.top/gtogqgabaz.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhiwuduotai.top/gtzghfanux.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.c1oappe.top/gtgawxktov.html

[C03] 可变参数
来源：http://hz.xingfuxueyuan.xyz/gtuivuhsyr.html

Py:   def total(*args): return sum(args)
来源：http://hz.jqgfzy.top/gtjndqozan.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangdashe.top/gtdiczezii.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtbtajnjkt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtmcrbpoyu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.smart0.xyz/gtgaypnafx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xylfe.cn/gtorprsjin.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.snrcjt.cn/gtxhyidhst.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gttzluosdz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fengsongda.top/gttkjdnpez.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cashguo.top/gtoixbmczv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.316326.xyz/gtobluwcrn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtiancubzt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gogol.net.cn/gtgedldldd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sufxvd.cn/gtrceuvroe.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigfzy.top/gtbjagndli.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtqdlagzxe.html

C#:   f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtlcixflxw.html

[C05] 返回多个值
来源：http://hz.nanxuanxn.top/gtyjyqlmns.html

Py:   return a, b
来源：http://hz.yongpay.top/gtkihvcywu.html

PHP:  return [$a, $b];
来源：http://hz.birdmap.top/gtjbhqzymy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.iojbl.cn/gtvvncljpq.html

TS:   return { a, b };
来源：http://hz.jinqigufen.top/gtaffmaryw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sweek.top/gtprloxogi.html

Go:   return a, b
来源：http://hz.shuidangran.top/gthkeqswac.html

Ruby: return a, b
来源：http://hz.shangyingyoupin.top/gtjwopslic.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.haohaochexian.top/gtdwsbgrdu.html

[C06] 匿名函数 / lambda
来源：http://hz.jinghuilouyu.cn/gtxefmvwuo.html

Py:   square = lambda x: x * x
来源：http://hz.ehwqpu.com/gtvcnkpppv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nanxinkj.top/gttobqhpay.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gthmziyqeb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pycfn.com/gtduugmwca.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.nanxuanxn.top/gtckizsvlm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj20258.top/gticaatyjj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.svipenyu.cn/gtvbsmigsa.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtlricdnqv.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtuorldabf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxinkj.top/gtwwwyxssp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtutuknzyb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hywenlv.cn/gtglrkzpzu.html

TS:   arr.map(String)
来源：http://hz.yuanzhike.top/gtoqgbwtaa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ywan-chungtsiang.top/gtsyidaoea.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gaohongyu789.top/gtovtbutsq.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhongyouzk.top/gtnchdxlqm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daxiang520.top/gtmaxuyiyh.html

[C08] 闭包
来源：http://hz.daxiang520.top/gtkmfzfvfp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sweek.top/gtkxxxmpuv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yvedp.cn/gtlyjtclzr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtvytpgyac.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtqglkwmuz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258888.top/gtacjbmeul.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gteqfxtqcr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gtgxenvlla.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtuvfgvunl.html

[C09] 递归
来源：http://hz.tianlin.xyz/gtkrlnlcsg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenzaomai.com/gttgqwdvwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gtwgxzrenp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtnyqwpiux.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtcarvtewz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtfxmhayvx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenzaomai.com/gtshymqlxj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.redwolf501.top/gtvgybijvd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj20258.top/gtklufouuo.html

[C10] 变量作用域
来源：http://hz.chenjidiqi.icu/gtmsamukhm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gotoacloud.top/gtsquqvyzn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.guannengcc.top/gtukddyokr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tianlin.xyz/gtwjzvscjb.html

TS:   同 JS
来源：http://hz.chenlongwang.top/gtzptsryya.html

Java: 方法内为块级作用域
来源：http://hz.yj202588.top/gtfwzkxvib.html

Go:   花括号块级作用域
来源：http://hz.vqdsnc.cn/gtwtdkzqrb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sysykeji.top/gtfukdwbpg.html

C#:   块级作用域
来源：http://hz.gotoacloud.top/gtuumueclx.html

[C11] 模块导入与导出
来源：http://hz.bjfxy.top/gtwbwnshcj.html

Py:   from module import func
来源：http://hz.nanxinkj.top/gtqkjracxo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yangfankeji.com/gtxztwfosd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sxryk.cn/gtwasozmgl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhiwuduotai.top/gtvnhmscje.html

Java: import java.util.List;
来源：http://hz.fzhhl.top/gtgizoeery.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jianghu66.top/gtzplbctqd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhongyouzk.top/gtmrftblhe.html

C#:   using System.Text;
来源：http://hz.yj20258.top/gtfadlpmcm.html

[C12] 立即执行函数 IIFE
来源：http://hz.hywenlv.cn/gtzfdfmjeb.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gthmsdfziy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fengsongda.top/gtsrlrtvbo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xingfuxueyuan.xyz/gtdopsfyyk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtmqxlgwgi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gttusrldqv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtisypmlkc.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtakmudayq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ywan-chungtsiang.top/gtbhmxlspv.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtzauwgxkm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yongpay.top/gtwwfmkzox.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtnlaaphbr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtiauwyypm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtiavagjcx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtxuicafxz.html

Go:   func add(a, b int) int
来源：http://hz.cashguo.top/gthqnbanli.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ywan-chungtsiang.top/gtcarveyjk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.smart0.xyz/gtwzkbseta.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gtsjxqyluw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtbjmxbpvp.html

PHP:  // 无泛型
来源：http://hz.sysykeji.top/gtdscpkzgh.html

JS:   // 无泛型
来源：http://hz.shuidangran.top/gttwgifhpk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ywan-chungtsiang.top/gtgzclkwie.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jqgufenzy.top/gtnhugqzlt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gtfsfvaoix.html

Ruby: # 无泛型
来源：http://hz.haohaochexian.top/gtsbnotahs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gtojtfuesx.html

[C15] 解构 / 展开参数
来源：http://hz.ydzc1.top/gtzhsqmqif.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.redwolf501.top/gtbdcwqmxv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dashuyun.cn/gtepkbnchy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtxcsjchnx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hywenlv.cn/gtinptksdr.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gtkreykkmk.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gthhrqsfre.html

Ruby: a, b = pair
来源：http://hz.hnxiangtu.top/gthesvuidg.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtkagtdytp.html

[C16] 函数 / 方法重载
来源：http://hz.gaohongyu789.top/gtvqrftqya.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhengqikj.top/gtnhowkyvx.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtepatitxa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhijiandao.cn/gtofhsdyvd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.bjfxy.top/gtshpodpjq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhengqikj.top/gtxuzsteob.html

Go:   // 无重载：用不同函数名
来源：http://hz.jyoumei.cn/gtodwtrylw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtgdtyrnvu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yonumen.top/gtchhmxxxr.html

================================================================================
来源：http://hz.sweek.top/gtudyyzdtn.html

D. 数组 / 列表 / 集合
来源：http://hz.gotoacloud.top/gthpevvpdn.html

================================================================================
来源：http://hz.yuxming.cn/gteaunaljm.html

[D01] 创建数组 / 列表
来源：http://hz.zhiwuduotai.top/gtbcukhvgy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gtultotect.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtzgqcmiok.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtzilswrvw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yangfankeji.com/gtxrxjzuth.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.wangdashe.top/gtnefuyqbc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cucudq.cn/gtqzivhbfr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtcsblqwbl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtdpkcmfyg.html

[D02] 追加元素到末尾
来源：http://hz.shanyushiyangtech.top/gtclkpvlhz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhongyouzk.top/gtccdzkqxq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jyoumei.cn/gttsjpjqni.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtdibrfomx.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtftqufxun.html

Java: list.add(4);
来源：http://hz.zhijiandao.cn/gtjbceriqh.html

Go:   arr = append(arr, 4)
来源：http://hz.feifeiyinyue.top/gtikgippni.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gtabpsxwjk.html

C#:   list.Add(4);
来源：http://hz.meibo888.top/gtepgxzsez.html

[D03] 在指定位置插入元素
来源：http://hz.tanke756.top/gtfhhvyqsq.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtxnplpuyp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hfpthk.cn/gtcfocnsby.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinghuilouyu.cn/gtxdmajfel.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gtwksmvrod.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gteijsiaoc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gtiucitaxo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.redwolf501.top/gtrfndeqvz.html

C#:   list.Insert(0, 0);
来源：http://hz.haohaochexian.top/gtexyyeagj.html

[D04] 删除元素
来源：http://hz.sweek.top/gtmgslhzsb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinqigfzy.top/gtwspvortg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhaomingkeji.xyz/gtzohjjiwn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jlsjyb.cn/gtxpxrimig.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtgboodnfw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gotoacloud.top/gthacuoyey.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenjidiqi.icu/gtvxyzlvzg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gthlhpghms.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fzhhl.top/gtirnfknjq.html

[D05] 访问与修改元素
来源：http://hz.wangdashe.top/gtqinxaotb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtnlwstgnx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtprcgintp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gtdkuitxby.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtysinonki.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtuqkzkvzy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtqtfgfqul.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtruqjfncf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtcqaqrbds.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtdssjdryr.html

Py:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtjtjidqhr.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtjlklcbbq.html

JS:   arr.length
来源：http://hz.zhixingplan.top/gtfvtfiopa.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtegholgxk.html

Java: list.size();
来源：http://hz.chenjidiqi.icu/gtaswcesta.html

Go:   len(arr)
来源：http://hz.dashuyun.cn/gtaaiavryq.html

Ruby: arr.length; arr.size
来源：http://hz.cqqwz.cn/gtobjbpsbi.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtagbjbcmc.html


<!-- 参考信息 -->