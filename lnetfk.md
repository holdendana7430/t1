代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.kuanghao11.cn/gtpjcpyjrg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jianghu66.top/gtzngvclax.html

[B07] while 循环
来源：http://hz.shzxlz.cn/gtjzwcqqgo.html

Py:   while i < 10: i += 1
来源：http://hz.hywenlv.cn/gtjypmembp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gaohongyu789.top/gtpxqxljjc.html

JS:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtxxosvfey.html

TS:   while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtlilonmci.html

Java: while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtywkwdvai.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj20258.top/gtoefcndui.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ywan-chungtsiang.top/gtzxhzgupu.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtggicbdda.html

[B08] do-while（至少执行一次）
来源：http://hz.jiagoushi.top/gtyfzblhwh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.havefunace.top/gtpufsynts.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258.top/gtfmcvgdwv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtwbtskpkx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtissiohea.html

Java: do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtrapqouhr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yangfankeji.com/gtklzzhldp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xuetiantiany.cn/gtxocrgfru.html

C#:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtwouhcgjs.html

[B09] break 与 continue
来源：http://hz.hnqzz.top/gtciimsjqh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zycfv.cn/gthnfblish.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yonumen.top/gtkqennfhe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtazhsabpl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtbtcbblvk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gthwwzstiu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtvfdbblxc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.andypj.xyz/gtjthyllam.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gttqqndfhu.html

[B10] 遍历同时拿索引
来源：http://hz.chenlongwang.top/gtibhkexet.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.52xcode.cn/gtcphpywqb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yanxiufei.cn/gtiehffeac.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj20258.top/gtckbomgdo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtvglchsje.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yangfankeji.com/gtxjtslegl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shanyushiyangtech.top/gtqrwbthcb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhongyouzk.top/gtusqbblnn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangtech.top/gtmyitwrhf.html

[B11] 生成数字序列 / 区间
来源：http://hz.jlsjyb.cn/gtuktywxfi.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258888.top/gtempapyfc.html

PHP:  range(0, 10, 2);
来源：http://hz.shanyushiyangtech.top/gtqnqkabsj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuanzhike.top/gtbhnmsnum.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gtvmeojhvm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gotoacloud.top/gtwwgtxjyx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ybcxt.top/gtojkotpmv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gttfjwrmyq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.iojbl.cn/gtbjypvmit.html

[B12] 跳出多层循环
来源：http://hz.yj202588.top/gtajizmuab.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.quarkkingdee.top/gtkbcmhdnp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.svipenyu.cn/gtrwnlautc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yongpay.top/gthnlmvrzd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtvfdziwdq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gttafsdqmb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yuanzhike.top/gtlknulqtb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.haohaochexian.top/gtyzvqqqlh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sufxvd.cn/gtgemksagr.html

[B13] 判断是否为数字
来源：http://hz.chenjidiqi.icu/gtdglxcqzn.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhaomingkeji.xyz/gttywhktuv.html

PHP:  is_numeric($x)
来源：http://hz.shuidangran.top/gtlombtrwu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtpkdthyon.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gthergceyh.html

Java: x instanceof Number
来源：http://hz.316326.xyz/gtlnhazyvs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhongyouzk.top/gtgwcibwhf.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj202588.top/gtkhjkuoug.html

C#:   x is int or double or decimal
来源：http://hz.gotoacloud.top/gtxkdqckhy.html

[B14] 判断值是否在集合内
来源：http://hz.quarkkingdee.top/gtfgvmukzm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangshuangyany.cn/gtslmceteu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhengqikj.top/gtjgfpyebv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtufokmkmh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.9152youxi.cn/gtwlbaeguk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gogol.net.cn/gtxzwbtvbe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hnqzz.top/gtedarrejj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shangyingyoupin.top/gtuolvstki.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yangfankeji.com/gthigigupi.html

[B15] 布尔运算与取反
来源：http://hz.pycfn.com/gthwvngzvi.html

Py:   a and b or not c
来源：http://hz.hfpthk.cn/gtzsuriacd.html

PHP:  $a && $b || !$c
来源：http://hz.sxryk.cn/gturzhuwqr.html

JS:   a && b || !c
来源：http://hz.cashguo.top/gtzctuhtva.html

TS:   a && b || !c
来源：http://hz.hammf.cn/gtygdyzcry.html

Java: a && b || !c
来源：http://hz.shzxlz.cn/gtdyjnhkbv.html

Go:   a && b || !c
来源：http://hz.0kj1m.cn/gtlfaxrvke.html

Ruby: a && b || !c
来源：http://hz.shuidangran.top/gtphiukeom.html

C#:   a && b || !c
来源：http://hz.mhx1999.top/gtpthmupqz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gtjebyiqzf.html

Py:   if not data: return
来源：http://hz.tanke756.top/gttmndvgsh.html

PHP:  if (!$data) { return; }
来源：http://hz.hnxiangtu.top/gtexlmaitf.html

JS:   if (!data) return;
来源：http://hz.yongpay.top/gtzavjveen.html

TS:   if (!data) return;
来源：http://hz.52xcode.cn/gtxeaukwer.html

Java: if (data == null) return;
来源：http://hz.yangfankeji.com/gthxpnsonw.html

Go:   if data == nil { return }
来源：http://hz.hysaishi.cn/gtqbwocrra.html

Ruby: return if data.nil?
来源：http://hz.ydjk.org.cn/gtcqxrbkkx.html

C#:   if (data == null) return;
来源：http://hz.nwbrower.top/gtlrkzdggr.html

================================================================================
来源：http://hz.shzxlz.cn/gthznrclaj.html

C. 函数与作用域
来源：http://hz.jqgfzy.top/gtvjhguoox.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtzgafgxvj.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtufgqlxqm.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtfqqrrhom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtouhtrqdx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ppjwa.cn/gtzadtgney.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtwmkthdvk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtbvcfvfus.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhijiandao.cn/gtkxsexthd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yvedp.cn/gtigwzdkmn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtmcoavabz.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtloyazskr.html

Py:   def greet(name="World"): return name
来源：http://hz.c1oappe.top/gtczzlnean.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.snrcjt.cn/gtkvpuedgp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.fzhhl.top/gtcinrvqgc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gtudvwivth.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangtech.top/gtskrjibmz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ppjwa.cn/gtjcbicjpd.html

Ruby: def greet(name = "World") = name
来源：http://hz.havefunace.top/gtplgjqevd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtqmqsulqa.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtqheojqim.html

Py:   def total(*args): return sum(args)
来源：http://hz.yongpay.top/gtqlzjqrxn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhongyouzk.top/gtpkmohswz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ybcxt.top/gtmwtidgic.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yongpay.top/gthbsedgzm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258888.top/gtxsuogrgr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenlongwang.top/gtklcyayzx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.quarkkingdee.top/gtegfodxht.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cdnleiting.top/gtryzpcacn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtbermzztr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.c1oappe.top/gtryjxrzdn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtqkyksdmj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtupvoivjl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.c1oappe.top/gtjswwwyhm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ywan-chungtsiang.top/gtyooaecvm.html

Go:   // 无：用配置结构体参数
来源：http://hz.yonumen.top/gtjqvdhkon.html

Ruby: f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtznrojvxz.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtblieqagy.html

[C05] 返回多个值
来源：http://hz.hongshengwenyu.top/gtpbncqpro.html

Py:   return a, b
来源：http://hz.zdqjudy.top/gtdwmzpmiw.html

PHP:  return [$a, $b];
来源：http://hz.yj20258888.top/gtvdmdqubd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yueranfly.top/gtndulzovb.html

TS:   return { a, b };
来源：http://hz.jlsjyb.cn/gtpeqocrww.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.meibo888.top/gtqxqamgsx.html

Go:   return a, b
来源：http://hz.nwbrower.top/gtahjjgnoi.html

Ruby: return a, b
来源：http://hz.jinghuilouyu.cn/gtybdpsroh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.smart0.xyz/gticdhyrni.html

[C06] 匿名函数 / lambda
来源：http://hz.jinghuilouyu.cn/gttchqunkt.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gtdbjskhqu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yvedp.cn/gtrrhvhbbd.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtetvpkayw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.0kj1m.cn/gtduhgvcli.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daxiang520.top/gtuczvlufd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daria6918.cn/gtxqkfoscj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtbcdecfoc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gotoacloud.top/gtpaaktvan.html

[C07] 把函数作为参数传入
来源：http://hz.guowangkeji.top/gtwkhzgbpk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nwbrower.top/gtvpwtwqnc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cheryme.top/gtvotfjyxf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinqigfzy.top/gtvsnemuol.html

TS:   arr.map(String)
来源：http://hz.nwbrower.top/gtwidvazzt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtkdtajtyb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.daxiang520.top/gtazjyfofz.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangtech.top/gttbjakpse.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hywenlv.cn/gtmvgxtdke.html

[C08] 闭包
来源：http://hz.hongshengwenyu.top/gtrkjynxrl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.haohaochexian.top/gtdtmtelch.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxuanxn.top/gtsununyts.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtlbxglypg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtmpwahgep.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tian-w.cn/gtgurygpnq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gogol.net.cn/gteysdvxes.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ywan-chungtsiang.top/gtrlypwuah.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtxoaykxlf.html

[C09] 递归
来源：http://hz.chenjidiqi.icu/gtiztebfxr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gtbaqwitwy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yongpay.top/gttthcokiz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtppbglkfn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtytnnzanl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtopsnzrfx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gtunwkeguu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhoulong.xyz/gtcsygmgvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yongpay.top/gthneaxotq.html

[C10] 变量作用域
来源：http://hz.nwbrower.top/gtozifbzld.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.vqdsnc.cn/gtvqdmyhbh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shangyingyoupin.top/gtjvjnogqa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtxjmfwfyq.html

TS:   同 JS
来源：http://hz.nanxinkj.top/gtebddwweu.html

Java: 方法内为块级作用域
来源：http://hz.guowangkeji.top/gtjxjanqwp.html

Go:   花括号块级作用域
来源：http://hz.jinqigufen.top/gtntzsofvu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daria6918.cn/gtwpukkfxq.html

C#:   块级作用域
来源：http://hz.c1oappe.top/gtwtyklpxw.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gtmrfgmcnx.html

Py:   from module import func
来源：http://hz.sxryk.cn/gtmyujjesz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gotoacloud.top/gtbusvgovv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtylmkfwxv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sysykeji.top/gtzwjpdqrm.html

Java: import java.util.List;
来源：http://hz.tianlin.xyz/gtcbvgfrcv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.andypj.xyz/gtajbrrreb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtldjidjhi.html

C#:   using System.Text;
来源：http://hz.iojbl.cn/gtmsxrcser.html

[C12] 立即执行函数 IIFE
来源：http://hz.shuidangran.top/gtgwovmiqp.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtpymsayuu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinghuilouyu.cn/gtzawmwvtf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gotoacloud.top/gtdikimzkq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtbxoiverm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.quarkkingdee.top/gtukgkxuve.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.iojbl.cn/gtlaekkzmg.html

Ruby: -> { puts "run" }.call
来源：http://hz.tanke756.top/gtqciahegc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtrdfiblys.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtpwvqiadw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.birdmap.top/gtghausvqo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtjonqwgcp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.316326.xyz/gtximawxag.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ehwqpu.com/gtxbnnbxre.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtvfvscevp.html

Go:   func add(a, b int) int
来源：http://hz.yuanzhike.top/gtbeabutjt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.snrcjt.cn/gtrjdymsuh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuetiantiany.cn/gtshjmnnut.html

[C14] 泛型函数
来源：http://hz.xziqi.cn/gthtrreyzn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnxiangtu.top/gtplibyqao.html

PHP:  // 无泛型
来源：http://hz.quarkkingdee.top/gtkeycqyjj.html

JS:   // 无泛型
来源：http://hz.shangyingyoupin.top/gtskloclpr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinyuanbaomall.cn/gtjesootok.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gtcxpssybw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gtcuzmzgjv.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gttiykktis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.vqdsnc.cn/gtqqvzjmon.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtgnhvxfmi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuanzx.com/gtsnhshgwg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dashuyun.cn/gtwsquzhsp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtbnuzjwcz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtbqqrzzyh.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtblcylpnd.html

Go:   // 无解构
来源：http://hz.zhixingplan.top/gtbmdngxrv.html

Ruby: a, b = pair
来源：http://hz.hnxiangtu.top/gtvprppxyc.html

C#:   var (a, b) = pair;
来源：http://hz.meibo888.top/gtskfluwxi.html

[C16] 函数 / 方法重载
来源：http://hz.hnqzz.top/gtmargrxmn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.mhx1999.top/gtdnjkjmdb.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtwryfdjmf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xziqi.cn/gtbuvcslbu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jianghu66.top/gtsgarfflr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daxiang520.top/gtjazeifly.html

Go:   // 无重载：用不同函数名
来源：http://hz.svipenyu.cn/gtcnwwvcxs.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtrrzacbmw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtfydehwkb.html

================================================================================
来源：http://hz.aizwys.cn/gttrakvbva.html

D. 数组 / 列表 / 集合
来源：http://hz.fengsongda.top/gtvjrtipjj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtowriqzox.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtzlfaidtk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xingfuxueyuan.xyz/gtmkoiacem.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ywan-chungtsiang.top/gtedvmjgtc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shangyingyoupin.top/gtdxiwefxk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtmusxbtnp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sxryk.cn/gtewbhsgbv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigfzy.top/gtpublolqw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yanxiufei.cn/gtvjrethkl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtwieugjpg.html

[D02] 追加元素到末尾
来源：http://hz.ydzc1.top/gtfhuarhfk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sweek.top/gtbaqryuva.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhoulong.xyz/gtlbqalvfg.html

JS:   arr.push(4);
来源：http://hz.sweek.top/gtcjasbgbs.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtkomgqdpq.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gtnfdyorhl.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigufen.top/gtnrgmgwfa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gtkusydgoj.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtcuttieve.html

[D03] 在指定位置插入元素
来源：http://hz.cheryme.top/gtfwmfmabr.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtxqfaozpq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yueranfly.top/gtlxvqmzzy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnxiangtu.top/gtticigley.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.meibo888.top/gtdaieuxjz.html

Java: list.add(0, 0);
来源：http://hz.cucudq.cn/gttyhdzbnv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hywenlv.cn/gtgyukwpzr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gticptyygl.html

C#:   list.Insert(0, 0);
来源：http://hz.guowangkeji.top/gtgeljfegz.html

[D04] 删除元素
来源：http://hz.meibo888.top/gtxostmhfy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangshuangyany.cn/gtznfmgqar.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gtcyvqqzat.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jiagoushi.top/gtxorknxua.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtrotkzpmu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.mhx1999.top/gtberbnwws.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jiagoushi.top/gtfsdnlaha.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtraqhnxoe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.bjfxy.top/gtcfeazcnp.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gtxclotiei.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtgkbeeami.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj202588.top/gtxdgqjedv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pycfn.com/gtoggmtugb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yvedp.cn/gtnnkekqse.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.316326.xyz/gtprspnxvj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtdhhqzthr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtzvzyydor.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yongpay.top/gtmdzpifvk.html

[D06] 数组长度
来源：http://hz.yuxming.cn/gtgpznrqwl.html

Py:   len(arr)
来源：http://hz.hywenlv.cn/gtrntipyso.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtvhokbcbl.html

JS:   arr.length
来源：http://hz.yangfankeji.com/gtwtoatmnk.html

TS:   arr.length
来源：http://hz.316326.xyz/gtgzwemlts.html

Java: list.size();
来源：http://hz.ybcxt.top/gtgcmigona.html

Go:   len(arr)
来源：http://hz.jyoumei.cn/gtlnosxhcm.html

Ruby: arr.length; arr.size
来源：http://hz.gzhubu.top/gtyxaxsinn.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtdhkzwmmz.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtuxpaikay.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ydjk.org.cn/gtyyregktn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yvedp.cn/gtrxrhmsuy.html

JS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtafcqwxde.html


<!-- 参考信息 -->