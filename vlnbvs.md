代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.xingfuxueyuan.xyz/gtqmypdods.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ppjwa.cn/gtwcjjgpua.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtxatxbtag.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtzidaxngm.html

Java: do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtylljziah.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zdqjudy.top/gtpiiqflaz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gogol.net.cn/gtkvwcwzmr.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtcjhmqopl.html

[B09] break 与 continue
来源：http://hz.cheryme.top/gtwilfxcxb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.chenzaomai.com/gtxsdnmahz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cdnleiting.top/gtizlhaavy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtjgrphuny.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtxqkpxtnp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtaepjwhqy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ydzc1.top/gtzvqpaqez.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhoulong.xyz/gtkajzusca.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtsnxremxc.html

[B10] 遍历同时拿索引
来源：http://hz.meibo888.top/gtckgblbet.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuetiantiany.cn/gtttjvihmb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sweek.top/gtlfrqrwpz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tanke756.top/gtspfzcytc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtykmyuwym.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shzxlz.cn/gtdzkaljnj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sufxvd.cn/gtsvunvolt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yonumen.top/gtthmoyiql.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sxryk.cn/gtplegatsl.html

[B11] 生成数字序列 / 区间
来源：http://hz.fzhhl.top/gtaeodtjkk.html

Py:   list(range(0, 10, 2))
来源：http://hz.shanyushiyangtech.top/gtgypxpezb.html

PHP:  range(0, 10, 2);
来源：http://hz.yvedp.cn/gtyafwgthh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinyuanbaomall.cn/gtrhudjiah.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydzc1.top/gtsjrjyadc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gaohongyu789.top/gtyzjptxlo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hywenlv.cn/gtqeqzwfym.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hnxiangtu.top/gtlkrkkjlv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xinyue.icu/gtogictujq.html

[B12] 跳出多层循环
来源：http://hz.xinyue.icu/gtilnpvwis.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.bjfxy.top/gtpflqexyy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xziqi.cn/gtvbzsmgkt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtxipjopta.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtkhgwiqxd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtipmtopzj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cucudq.cn/gtcxrhblbr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gtmcopjnxh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hfpthk.cn/gtfnbpeibg.html

[B13] 判断是否为数字
来源：http://hz.jianghu66.top/gtdrndvpli.html

Py:   isinstance(x, (int, float))
来源：http://hz.gogol.net.cn/gtwqnnqdnw.html

PHP:  is_numeric($x)
来源：http://hz.jqgfzy.top/gtmrhoyxcw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhoulong.xyz/gtkmptctlo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zycfv.cn/gtnoqdvehv.html

Java: x instanceof Number
来源：http://hz.jyoumei.cn/gtnxeknlkd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxuanxn.top/gtdijchwff.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tianlin.xyz/gtzoadrady.html

C#:   x is int or double or decimal
来源：http://hz.ywan-chungtsiang.top/gtgxhnhqid.html

[B14] 判断值是否在集合内
来源：http://hz.aibaodan.cn/gtsirudyes.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jqgfzy.top/gtgzqsopev.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.dashuyun.cn/gtokympqkj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.316326.xyz/gtimocqxga.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yuxming.cn/gtghqjmpim.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.snrcjt.cn/gtfmeivorm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxinkj.top/gtxfzdulzj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.daria6918.cn/gtkumluykc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cqqwz.cn/gtxqycdenk.html

[B15] 布尔运算与取反
来源：http://hz.ywan-chungtsiang.top/gtmmxmlmdi.html

Py:   a and b or not c
来源：http://hz.guowangkeji.top/gtrxvovrxr.html

PHP:  $a && $b || !$c
来源：http://hz.ydzc1.top/gtpzwmksok.html

JS:   a && b || !c
来源：http://hz.yangfankeji.com/gtknpvcopt.html

TS:   a && b || !c
来源：http://hz.sweek.top/gtfitcoger.html

Java: a && b || !c
来源：http://hz.vqdsnc.cn/gtnigcozru.html

Go:   a && b || !c
来源：http://hz.andypj.xyz/gtnazkskuh.html

Ruby: a && b || !c
来源：http://hz.andypj.xyz/gttcocwrfo.html

C#:   a && b || !c
来源：http://hz.gogol.net.cn/gtzcrilgqy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hongshengwenyu.top/gtpnqdihfq.html

Py:   if not data: return
来源：http://hz.jyoumei.cn/gtbnkckhue.html

PHP:  if (!$data) { return; }
来源：http://hz.tianlin.xyz/gtzpkbdxts.html

JS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtktjtojcg.html

TS:   if (!data) return;
来源：http://hz.pycfn.com/gtqfogfzwx.html

Java: if (data == null) return;
来源：http://hz.nwbrower.top/gtpjxngaxk.html

Go:   if data == nil { return }
来源：http://hz.nwbrower.top/gtdxqukzlv.html

Ruby: return if data.nil?
来源：http://hz.zhongyouzk.top/gtcippanxq.html

C#:   if (data == null) return;
来源：http://hz.sysykeji.top/gteorlbvby.html

================================================================================
来源：http://hz.yongpay.top/gttqsieyyw.html

C. 函数与作用域
来源：http://hz.yvedp.cn/gtqlpclhec.html

================================================================================
来源：http://hz.nanxinkj.top/gtkjwkhqze.html

[C01] 定义函数
来源：http://hz.xinyue.icu/gtpaszgneb.html

Py:   def add(a, b): return a + b
来源：http://hz.xuanzx.com/gthspecgbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gthodvrarv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fzhhl.top/gtsbmrzufo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtqdhdtpjs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtvfrmfczk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hongshengwenyu.top/gtiuydjtjf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cheryme.top/gtshrimrry.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gthtxtoxbr.html

[C02] 默认参数
来源：http://hz.52xcode.cn/gttsvpchhy.html

Py:   def greet(name="World"): return name
来源：http://hz.yj202588.top/gtegcodqob.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.wangshuangyany.cn/gtqvacnnih.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zycfv.cn/gtaukdqmtz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aibaodan.cn/gtfdnelpov.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj202588.top/gtwfuzbnly.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gtdpqjlmhy.html

Ruby: def greet(name = "World") = name
来源：http://hz.xingfuxueyuan.xyz/gtptsmebwp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtojepdwqk.html

[C03] 可变参数
来源：http://hz.kuanghao11.cn/gtfzlazdmb.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtpdafbkab.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtldyifzpj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtcjcpvrdl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gtzbltedvi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhoulong.xyz/gtchfghbdy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gogol.net.cn/gtnwfcefqz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.bjfxy.top/gtjytgfsjn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gtcdegmsya.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtbkfpfvgk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtkzoxizvg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jianghu66.top/gtyynngkvi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ivvv.top/gtikjkqxnf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtphabdjhq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sufxvd.cn/gtlcebbemp.html

Go:   // 无：用配置结构体参数
来源：http://hz.guannengcc.top/gtxzbnlxqp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtrsfgebce.html

C#:   f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtxjconkok.html

[C05] 返回多个值
来源：http://hz.zdqjudy.top/gtozhqpqqh.html

Py:   return a, b
来源：http://hz.sxryk.cn/gtpfnennlp.html

PHP:  return [$a, $b];
来源：http://hz.quarkkingdee.top/gtmpxzfkqh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pycfn.com/gtsydogcxc.html

TS:   return { a, b };
来源：http://hz.fzhhl.top/gthkbfpyda.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xziqi.cn/gtzjibiubk.html

Go:   return a, b
来源：http://hz.jinghuilouyu.cn/gtazogkafz.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtzyohcenn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtiblihstq.html

[C06] 匿名函数 / lambda
来源：http://hz.guowangkeji.top/gtjzhvwauf.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigfzy.top/gtmsdwflma.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jiagoushi.top/gtzsnpbggk.html

JS:   const square = x => x * x;
来源：http://hz.ehwqpu.com/gtaxijlhza.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtqqbowxcd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yangfankeji.com/gtlhuwlzvl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj20258888.top/gtftmpzrgx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cqqwz.cn/gtpwolctiy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jyoumei.cn/gtgqckekmq.html

[C07] 把函数作为参数传入
来源：http://hz.birdmap.top/gtlhbbgrks.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shangyingyoupin.top/gtmcgjdicl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.52xcode.cn/gtsjdqaqxh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jlsjyb.cn/gtwetayphe.html

TS:   arr.map(String)
来源：http://hz.aibaodan.cn/gtfvljvdad.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhongyouzk.top/gtvpaivfbf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinyuanbaomall.cn/gtgwxlbygq.html

Ruby: arr.map(&:upcase)
来源：http://hz.xziqi.cn/gtsjapekrw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gttprkbxyz.html

[C08] 闭包
来源：http://hz.zhoulong.xyz/gtagndilmc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtuinagxhl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gaohongyu789.top/gtqyicmili.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtzdrogycv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtotnmvtjz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shanyushiyangtech.top/gtqmfodcel.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yonumen.top/gtoyazesoa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.havefunace.top/gtbdzinjle.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtwomviiij.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtimnqhryf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.iojbl.cn/gtdcqpmyvj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ywan-chungtsiang.top/gtyarvqmev.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gttutwbzrn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtdzbyyowt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.svipenyu.cn/gtfkeqevle.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuanzx.com/gtjymmxydb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtwetmlhoa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj20258888.top/gtzaglrbjx.html

[C10] 变量作用域
来源：http://hz.yueranfly.top/gtlqxdyequ.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hongshengwenyu.top/gtsvtdikyx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhiwuduotai.top/gtrhmigcpo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtxwgmnttk.html

TS:   同 JS
来源：http://hz.yonumen.top/gtbysqwfbx.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtezutxikn.html

Go:   花括号块级作用域
来源：http://hz.pycfn.com/gtcqlvfggv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.bjfxy.top/gtqvqjbezt.html

C#:   块级作用域
来源：http://hz.shzxlz.cn/gtqozrrcyz.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtcttdxrbb.html

Py:   from module import func
来源：http://hz.shangyingyoupin.top/gtazxzjuei.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtdwutolca.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cucudq.cn/gtdrrlbbhk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.pengpengdd.cyou/gtcerjaooc.html

Java: import java.util.List;
来源：http://hz.chenjidiqi.icu/gtbsbxfxqd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenlongwang.top/gtmbacvdgd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yvedp.cn/gtuidryfiw.html

C#:   using System.Text;
来源：http://hz.guowangkeji.top/gtlyvyrxhv.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtxdunyeyo.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gtzzswpflq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cqqwz.cn/gthoazkoev.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtncxpehim.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhoulong.xyz/gtwadivrih.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sufxvd.cn/gtmpckmapt.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtfhavjvng.html

Ruby: -> { puts "run" }.call
来源：http://hz.hfpthk.cn/gtlhnxberk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtieewmjjd.html

[C13] 类型声明 / 类型注解
来源：http://hz.vqdsnc.cn/gtdffdimjv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cqqwz.cn/gtamlhcwko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtggjxgcbd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gthluovizb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtyvbazmgm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtgtpducqd.html

Go:   func add(a, b int) int
来源：http://hz.jlsjyb.cn/gtyfbkntli.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhixingplan.top/gtohdvydjs.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.redwolf501.top/gtfmdmaijl.html

[C14] 泛型函数
来源：http://hz.pengpengdd.cyou/gtmeuawpzz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xinyue.icu/gtokvqvhhe.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtfddjgszw.html

JS:   // 无泛型
来源：http://hz.9152youxi.cn/gttzvuvmye.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ppjwa.cn/gtqhymscqr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuetiantiany.cn/gtbdunzudd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgufenzy.top/gtceabuozj.html

Ruby: # 无泛型
来源：http://hz.yj20258888.top/gtkypavfoa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yongpay.top/gtntgslqmf.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtfdwwvden.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhengqikj.top/gtinxrvdgw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtqbnvgmyd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtxsopvbar.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cqqwz.cn/gtdnonotuc.html

Java: // 无解构
来源：http://hz.fengsongda.top/gtkkvglatl.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtmdakcpdv.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtzhojirjw.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtmltthfcz.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtfexfexeg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.snrcjt.cn/gtttfgsvrz.html

PHP:  // 无重载
来源：http://hz.sysykeji.top/gtudcgeaqu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gttnyrwdhy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.9152youxi.cn/gtcqykkrib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sxryk.cn/gterfpftzt.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinyuanbaomall.cn/gtyfbiplhe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cqqwz.cn/gtiuvdqtlk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gthslkdtrr.html

================================================================================
来源：http://hz.cashguo.top/gtkrizerbk.html

D. 数组 / 列表 / 集合
来源：http://hz.hfpthk.cn/gtwvcexvpn.html

================================================================================
来源：http://hz.gaohongyu789.top/gtksxobuew.html

[D01] 创建数组 / 列表
来源：http://hz.gaohongyu789.top/gtegtixluu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhijiandao.cn/gtkzhwpvmz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258.top/gttldsifqc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtfpvxzmxf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gtzsigbhfv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tianlin.xyz/gtrfcyjsxo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.birdmap.top/gtiwabfudv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shuidangran.top/gtlqhjjjhi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dashuyun.cn/gtxuodnooh.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtudvatcak.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tian-w.cn/gtmlblkhph.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tanke756.top/gtmfnbxngo.html

JS:   arr.push(4);
来源：http://hz.redwolf501.top/gtlnliuynv.html

TS:   arr.push(4);
来源：http://hz.yuanzhike.top/gtlyjjhhku.html

Java: list.add(4);
来源：http://hz.nwbrower.top/gtyadeobck.html

Go:   arr = append(arr, 4)
来源：http://hz.havefunace.top/gteebjshyc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jlsjyb.cn/gtzzqbjpoj.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gtuuggcopd.html

[D03] 在指定位置插入元素
来源：http://hz.yj202588.top/gtlramhhqk.html

Py:   arr.insert(0, 0)
来源：http://hz.tian-w.cn/gtcxulecrz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.bjfxy.top/gtfjomyhit.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ehwqpu.com/gtrsglwzia.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gaohongyu789.top/gtqjmyzojx.html

Java: list.add(0, 0);
来源：http://hz.gzhubu.top/gtnpxflrkc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuanzhike.top/gttgsqcohe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgfzy.top/gttpbgbuxi.html

C#:   list.Insert(0, 0);
来源：http://hz.feifeiyinyue.top/gtrkakiqcg.html

[D04] 删除元素
来源：http://hz.sxryk.cn/gtahdbtvdi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangkeji.top/gtixcgsubf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nwbrower.top/gtfngwibcp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtizbteqjy.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gtlcnxitfa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hammf.cn/gtmueufqns.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.redwolf501.top/gtycuiwzrw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhaomingkeji.xyz/gttmvmctlz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.quarkkingdee.top/gtxlukuysp.html

[D05] 访问与修改元素
来源：http://hz.meibo888.top/gtukcwdhzb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtrravrpet.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.birdmap.top/gtfcswvqhr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhixingplan.top/gtervhelij.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.redwolf501.top/gtqjdcvovm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenzaomai.com/gtcbojltit.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtuuknpcla.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtkqnsncmj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aizwys.cn/gtxeqyggfa.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtmkkxojbb.html

Py:   len(arr)
来源：http://hz.havefunace.top/gtjcbzbrda.html

PHP:  count($arr);
来源：http://hz.xziqi.cn/gttrnhqndh.html

JS:   arr.length
来源：http://hz.xuetiantiany.cn/gtnjjaegas.html

TS:   arr.length
来源：http://hz.cucudq.cn/gtdcgqwuiq.html

Java: list.size();
来源：http://hz.redwolf501.top/gteowxupkj.html

Go:   len(arr)
来源：http://hz.cheryme.top/gtvxbsjrqv.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtmkklhxok.html

C#:   list.Count;
来源：http://hz.ivvv.top/gtidevtsws.html

[D07] 切片 / 取子数组
来源：http://hz.dashuyun.cn/gtvddqmvpr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhoulong.xyz/gtjpuoanci.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydzc1.top/gtdxpzfqyk.html

JS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtdaeznxay.html

TS:   arr.slice(1, 4);
来源：http://hz.zhoulong.xyz/gtgcjkmzjj.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtwmbyblmu.html

Go:   arr[1:4]
来源：http://hz.yvedp.cn/gtnrxlldnh.html

Ruby: arr[1, 3]
来源：http://hz.9152youxi.cn/gtsqovatrx.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtgryybeoe.html

[D08] 合并两个数组
来源：http://hz.xuetiantiany.cn/gtmposphfd.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtnfyolxvz.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtitfcwtkr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtkhzwidcx.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtmxcibygu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinyuanbaomall.cn/gtxzkomuxe.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gtwqngmqsr.html


<!-- 参考信息 -->