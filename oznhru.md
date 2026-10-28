代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.316326.xyz/gtvqrlnrkp.html

JS:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtmnngykcj.html

TS:   while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtgfytkspw.html

Java: while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtgvnezslf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hongshengwenyu.top/gtnpqlrgbz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yueranfly.top/gtfaipkdst.html

C#:   while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gthxvnrqtb.html

[B08] do-while（至少执行一次）
来源：http://hz.dianchejie.cn/gtblfvecyh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ehwqpu.com/gtzbypopar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yuanzhike.top/gttgrjquag.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtxnhmyydk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gticrbrqnk.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhixingplan.top/gtjxeibixl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.havefunace.top/gteqazgwcv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.aizwys.cn/gtwsrfnxmg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtpxqlhwis.html

[B09] break 与 continue
来源：http://hz.gogol.net.cn/gtnxsjgxcv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yj20258.top/gtuitvgzpm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj202588.top/gtrgpwdunn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtkbelxdas.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtcanlbuxe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtsazymgxf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.kuanghao11.cn/gtjchwfjht.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shanyushiyangkeji.top/gtirrwgyrq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtodubqsco.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigfzy.top/gthpyoqgzi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jiagoushi.top/gtkwgadfja.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jyoumei.cn/gtoxzpngdr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtbthcavjf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yvedp.cn/gthvyghhcv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cqqwz.cn/gtcyeygajc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.kuanghao11.cn/gtifofuozu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtlzkihxgt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangshuangyany.cn/gtccgoqzbz.html

[B11] 生成数字序列 / 区间
来源：http://hz.gotoacloud.top/gtsroeseyk.html

Py:   list(range(0, 10, 2))
来源：http://hz.cqqwz.cn/gtpenammtp.html

PHP:  range(0, 10, 2);
来源：http://hz.gotoacloud.top/gtmzuecjsc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtuydbocpk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gtfljdskdm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinghuilouyu.cn/gtqismkmle.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigfzy.top/gttxfewchm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xziqi.cn/gtlldrmrjl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.c1oappe.top/gtncitcatk.html

[B12] 跳出多层循环
来源：http://hz.cucudq.cn/gtnphlxsvr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sxryk.cn/gtefyxuegf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.birdmap.top/gtljwcfnis.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtcpqlofng.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtivusartf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtdkgfwdwy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.aibaodan.cn/gtteewbqsp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gogol.net.cn/gtnwazljjp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sxryk.cn/gtmudjbtjz.html

[B13] 判断是否为数字
来源：http://hz.xylfe.cn/gtubvxppjq.html

Py:   isinstance(x, (int, float))
来源：http://hz.jyoumei.cn/gtvtjbeawh.html

PHP:  is_numeric($x)
来源：http://hz.cashguo.top/gtmxuofrcd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuetiantiany.cn/gtinlwgynh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.feifeiyinyue.top/gtsbystitp.html

Java: x instanceof Number
来源：http://hz.shuidangran.top/gtgmwxnhpz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258888.top/gtxrpueubx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daxiang520.top/gtruudwdko.html

C#:   x is int or double or decimal
来源：http://hz.yuanzhike.top/gticydcyze.html

[B14] 判断值是否在集合内
来源：http://hz.hfpthk.cn/gtgbalkgns.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nanxuanxn.top/gtcxzvjvwf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xziqi.cn/gtufzysbfx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.9152youxi.cn/gtjawsyame.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtmrzoevrj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgfzy.top/gtjgbwphdl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xylfe.cn/gteinbayve.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.birdmap.top/gtjpvszurj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhijiandao.cn/gtqeqrezkq.html

[B15] 布尔运算与取反
来源：http://hz.c1oappe.top/gtytxrmxsw.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtslltumdj.html

PHP:  $a && $b || !$c
来源：http://hz.dianchejie.cn/gtxmcdprwq.html

JS:   a && b || !c
来源：http://hz.gzhubu.top/gtudvmzssj.html

TS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gthtmzucnj.html

Java: a && b || !c
来源：http://hz.jianghu66.top/gtsxmqplln.html

Go:   a && b || !c
来源：http://hz.birdmap.top/gtuasipkox.html

Ruby: a && b || !c
来源：http://hz.yj20258888.top/gtivldltlt.html

C#:   a && b || !c
来源：http://hz.gotoacloud.top/gtrmjobnrc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtqpdgamvw.html

Py:   if not data: return
来源：http://hz.yvedp.cn/gtmemgpato.html

PHP:  if (!$data) { return; }
来源：http://hz.yonumen.top/gtoyzknfuw.html

JS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtkzgbpsiy.html

TS:   if (!data) return;
来源：http://hz.meibo888.top/gtkicdwxaf.html

Java: if (data == null) return;
来源：http://hz.yvedp.cn/gtijldmayi.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtdgoueeuq.html

Ruby: return if data.nil?
来源：http://hz.jianghu66.top/gtsuxnfnft.html

C#:   if (data == null) return;
来源：http://hz.zycfv.cn/gturwxoydt.html

================================================================================
来源：http://hz.ppjwa.cn/gtrpdwlkkx.html

C. 函数与作用域
来源：http://hz.redwolf501.top/gtjdaqxeol.html

================================================================================
来源：http://hz.yuxming.cn/gtssbmkzlu.html

[C01] 定义函数
来源：http://hz.tanke756.top/gtjujjfxct.html

Py:   def add(a, b): return a + b
来源：http://hz.daxiang520.top/gtubvyufhw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtaknvhtzo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtvbvlqclz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtvydbpwyq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtrjcmwkau.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtpcurxlbq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.havefunace.top/gtrrsfmgch.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gthkjddzgm.html

[C02] 默认参数
来源：http://hz.wangshuangyany.cn/gtwujqswvw.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtpxtqojud.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shzxlz.cn/gtodfecaiw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yueranfly.top/gtodksvues.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gtnxcmvvps.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.snrcjt.cn/gtydnodtlv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtmatipjes.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gtsgbcipdw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zycfv.cn/gtgljhzspe.html

[C03] 可变参数
来源：http://hz.jinyuanbaomall.cn/gtpmkkhqyv.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhixingplan.top/gtxpnlxumr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hfpthk.cn/gtguempqnx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gtjuqndeho.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtwwxhuzxb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sufxvd.cn/gtmttlrjrh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fzhhl.top/gtrmzqzgss.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dianchejie.cn/gtzoivytbv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hongshengwenyu.top/gtjkhexnsn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ywan-chungtsiang.top/gtljovcouk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.havefunace.top/gtufoiczeq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gzhubu.top/gtjfuctjmd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.meibo888.top/gtegenjoyj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gteddlfeeb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ehwqpu.com/gtdhccvlyk.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuanzx.com/gtzxuxlntg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtxsicvuao.html

C#:   f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtwscmnekm.html

[C05] 返回多个值
来源：http://hz.zhoulong.xyz/gtybsyulta.html

Py:   return a, b
来源：http://hz.yonumen.top/gtmkgwatkp.html

PHP:  return [$a, $b];
来源：http://hz.hfpthk.cn/gtsokznfuu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cashguo.top/gtgbnbegqz.html

TS:   return { a, b };
来源：http://hz.cucudq.cn/gtaqwqixdv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtndmdcvlz.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtcieizrwm.html

Ruby: return a, b
来源：http://hz.yj20258888.top/gtfosxvjaz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shanyushiyangtech.top/gtiyxdsbzt.html

[C06] 匿名函数 / lambda
来源：http://hz.smart0.xyz/gtmihfzsub.html

Py:   square = lambda x: x * x
来源：http://hz.gzhubu.top/gthcqcourx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.feifeiyinyue.top/gtygxgqzgz.html

JS:   const square = x => x * x;
来源：http://hz.zhongyouzk.top/gtsmtsnxqb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhijiandao.cn/gtbwkfmwvn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jyoumei.cn/gtytnpokfp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gzhubu.top/gtweoyvklp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydjk.org.cn/gtrogupyca.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.kuanghao11.cn/gtwkzaqqam.html

[C07] 把函数作为参数传入
来源：http://hz.zhijiandao.cn/gttkxdeopq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangkeji.top/gtzsfspcco.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.havefunace.top/gtsvyogncl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.iojbl.cn/gtrhiwrtim.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gteqkkupmi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuxming.cn/gtwsnhtloh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgufenzy.top/gtapclacen.html

Ruby: arr.map(&:upcase)
来源：http://hz.smart0.xyz/gtkikphecf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.9152youxi.cn/gtbqvwunkg.html

[C08] 闭包
来源：http://hz.hnxiangtu.top/gtqkqappsn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhoulong.xyz/gtqizpjtuk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fengsongda.top/gthctzywes.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtzcgymesq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtfknwyjnw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenzaomai.com/gtnmlvdzom.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tianlin.xyz/gttkzdbltg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhongyouzk.top/gtmwxpgjml.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtrsrgbvue.html

[C09] 递归
来源：http://hz.zhaomingkeji.xyz/gtgdhcqoql.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtfcstmtcy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pycfn.com/gtywdttown.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtkjyyxtlw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtsduyjqzn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenzaomai.com/gtnzmrzwrv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtafhsmswo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtfzpxwaud.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.fengsongda.top/gtowhsjnpx.html

[C10] 变量作用域
来源：http://hz.hnxiangtu.top/gthfeovzkm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtfepwusjr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgufenzy.top/gtbdewapwf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtrmvkrgsk.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtukituwkp.html

Java: 方法内为块级作用域
来源：http://hz.ydzc1.top/gtkramhdev.html

Go:   花括号块级作用域
来源：http://hz.yj20258888.top/gtafvbosus.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xylfe.cn/gtetwtarha.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtwioxhbkn.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtdwjtbxrn.html

Py:   from module import func
来源：http://hz.iojbl.cn/gtkqozmmjf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtstqntkhe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ybcxt.top/gtmoljgqdm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xylfe.cn/gtfayjfzcn.html

Java: import java.util.List;
来源：http://hz.aizwys.cn/gtjuyrwuwm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xingfuxueyuan.xyz/gtgyqhpbog.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigufen.top/gtaijengpp.html

C#:   using System.Text;
来源：http://hz.guowangkeji.top/gtheuknszf.html

[C12] 立即执行函数 IIFE
来源：http://hz.shuidangran.top/gtkcotiviu.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgufenzy.top/gtfrtcnagt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ivvv.top/gtkgvbgnke.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtxngszsdm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gtmbbcpquy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.vqdsnc.cn/gtnluztdel.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtfrieqnpv.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtofireanq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gthhxpawjx.html

[C13] 类型声明 / 类型注解
来源：http://hz.jianghu66.top/gtyrsppmuh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gttmdjwjja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtlqimnewl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ppjwa.cn/gtoguyaetd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtfbghdylj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gtdxukaoeu.html

Go:   func add(a, b int) int
来源：http://hz.jinyuanbaomall.cn/gtmgtppsef.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.haohaochexian.top/gtynkcpiix.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuanzx.com/gtgdrlcmei.html

[C14] 泛型函数
来源：http://hz.ehwqpu.com/gtvwfjxxra.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gtmrkdsnpx.html

PHP:  // 无泛型
来源：http://hz.jqgufenzy.top/gtpgfjdhyv.html

JS:   // 无泛型
来源：http://hz.nanxuanxn.top/gtahhtzsac.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.iojbl.cn/gteqqwejnq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gotoacloud.top/gtegafzihi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigufen.top/gtfdnaazvg.html

Ruby: # 无泛型
来源：http://hz.feifeiyinyue.top/gtsbqyjlyf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.mhx1999.top/gtksuiqueo.html

[C15] 解构 / 展开参数
来源：http://hz.jinghuilouyu.cn/gtmukvqezd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gzhubu.top/gtwvcixgpm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.c1oappe.top/gtvlqaovfd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtxkuxtnii.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hywenlv.cn/gtxsadrotl.html

Java: // 无解构
来源：http://hz.feifeiyinyue.top/gtoxtaxnfq.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtjjbxztvd.html

Ruby: a, b = pair
来源：http://hz.chenlongwang.top/gtuelcclhg.html

C#:   var (a, b) = pair;
来源：http://hz.vqdsnc.cn/gtjaibhzpm.html

[C16] 函数 / 方法重载
来源：http://hz.birdmap.top/gtaqunxjpa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zdqjudy.top/gtgigukizp.html

PHP:  // 无重载
来源：http://hz.pengpengdd.cyou/gtyrcgwjiz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtvybysajs.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gtcrvpmmuk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtxjpxoona.html

Go:   // 无重载：用不同函数名
来源：http://hz.shangyingyoupin.top/gtjoygdnwn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jyoumei.cn/gtjdetcwjw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gtkwrvecsm.html

================================================================================
来源：http://hz.sweek.top/gtxttwnqeg.html

D. 数组 / 列表 / 集合
来源：http://hz.yanxiufei.cn/gtmwfilrtc.html

================================================================================
来源：http://hz.chenlongwang.top/gtvkkenbgy.html

[D01] 创建数组 / 列表
来源：http://hz.xuetiantiany.cn/gttazdqabg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtnobyhuvn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtessevfog.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yueranfly.top/gtlrjpafff.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fengsongda.top/gtxkjyhdjg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sysykeji.top/gtaodlelrp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gtoffgvkay.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gttvsosqqi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtvecveadv.html

[D02] 追加元素到末尾
来源：http://hz.cashguo.top/gtwfzpkcli.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangtech.top/gtclhvthat.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ehwqpu.com/gtcmumxbkm.html

JS:   arr.push(4);
来源：http://hz.tian-w.cn/gtgsmpwpok.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gtnfjicqki.html

Java: list.add(4);
来源：http://hz.yueranfly.top/gtnzyhpezn.html

Go:   arr = append(arr, 4)
来源：http://hz.c1oappe.top/gtsbcrjzsj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtpaawprwm.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtkrjkvupp.html

[D03] 在指定位置插入元素
来源：http://hz.chenzaomai.com/gtkigtpilz.html

Py:   arr.insert(0, 0)
来源：http://hz.jianghu66.top/gtjzhbpycc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtnvdvomsf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtkiygtmsj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.iojbl.cn/gtwtktsmcm.html

Java: list.add(0, 0);
来源：http://hz.sufxvd.cn/gtvjgwhybx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jiagoushi.top/gtiimbqdxg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tianlin.xyz/gtagxkqhrx.html

C#:   list.Insert(0, 0);
来源：http://hz.ydzc1.top/gtyzekgwrr.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gtmpvchvfh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhiwuduotai.top/gthbjjjiog.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gtrzdeblcd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gthopsfrzs.html

TS:   arr.splice(0, 1);
来源：http://hz.c1oappe.top/gtwoxbdgme.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daxiang520.top/gtsvylhbfb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yvedp.cn/gtetdyihcf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jyoumei.cn/gtxvfmypxt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xinyue.icu/gtihadsiix.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtewzegkpo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtzknrutjr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.52xcode.cn/gtqefdxssq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gthqpweiog.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pengpengdd.cyou/gtxvjtvxvp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cucudq.cn/gtfrncprze.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.mhx1999.top/gtfukvitxz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtehhxcvgr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gtqrnbchiw.html

[D06] 数组长度
来源：http://hz.zhongyouzk.top/gtqfzexqwm.html

Py:   len(arr)
来源：http://hz.feifeiyinyue.top/gtzuwipypq.html

PHP:  count($arr);
来源：http://hz.zhongyouzk.top/gtrtzlwnac.html

JS:   arr.length
来源：http://hz.pengpengdd.cyou/gtrijlqmom.html

TS:   arr.length
来源：http://hz.gaohongyu789.top/gtydzrlvpq.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtyuvfbwma.html

Go:   len(arr)
来源：http://hz.svipenyu.cn/gtaqpkfldq.html

Ruby: arr.length; arr.size
来源：http://hz.316326.xyz/gtkrykrooc.html

C#:   list.Count;
来源：http://hz.redwolf501.top/gtqazuqdib.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtahswijks.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zdqjudy.top/gtjhkdecqv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fzhhl.top/gtberwkill.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gteighqpmj.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtcodtfmed.html

Java: list.subList(1, 4);
来源：http://hz.dashuyun.cn/gtheuffode.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtzyeyenqh.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gttmcfqllh.html


<!-- 参考信息 -->