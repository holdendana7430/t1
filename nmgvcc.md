代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhoulong.xyz/gtsibsogsq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xinyue.icu/gtujmzjrjo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xingfuxueyuan.xyz/gtksrbdjpx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinqigfzy.top/gtogslkual.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.tianlin.xyz/gtppvhjqdf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.tian-w.cn/gtxrsgxccw.html

[B07] while 循环
来源：http://hz.kuanghao11.cn/gtshalpybv.html

Py:   while i < 10: i += 1
来源：http://hz.xinyue.icu/gtqritiayw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.aizwys.cn/gtptpijdpr.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtsxqmsbil.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtrcakvpoy.html

Java: while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtfhurduzl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.316326.xyz/gtvfzylroh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shanyushiyangtech.top/gtanlidqfd.html

C#:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtilfarnby.html

[B08] do-while（至少执行一次）
来源：http://hz.chenjidiqi.icu/gtuypipauu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.quarkkingdee.top/gtkmaapohe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenlongwang.top/gtseasahfv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtqlkcsljc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hongshengwenyu.top/gtmuawmjxj.html

Java: do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtkceupxsb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dashuyun.cn/gtetkauggv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yuxming.cn/gtpkrqbgyf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtacpcyzqe.html

[B09] break 与 continue
来源：http://hz.sxryk.cn/gtnjwowoou.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.dianchejie.cn/gtrtemrzgq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtvhgyqcfm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtlrdebaaa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtifnckvfb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtdlhrslpl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.0kj1m.cn/gtwcwnkick.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgfzy.top/gtjdasbxnu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtsaszucvl.html

[B10] 遍历同时拿索引
来源：http://hz.yueranfly.top/gtsnbfdcsg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jqgufenzy.top/gtdnhgymju.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhengqikj.top/gtwsgwjdme.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.316326.xyz/gtjqacrpai.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtghbtzpgb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.bjfxy.top/gtmandwgqj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aizwys.cn/gthkwdcppt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hongshengwenyu.top/gtbbcvmvza.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jlsjyb.cn/gtfsoimyqx.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgfzy.top/gtdzpwdale.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhiwuduotai.top/gtzvbzrznr.html

PHP:  range(0, 10, 2);
来源：http://hz.snrcjt.cn/gtqafonovw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtcpbqiehw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ehwqpu.com/gtlpfsggjr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.dianchejie.cn/gtbgznxtoe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hysaishi.cn/gtlrwtfjkk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xingfuxueyuan.xyz/gtyvjxrbwa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hnxiangtu.top/gtolammlxv.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gteciltxpv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ppjwa.cn/gtstizrern.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.snrcjt.cn/gtlpklipvf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gtomienfwf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtjwdhfqzc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gteistplbl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ehwqpu.com/gtyiclhcvh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yvedp.cn/gtdjledmjb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shangyingyoupin.top/gtganghjtb.html

[B13] 判断是否为数字
来源：http://hz.sxryk.cn/gteyrredgy.html

Py:   isinstance(x, (int, float))
来源：http://hz.daxiang520.top/gtpyjxlqwn.html

PHP:  is_numeric($x)
来源：http://hz.hongshengwenyu.top/gtjbqzhjig.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cucudq.cn/gtrohwxqbp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.vqdsnc.cn/gtfozkrajy.html

Java: x instanceof Number
来源：http://hz.pengpengdd.cyou/gtyqftjpbs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cucudq.cn/gtijmfuumt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pycfn.com/gtprcgqnhe.html

C#:   x is int or double or decimal
来源：http://hz.smart0.xyz/gtzpmpzysz.html

[B14] 判断值是否在集合内
来源：http://hz.tanke756.top/gtalovjytx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangtech.top/gtiwmiuaqe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenlongwang.top/gtqiktzkax.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hfpthk.cn/gtwrvqhhly.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258.top/gtjjkjwvgb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nwbrower.top/gtkdumumia.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hnqzz.top/gtzndxiolx.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.wangshuangyany.cn/gtthukifbn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ybcxt.top/gtttsqgczg.html

[B15] 布尔运算与取反
来源：http://hz.chenzaomai.com/gtasxmfgqn.html

Py:   a and b or not c
来源：http://hz.jqgufenzy.top/gtzhyfnrjy.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258.top/gtjznrvfcl.html

JS:   a && b || !c
来源：http://hz.hysaishi.cn/gtbbuqkdrs.html

TS:   a && b || !c
来源：http://hz.aizwys.cn/gtrzgjdvbh.html

Java: a && b || !c
来源：http://hz.havefunace.top/gtfxgnwtbx.html

Go:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtjnimlfov.html

Ruby: a && b || !c
来源：http://hz.yongpay.top/gteckoddmj.html

C#:   a && b || !c
来源：http://hz.jianghu66.top/gtgnlezekc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.316326.xyz/gtgghhqzjw.html

Py:   if not data: return
来源：http://hz.hongshengwenyu.top/gtcchobfrn.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtfswxmzuj.html

JS:   if (!data) return;
来源：http://hz.tanke756.top/gtfwytvgpn.html

TS:   if (!data) return;
来源：http://hz.sysykeji.top/gtpacuhoyf.html

Java: if (data == null) return;
来源：http://hz.nanxinkj.top/gtvwdfmwrz.html

Go:   if data == nil { return }
来源：http://hz.nanxinkj.top/gtwglleglx.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gtqaggfdqg.html

C#:   if (data == null) return;
来源：http://hz.cdnleiting.top/gtjikwblyo.html

================================================================================
来源：http://hz.meibo888.top/gtfxsvznoe.html

C. 函数与作用域
来源：http://hz.shuidangran.top/gtbarcbmoy.html

================================================================================
来源：http://hz.jqgfzy.top/gtruyvzsyv.html

[C01] 定义函数
来源：http://hz.aizwys.cn/gtcifmvydl.html

Py:   def add(a, b): return a + b
来源：http://hz.tanke756.top/gtkuvvgxkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtyjrgfmvz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.aizwys.cn/gtnjzerwdt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtbysrxonk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtofwxwwxo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gtvlipjjnk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ivvv.top/gtjvtvonfs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtfgcnjnsy.html

[C02] 默认参数
来源：http://hz.shuidangran.top/gtkfspwdzp.html

Py:   def greet(name="World"): return name
来源：http://hz.smart0.xyz/gtwraqfgzc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aibaodan.cn/gtghmwuiuo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtknofydcr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj202588.top/gtnmrqmzqi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtjvsfclua.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guannengcc.top/gtlxxjayzu.html

Ruby: def greet(name = "World") = name
来源：http://hz.snrcjt.cn/gtliaqiggg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zdqjudy.top/gtlynkkupv.html

[C03] 可变参数
来源：http://hz.zhixingplan.top/gtyzzrzvnf.html

Py:   def total(*args): return sum(args)
来源：http://hz.hfpthk.cn/gtlrrurwzy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ppjwa.cn/gtvtfpmdix.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yongpay.top/gtpwpaeqna.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtsavefeym.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhiwuduotai.top/gtpsxdmxqg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigufen.top/gtndvujysg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhixingplan.top/gtjlgmjakc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jlsjyb.cn/gtahpwbusn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtprsllbix.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gtnxdgmknq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangkeji.top/gtfmipqfwk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gtwyuekrah.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtmyjhbmkb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.iojbl.cn/gtlgdviyhz.html

Go:   // 无：用配置结构体参数
来源：http://hz.316326.xyz/gtupgttyrf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtkbnkpatv.html

C#:   f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtlhrxaskh.html

[C05] 返回多个值
来源：http://hz.yuanzhike.top/gtdyrsrwdk.html

Py:   return a, b
来源：http://hz.sufxvd.cn/gtoolqcruw.html

PHP:  return [$a, $b];
来源：http://hz.xziqi.cn/gtrkmmnmfy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pengpengdd.cyou/gtjyyfzmgv.html

TS:   return { a, b };
来源：http://hz.hywenlv.cn/gtsypiejzq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinyuanbaomall.cn/gtyftkwdsh.html

Go:   return a, b
来源：http://hz.ydzc1.top/gtplvwhtcf.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gttbsysemk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.daxiang520.top/gtqebpohkk.html

[C06] 匿名函数 / lambda
来源：http://hz.zhaomingkeji.xyz/gttmwhdfrf.html

Py:   square = lambda x: x * x
来源：http://hz.ppjwa.cn/gtyimxmgme.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinyuanbaomall.cn/gttooggugm.html

JS:   const square = x => x * x;
来源：http://hz.hnqzz.top/gtshhllvaw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guannengcc.top/gtnsnaqxjc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.quarkkingdee.top/gtimvsisuq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ywan-chungtsiang.top/gtygctoiww.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jyoumei.cn/gtcoxmqclz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhiwuduotai.top/gtisoanfgt.html

[C07] 把函数作为参数传入
来源：http://hz.zhengqikj.top/gtkifemjmy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hnqzz.top/gtkbwkwyzp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hongshengwenyu.top/gtbhykzqxm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtaurqehaw.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gtnapsvryo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hongshengwenyu.top/gtlxbwbcwx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gtmhhgnntm.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gtofvzlnrj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtfcpstrxj.html

[C08] 闭包
来源：http://hz.ehwqpu.com/gtwdqzongp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xziqi.cn/gtincnxmum.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtmbumtkya.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gteoymejbc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtecpvyqma.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pycfn.com/gtcezlpamy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.svipenyu.cn/gtjmikinco.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guannengcc.top/gtrfsjkxoh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtjxvdglxs.html

[C09] 递归
来源：http://hz.dashuyun.cn/gtbspxryeo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtsuybwuhm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gthvvmlhzz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gtzqnegqae.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jianghu66.top/gthcdonawc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtocsxsphm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.wangshuangyany.cn/gtzxkannoo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtnvcxtzln.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtqdivwqzu.html

[C10] 变量作用域
来源：http://hz.gotoacloud.top/gttxjbljek.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenjidiqi.icu/gtjisdaiad.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ywan-chungtsiang.top/gttggzzwtp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dashuyun.cn/gtxnkgbvlv.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtajzmafko.html

Java: 方法内为块级作用域
来源：http://hz.yongpay.top/gtbvuebfea.html

Go:   花括号块级作用域
来源：http://hz.ivvv.top/gtdmjjuxxq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhoulong.xyz/gtwcyvfkxp.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtwtqufaba.html

[C11] 模块导入与导出
来源：http://hz.cashguo.top/gtpisukigt.html

Py:   from module import func
来源：http://hz.ybcxt.top/gthujtcsvb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtrqmquleh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtpaehglue.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtzibmlruv.html

Java: import java.util.List;
来源：http://hz.hongshengwenyu.top/gtexlpoqjx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cucudq.cn/gtveirkqme.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxuanxn.top/gtyilltxnc.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtavlktuit.html

[C12] 立即执行函数 IIFE
来源：http://hz.yanxiufei.cn/gtxndhvzpe.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtmyorjtdl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhongyouzk.top/gtrfnzwbxa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtctvpghde.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtlsfdnucb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgufenzy.top/gtfdoitenn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xinyue.icu/gtahphnaiq.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuanzx.com/gtaryqwhyv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuanzhike.top/gtkvzirbxm.html

[C13] 类型声明 / 类型注解
来源：http://hz.nanxinkj.top/gtwqlruwjs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtdwjfcyvd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtwctzdyss.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jlsjyb.cn/gtadgffcym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtoimtqnpo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtivjzaufk.html

Go:   func add(a, b int) int
来源：http://hz.ydzc1.top/gttzqzjiwj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cashguo.top/gtjsrfmwcj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhongyouzk.top/gtempqsyzq.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gtvutxpuhm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxinkj.top/gtrnlrpvfi.html

PHP:  // 无泛型
来源：http://hz.jinghuilouyu.cn/gtdmkkpbgz.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtmzcldnti.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydjk.org.cn/gtmbqzepyy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtdyogaopv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangshuangyany.cn/gtltvexgiw.html

Ruby: # 无泛型
来源：http://hz.ivvv.top/gtfknkqdpa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtykeezitm.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gtnrfobnmu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhongyouzk.top/gtsxpcbmzj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydzc1.top/gtsqefxhve.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hammf.cn/gtragwxoou.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.bjfxy.top/gtcuqdchmd.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtzaeqfwns.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gthbhqwjfm.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtzjwzlnog.html

C#:   var (a, b) = pair;
来源：http://hz.wangshuangyany.cn/gttakthuze.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtxjbhrmls.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.bjfxy.top/gtwulqlrbo.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gtbyiwizue.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aibaodan.cn/gtcvmtstoq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.316326.xyz/gtpfdmfyrn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shangyingyoupin.top/gtawzddoeo.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtslrwfqig.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yonumen.top/gtxwswhgaj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ehwqpu.com/gtclflkbza.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoyyahqnu.html

D. 数组 / 列表 / 集合
来源：http://hz.jyoumei.cn/gtehbvrvaf.html

================================================================================
来源：http://hz.tanke756.top/gtfuadmewl.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtteoiyzfl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sxryk.cn/gtbhibqgqz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtnjbcairi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shuidangran.top/gtbwextszv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pengpengdd.cyou/gtpgxbvekz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gogol.net.cn/gttrmxlipm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pycfn.com/gtdpikwdzu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ybcxt.top/gtxlqophxl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hnqzz.top/gtqqyndapq.html

[D02] 追加元素到末尾
来源：http://hz.ybcxt.top/gtlyulsfmf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jianghu66.top/gtqgjvnypm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuanzhike.top/gtsidyafna.html

JS:   arr.push(4);
来源：http://hz.sweek.top/gtvilhwykv.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtkzzmxtnc.html

Java: list.add(4);
来源：http://hz.zhiwuduotai.top/gtfsrkbogj.html

Go:   arr = append(arr, 4)
来源：http://hz.hammf.cn/gtowuocjeb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydzc1.top/gtuzsdvojf.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangtech.top/gtmrtnyjnx.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtbjtzilwi.html

Py:   arr.insert(0, 0)
来源：http://hz.yuanzhike.top/gtjnljiwtn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenzaomai.com/gtucqtfiqm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.iojbl.cn/gtaejtwsdx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinyuanbaomall.cn/gtzcnbkaqa.html

Java: list.add(0, 0);
来源：http://hz.shangyingyoupin.top/gtpftqooeq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.smart0.xyz/gtbubjqnvd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gtbpvbzlyf.html

C#:   list.Insert(0, 0);
来源：http://hz.hysaishi.cn/gtufurdtdc.html

[D04] 删除元素
来源：http://hz.ydzc1.top/gtsnaghfkm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinyuanbaomall.cn/gtmujpfqcq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sufxvd.cn/gtiidrahef.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtnqvalpxx.html

TS:   arr.splice(0, 1);
来源：http://hz.zdqjudy.top/gtfqeeveeg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ywan-chungtsiang.top/gtxtkipakl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.dianchejie.cn/gtwnqrbuwo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.snrcjt.cn/gtwiqwvvjw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sxryk.cn/gtoxysnrfd.html

[D05] 访问与修改元素
来源：http://hz.hfpthk.cn/gtexxtvcmx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gtdkcrewiz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtfykcasms.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tianlin.xyz/gtqambmzyv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gtiahasnzi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtfslyolmf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtoiuddnxb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtbszpwbxn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtidhrwcpq.html

[D06] 数组长度
来源：http://hz.birdmap.top/gtytwjzeme.html

Py:   len(arr)
来源：http://hz.xziqi.cn/gtukhwmzir.html

PHP:  count($arr);
来源：http://hz.snrcjt.cn/gtkcioulpg.html

JS:   arr.length
来源：http://hz.cheryme.top/gtsmjthzlw.html

TS:   arr.length
来源：http://hz.meibo888.top/gtckrnedcy.html

Java: list.size();
来源：http://hz.tanke756.top/gtlkzwaubp.html

Go:   len(arr)
来源：http://hz.yongpay.top/gtuhgkdeuz.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gtwakwhcca.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtxbeuarur.html


<!-- 参考信息 -->