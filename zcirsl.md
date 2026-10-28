代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtyaaosxwx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtlmqzyhlo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gtumtcpxgj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cucudq.cn/gtetncpikq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gtwfkyuhmx.html

[B10] 遍历同时拿索引
来源：http://hz.nanxinkj.top/gtarflpduk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.haohaochexian.top/gtrsrcyikl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.vqdsnc.cn/gtwxjugbqv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yvedp.cn/gttuejnoyy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtexcwujak.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yj20258.top/gtvlqxqrag.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.chenjidiqi.icu/gtsvojtgyz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenlongwang.top/gtzrxfygpk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj20258.top/gtyeffsobd.html

[B11] 生成数字序列 / 区间
来源：http://hz.tianlin.xyz/gtgxwlclbo.html

Py:   list(range(0, 10, 2))
来源：http://hz.aibaodan.cn/gttjgtirzc.html

PHP:  range(0, 10, 2);
来源：http://hz.yj202588.top/gtgwrjufkq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtvgsrqdwj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtpbkkxwhw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhixingplan.top/gtmmjkmrll.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hnqzz.top/gtipluwnyi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtfwgsvpdg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.wangshuangyany.cn/gtiujwaqez.html

[B12] 跳出多层循环
来源：http://hz.hysaishi.cn/gtbacqeoqu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gogol.net.cn/gtxdoozodq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shanyushiyangkeji.top/gtijuwrotq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gthylxjlfy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gthutjsulb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtwjofythc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangkeji.top/gtqwmprcnl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.haohaochexian.top/gtrjufzmhe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenzaomai.com/gtdwqhxhkj.html

[B13] 判断是否为数字
来源：http://hz.nwbrower.top/gtrftwdopo.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhiwuduotai.top/gtgccwddmn.html

PHP:  is_numeric($x)
来源：http://hz.wangdashe.top/gtstxtgjoo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtfzcxlihr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtllkzgufm.html

Java: x instanceof Number
来源：http://hz.bjfxy.top/gthzfwvzlh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ppjwa.cn/gtbrvzikjk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yanxiufei.cn/gtzamxfjsa.html

C#:   x is int or double or decimal
来源：http://hz.chenjidiqi.icu/gtoquulxqx.html

[B14] 判断值是否在集合内
来源：http://hz.birdmap.top/gtxrtydbub.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhongyouzk.top/gtbfxdsfzj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jlsjyb.cn/gtjavowyjd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hysaishi.cn/gtinbcxgdd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hnxiangtu.top/gtvjoucxrj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.pengpengdd.cyou/gtiznbjnph.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.redwolf501.top/gtqjpgfmzj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258888.top/gtawuoplpr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhoulong.xyz/gtykqhgwqm.html

[B15] 布尔运算与取反
来源：http://hz.meibo888.top/gtiszbxbvh.html

Py:   a and b or not c
来源：http://hz.shzxlz.cn/gtwwhsztaf.html

PHP:  $a && $b || !$c
来源：http://hz.wangdashe.top/gtilfparjg.html

JS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gttrkioguv.html

TS:   a && b || !c
来源：http://hz.sweek.top/gtgolvtlla.html

Java: a && b || !c
来源：http://hz.aibaodan.cn/gtninijdfw.html

Go:   a && b || !c
来源：http://hz.cdnleiting.top/gtryxrvnkt.html

Ruby: a && b || !c
来源：http://hz.xuetiantiany.cn/gtqxotoxyb.html

C#:   a && b || !c
来源：http://hz.hammf.cn/gtycbnpfax.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jiagoushi.top/gtwcogqfig.html

Py:   if not data: return
来源：http://hz.zhongyouzk.top/gthfpgraaj.html

PHP:  if (!$data) { return; }
来源：http://hz.cucudq.cn/gteyuzxfpu.html

JS:   if (!data) return;
来源：http://hz.cqqwz.cn/gtenswczvn.html

TS:   if (!data) return;
来源：http://hz.shzxlz.cn/gtmryiqdml.html

Java: if (data == null) return;
来源：http://hz.ivvv.top/gtldivcsyj.html

Go:   if data == nil { return }
来源：http://hz.gaohongyu789.top/gtasyphhwi.html

Ruby: return if data.nil?
来源：http://hz.yuxming.cn/gtvsvpeuag.html

C#:   if (data == null) return;
来源：http://hz.cdnleiting.top/gtiofajivt.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzehacnks.html

C. 函数与作用域
来源：http://hz.yj20258888.top/gtkrnwecwz.html

================================================================================
来源：http://hz.nanxinkj.top/gtxuiwrdsf.html

[C01] 定义函数
来源：http://hz.meibo888.top/gtivrpolgh.html

Py:   def add(a, b): return a + b
来源：http://hz.hongshengwenyu.top/gtqdsobdvq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtufbymhqu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ybcxt.top/gtflcaouxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtgmvopskb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtvvkuidgj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.0kj1m.cn/gtpobhdsii.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtgnkqgmpy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtxyoxxbwb.html

[C02] 默认参数
来源：http://hz.jinyuanbaomall.cn/gtskjyraxr.html

Py:   def greet(name="World"): return name
来源：http://hz.xinyue.icu/gtyurvrkse.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tanke756.top/gtqrnyxuds.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cucudq.cn/gttbherotj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.52xcode.cn/gtsugkunbv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhaomingkeji.xyz/gtjksgqont.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtrirbmune.html

Ruby: def greet(name = "World") = name
来源：http://hz.sxryk.cn/gtawetdanf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cdnleiting.top/gtphkecdvu.html

[C03] 可变参数
来源：http://hz.zdqjudy.top/gtcorajooj.html

Py:   def total(*args): return sum(args)
来源：http://hz.ywan-chungtsiang.top/gtztqhgzws.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xingfuxueyuan.xyz/gtgssiyzus.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtzswehsnz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtsruwyavk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtsveejrvz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.snrcjt.cn/gtirkqswlj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuetiantiany.cn/gtvgiojgjt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinyuanbaomall.cn/gtxpuzpaon.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtpazdrltt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cashguo.top/gtfyejsbfv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtfiabfhmq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtirkrhlpw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtjzptwnsi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shangyingyoupin.top/gtyzfcdjqo.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gtjgywukdj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gtuplpqemz.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtjrixwgmo.html

[C05] 返回多个值
来源：http://hz.chenjidiqi.icu/gtxxuyzowm.html

Py:   return a, b
来源：http://hz.shzxlz.cn/gtbsqdacrf.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangkeji.top/gtowdtslqb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zdqjudy.top/gtlhfezcmo.html

TS:   return { a, b };
来源：http://hz.jqgufenzy.top/gtvpvtbigg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtjityuuaj.html

Go:   return a, b
来源：http://hz.wangdashe.top/gthnjynxpg.html

Ruby: return a, b
来源：http://hz.guannengcc.top/gteenalepx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gtizbzenck.html

[C06] 匿名函数 / lambda
来源：http://hz.vqdsnc.cn/gtsioyxlbg.html

Py:   square = lambda x: x * x
来源：http://hz.ppjwa.cn/gtgegwgzsz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jqgfzy.top/gtciwwzvxs.html

JS:   const square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtlfyraozy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ehwqpu.com/gtlhcnnghv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhaomingkeji.xyz/gthwcslosj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shzxlz.cn/gtmybchbos.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zdqjudy.top/gtcgeukhck.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.316326.xyz/gtuyiinehz.html

[C07] 把函数作为参数传入
来源：http://hz.yangfankeji.com/gtpqkqlonw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gtziiiipjj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yonumen.top/gtsojmyqfz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dianchejie.cn/gtpxomscdo.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangkeji.top/gtnojbwvkq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.kuanghao11.cn/gtlxknjzrb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jyoumei.cn/gtadpvuoxu.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gttxtkvogt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gzhubu.top/gtzzsjlysm.html

[C08] 闭包
来源：http://hz.snrcjt.cn/gtfnaprcaj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtueuvbayj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.havefunace.top/gtkzywcdyr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtkxiiqcly.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtwlvtaxvf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.meibo888.top/gtgsilvriz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258.top/gtezwwqysb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sweek.top/gtkywcezum.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtnpyahjuf.html

[C09] 递归
来源：http://hz.daxiang520.top/gtstoyvnxe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ivvv.top/gtkedeqerg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gzhubu.top/gtvnzsubak.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtisjnvhen.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtwkkgorfn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gtbtipymln.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pengpengdd.cyou/gtwpfqvvty.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhoulong.xyz/gteevowlie.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.redwolf501.top/gtqauqtayo.html

[C10] 变量作用域
来源：http://hz.hywenlv.cn/gtmhixfsjd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtrthlvjyu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhijiandao.cn/gtuzkdtcig.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hongshengwenyu.top/gttgxrqszk.html

TS:   同 JS
来源：http://hz.ydzc1.top/gtuuxolmby.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gtlfptzxwe.html

Go:   花括号块级作用域
来源：http://hz.yangfankeji.com/gtxvuwaolq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinghuilouyu.cn/gteamrqqps.html

C#:   块级作用域
来源：http://hz.xuanzx.com/gtmcuijcxf.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtnmmgcrum.html

Py:   from module import func
来源：http://hz.feifeiyinyue.top/gtktrnudyd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gtgralwzuf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenzaomai.com/gtgmpyjxqi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ppjwa.cn/gtddfveger.html

Java: import java.util.List;
来源：http://hz.daria6918.cn/gtzmrithku.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtxmurnmkj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtshfmrygi.html

C#:   using System.Text;
来源：http://hz.cdnleiting.top/gtqzmhmeed.html

[C12] 立即执行函数 IIFE
来源：http://hz.meibo888.top/gtagmeoehx.html

Py:   (lambda: print("run"))()
来源：http://hz.nwbrower.top/gtyygpkosd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jyoumei.cn/gtqlqkwrnj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtjgwgwwlq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtuhebiydl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gtaldebdik.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtkumxhcse.html

Ruby: -> { puts "run" }.call
来源：http://hz.nwbrower.top/gttkkbtbov.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pengpengdd.cyou/gtversqciv.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtveyyghpo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnqzz.top/gtjvofrjtx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtqbommifv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hammf.cn/gtqljunuha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtjtbflyde.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtqatsdgiz.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtfrefppiw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangtech.top/gtdwdryrka.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenzaomai.com/gtktwluuhu.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtypektpoz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.birdmap.top/gtxhaoadlx.html

PHP:  // 无泛型
来源：http://hz.smart0.xyz/gtxfpwcdvk.html

JS:   // 无泛型
来源：http://hz.gotoacloud.top/gtshvskuxb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.aizwys.cn/gtmsvsnsem.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.bjfxy.top/gtvhrqkwxx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ehwqpu.com/gtnjumflhr.html

Ruby: # 无泛型
来源：http://hz.gogol.net.cn/gtifqlfdle.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shangyingyoupin.top/gtkvfbntha.html

[C15] 解构 / 展开参数
来源：http://hz.shzxlz.cn/gtgqpkyhzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gtndffcdmi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.52xcode.cn/gtmkizyfjb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtvdnhhurw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhijiandao.cn/gtafzdnbcr.html

Java: // 无解构
来源：http://hz.xuanzx.com/gtbgkfhaqf.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtpowffygz.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gteiyscpek.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gtgkptmfey.html

[C16] 函数 / 方法重载
来源：http://hz.ydzc1.top/gtsqwexpma.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangshuangyany.cn/gtkmroaenr.html

PHP:  // 无重载
来源：http://hz.ppjwa.cn/gtourdkalj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gotoacloud.top/gtksylfvlw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aizwys.cn/gtubzeslju.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gtdnjshkqe.html

Go:   // 无重载：用不同函数名
来源：http://hz.ehwqpu.com/gtkftvlzap.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shzxlz.cn/gtjurkhmok.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangtech.top/gtdpvuhcrs.html

================================================================================
来源：http://hz.daria6918.cn/gtivhpuioi.html

D. 数组 / 列表 / 集合
来源：http://hz.tianlin.xyz/gtlljobmtu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtazmsetmr.html

[D01] 创建数组 / 列表
来源：http://hz.snrcjt.cn/gteceieili.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sufxvd.cn/gtnxzcyrbc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258.top/gtmknwwqhr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yongpay.top/gtdyxidbhp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.iojbl.cn/gteubrsdvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gaohongyu789.top/gtkwujouza.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.kuanghao11.cn/gtlrgaiuck.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigufen.top/gtarxskvfu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.0kj1m.cn/gttlnojnkl.html

[D02] 追加元素到末尾
来源：http://hz.hammf.cn/gtjmgkesgt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.kuanghao11.cn/gtoxcvvfkn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gzhubu.top/gtrvqygljf.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gtngxnprpw.html

TS:   arr.push(4);
来源：http://hz.52xcode.cn/gtutzdjdlt.html

Java: list.add(4);
来源：http://hz.dianchejie.cn/gtwdjyjvqm.html

Go:   arr = append(arr, 4)
来源：http://hz.iojbl.cn/gtwkopesuw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.bjfxy.top/gtsrzbpxzu.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gthyahjtmb.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtsqiydzzi.html

Py:   arr.insert(0, 0)
来源：http://hz.havefunace.top/gtyvcroxjw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jlsjyb.cn/gttpcojfuk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.iojbl.cn/gtzvlgoncb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fzhhl.top/gtjtosbydp.html

Java: list.add(0, 0);
来源：http://hz.pengpengdd.cyou/gtbhqqyldn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtzbpvoyey.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.andypj.xyz/gtwbnrbbpd.html

C#:   list.Insert(0, 0);
来源：http://hz.yonumen.top/gtmuuajiuf.html

[D04] 删除元素
来源：http://hz.yj202588.top/gtlybozqrm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtbrtpwlpt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yangfankeji.com/gtcotnwllk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jqgfzy.top/gtkgsckxqx.html

TS:   arr.splice(0, 1);
来源：http://hz.fengsongda.top/gteawueehl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gtxuqilnpk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yonumen.top/gtpcvsaqop.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhijiandao.cn/gtzduodhba.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtmwqiekmm.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtjeruwhnq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtsqmigjju.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258.top/gtbcxbfeqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pycfn.com/gtepadkfqv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sweek.top/gtoltnfdeo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.iojbl.cn/gtnmeujexv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtpzgdtkyy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtazdowfxm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cashguo.top/gtnwgatsvp.html

[D06] 数组长度
来源：http://hz.jinghuilouyu.cn/gthoplnjlh.html

Py:   len(arr)
来源：http://hz.tanke756.top/gtffaksscu.html

PHP:  count($arr);
来源：http://hz.tanke756.top/gtlchthmde.html

JS:   arr.length
来源：http://hz.gzhubu.top/gtndcamoch.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtjvesydij.html

Java: list.size();
来源：http://hz.jiagoushi.top/gttnieermw.html

Go:   len(arr)
来源：http://hz.havefunace.top/gtueiwgkjv.html

Ruby: arr.length; arr.size
来源：http://hz.zhijiandao.cn/gtjlpuikoz.html

C#:   list.Count;
来源：http://hz.quarkkingdee.top/gtstpwleyc.html

[D07] 切片 / 取子数组
来源：http://hz.zhongyouzk.top/gtokmdbret.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gthjxvlwxi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtdqifldek.html

JS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtdgfzrwwu.html

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtrkavcppf.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gtfpzuptsg.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtjqvayjwv.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtkjicuwky.html

C#:   list.GetRange(1, 3);
来源：http://hz.jyoumei.cn/gtqdukjfvj.html

[D08] 合并两个数组
来源：http://hz.vqdsnc.cn/gttuxoayvo.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtxautuvtj.html

PHP:  array_merge($a, $b);
来源：http://hz.fzhhl.top/gtffevvzef.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jlsjyb.cn/gtaaitcgij.html

TS:   [...a, ...b];
来源：http://hz.xinyue.icu/gthfppjbdt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenzaomai.com/gtsgcoelpy.html

Go:   append(a, b...)
来源：http://hz.yonumen.top/gthrmwplhz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sxryk.cn/gtaicvfhdm.html

C#:   a.Concat(b).ToList()
来源：http://hz.ppjwa.cn/gtnhkivbud.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtyqfkhprk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtiapsnqvb.html

PHP:  sort($arr);
来源：http://hz.316326.xyz/gtprruxvqx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cdnleiting.top/gtkcgtuzzx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtzeufsrdo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.dashuyun.cn/gtiixpxuqj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtqyzkcfqr.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtiedogvpn.html

C#:   list.Sort();
来源：http://hz.cucudq.cn/gtwbvrbita.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gthqwlfmaq.html


<!-- 参考信息 -->