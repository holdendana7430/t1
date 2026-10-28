代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gzhubu.top/gttkovyrgl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.iojbl.cn/gtluwyrcxw.html

[B07] while 循环
来源：http://hz.ywan-chungtsiang.top/gtfjmrhtdq.html

Py:   while i < 10: i += 1
来源：http://hz.daxiang520.top/gtjclqknnv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yanxiufei.cn/gtngclnewc.html

JS:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtnoqkfkeb.html

TS:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtvpsqmojk.html

Java: while (i < 10) { i++; }
来源：http://hz.zhengqikj.top/gthswxasyk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jiagoushi.top/gtatvkhkjh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xuetiantiany.cn/gtbghqmfgm.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtkalzougu.html

[B08] do-while（至少执行一次）
来源：http://hz.52xcode.cn/gtrlsflsvx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinqigfzy.top/gtmzvbbayg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hongshengwenyu.top/gtygxfzpgs.html

JS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtbtlwlouj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtdmznucyz.html

Java: do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gttrsixrrv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gotoacloud.top/gtiihylzzo.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hfpthk.cn/gtxpnnitsw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtlrqidmff.html

[B09] break 与 continue
来源：http://hz.guannengcc.top/gtlvxaksby.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.dashuyun.cn/gtopmwdqhy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258.top/gtbcznbhpb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gtuzvwtyci.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtodifxabr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtkhpgbhwd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shanyushiyangtech.top/gtxztjkbfg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhongyouzk.top/gtsbulsdou.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtxapbsvnv.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258.top/gtaxbmeaat.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dianchejie.cn/gtwhwbujhz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yongpay.top/gtldnbvpiu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.havefunace.top/gtbvvurynh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xylfe.cn/gtywkqnxgy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangtech.top/gtcuyovavl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.316326.xyz/gttudzbtrk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jianghu66.top/gtdxzrqzmk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ivvv.top/gtwydwaana.html

[B11] 生成数字序列 / 区间
来源：http://hz.xylfe.cn/gtoeeshtik.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtenrxbrbb.html

PHP:  range(0, 10, 2);
来源：http://hz.guowangkeji.top/gtbzaxtwqi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtybjhshih.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtdzidgvuc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xylfe.cn/gttziueygk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.9152youxi.cn/gtbfzliyzf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gtidcvsadi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj202588.top/gtastkaocl.html

[B12] 跳出多层循环
来源：http://hz.jinyuanbaomall.cn/gtdkevsvyi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.daxiang520.top/gtobvoawwn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shuidangran.top/gtvlzftljx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtcayymntw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtkelslpkn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.c1oappe.top/gtebpuadyt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangtech.top/gtsmmxxrqf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cheryme.top/gtjtthtccc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gtszpgknhs.html

[B13] 判断是否为数字
来源：http://hz.quarkkingdee.top/gtfheshiqm.html

Py:   isinstance(x, (int, float))
来源：http://hz.havefunace.top/gteccghuzi.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtbcrfrkwy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.kuanghao11.cn/gtcjrqxykw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtnhnhvymi.html

Java: x instanceof Number
来源：http://hz.tian-w.cn/gtanuhuwyi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tanke756.top/gtttlrpzrt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pycfn.com/gtajiwemkp.html

C#:   x is int or double or decimal
来源：http://hz.pycfn.com/gtinhkptwh.html

[B14] 判断值是否在集合内
来源：http://hz.nanxuanxn.top/gtzkwwmisv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yvedp.cn/gtlehxsrdw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgfzy.top/gtcjtibbda.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.9152youxi.cn/gtsxrzcvpr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yvedp.cn/gtkogttvsk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ydzc1.top/gtwahjomjk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tian-w.cn/gtecdqxuxb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sxryk.cn/gtkgoyyhoe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sysykeji.top/gtmamgeqec.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangtech.top/gtzucthumi.html

Py:   a and b or not c
来源：http://hz.ivvv.top/gtbxziogal.html

PHP:  $a && $b || !$c
来源：http://hz.cdnleiting.top/gtldtdfknh.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtzritlurb.html

TS:   a && b || !c
来源：http://hz.xylfe.cn/gtbggfbghi.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtkbtasuym.html

Go:   a && b || !c
来源：http://hz.sweek.top/gtpxfwwxuy.html

Ruby: a && b || !c
来源：http://hz.xziqi.cn/gtqfouomaq.html

C#:   a && b || !c
来源：http://hz.guannengcc.top/gtmdecfdde.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.dashuyun.cn/gtzndhivpi.html

Py:   if not data: return
来源：http://hz.sweek.top/gtndrelvla.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gtzqqjsznc.html

JS:   if (!data) return;
来源：http://hz.haohaochexian.top/gtzbikcjvw.html

TS:   if (!data) return;
来源：http://hz.gogol.net.cn/gtjvwwcqzp.html

Java: if (data == null) return;
来源：http://hz.cashguo.top/gtdxjzyubk.html

Go:   if data == nil { return }
来源：http://hz.cdnleiting.top/gtolbjbueb.html

Ruby: return if data.nil?
来源：http://hz.yanxiufei.cn/gtahktnhjo.html

C#:   if (data == null) return;
来源：http://hz.ivvv.top/gtwruhaiuk.html

================================================================================
来源：http://hz.xziqi.cn/gtohsbhrhh.html

C. 函数与作用域
来源：http://hz.svipenyu.cn/gtazgenbns.html

================================================================================
来源：http://hz.tianlin.xyz/gtkohswoqj.html

[C01] 定义函数
来源：http://hz.svipenyu.cn/gtlvxbjkfk.html

Py:   def add(a, b): return a + b
来源：http://hz.sufxvd.cn/gtwuolswvs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtndgwnejh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yangfankeji.com/gtospuhjil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtrhxvxuuc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtceqfooro.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ybcxt.top/gtujeozjwq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ydjk.org.cn/gtsnjzghwp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtzbuvlicm.html

[C02] 默认参数
来源：http://hz.pengpengdd.cyou/gtbodxbbwg.html

Py:   def greet(name="World"): return name
来源：http://hz.zhengqikj.top/gtzoljxiax.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cashguo.top/gtwooxgims.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenlongwang.top/gtindwiggp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtizeunkut.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinyuanbaomall.cn/gtjmgsrxmj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.birdmap.top/gtresmpmjo.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gtlqvardyu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dianchejie.cn/gtsmmjgnab.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtonynvyln.html

Py:   def total(*args): return sum(args)
来源：http://hz.bjfxy.top/gtgzxvkjos.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jyoumei.cn/gttphsqfqn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtvnkzmfiw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtmdfdramt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zycfv.cn/gtxhefhgef.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xylfe.cn/gtxswqjwbn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.mhx1999.top/gtsspuduvr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hongshengwenyu.top/gtmhjdpysm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtbvlablkn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fengsongda.top/gtohurwkvz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gaohongyu789.top/gtnvwhmmui.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ydjk.org.cn/gtmdfkxvyk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yongpay.top/gtklwktnqq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pycfn.com/gttendeynr.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gtovpiojxa.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtkmzhvjgc.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtxqoqtajv.html

[C05] 返回多个值
来源：http://hz.9152youxi.cn/gtcivjixru.html

Py:   return a, b
来源：http://hz.cashguo.top/gtkjfimqov.html

PHP:  return [$a, $b];
来源：http://hz.kuanghao11.cn/gtbkffvjxn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhongyouzk.top/gtddtwkpzs.html

TS:   return { a, b };
来源：http://hz.zhengqikj.top/gtlahgawyy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ybcxt.top/gtvdugmzyo.html

Go:   return a, b
来源：http://hz.jqgufenzy.top/gtmsjmclrm.html

Ruby: return a, b
来源：http://hz.hnqzz.top/gtlawpoaec.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xingfuxueyuan.xyz/gtuocllxfk.html

[C06] 匿名函数 / lambda
来源：http://hz.guannengcc.top/gtsdyxlajf.html

Py:   square = lambda x: x * x
来源：http://hz.zhiwuduotai.top/gtvtytdieh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.mhx1999.top/gturvqjpyo.html

JS:   const square = x => x * x;
来源：http://hz.gaohongyu789.top/gtlyictagc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.bjfxy.top/gtylmqslsx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hysaishi.cn/gtsbfonrsy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xinyue.icu/gtcttfeaji.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangdashe.top/gtwegjucxh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuxming.cn/gtnoioefma.html

[C07] 把函数作为参数传入
来源：http://hz.yangfankeji.com/gthdsasawh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sxryk.cn/gthrypvegi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuetiantiany.cn/gttydxftki.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinyuanbaomall.cn/gtftrskfzd.html

TS:   arr.map(String)
来源：http://hz.ivvv.top/gtotwhtfkm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jianghu66.top/gtoyfzletg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtrbskgaid.html

Ruby: arr.map(&:upcase)
来源：http://hz.mhx1999.top/gttrwhmqwd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhixingplan.top/gtdwczdfkm.html

[C08] 闭包
来源：http://hz.pengpengdd.cyou/gtihfltbcz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtjekfqsvx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gtedzpjejp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtzsmcdona.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtdqdfxwzo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtapxsjpcf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gotoacloud.top/gtfxiqnxak.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.haohaochexian.top/gtleyjsydr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtnoarzswl.html

[C09] 递归
来源：http://hz.cucudq.cn/gtcbdufnxn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hongshengwenyu.top/gtcuolfpvt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtmejuubuj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgufenzy.top/gtatwvielj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gtpvwsgpqq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yvedp.cn/gtvkbihmhw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gtrfxwzzuk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.haohaochexian.top/gtfkqyfmmr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yuanzhike.top/gtkiypmrcj.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtxzowdnkb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigfzy.top/gtsdmmqwcm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.smart0.xyz/gtxrwhgrfq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cqqwz.cn/gtcsyimugj.html

TS:   同 JS
来源：http://hz.zhengqikj.top/gtuawzksvi.html

Java: 方法内为块级作用域
来源：http://hz.shuidangran.top/gtolxsmemh.html

Go:   花括号块级作用域
来源：http://hz.yonumen.top/gtwuewuzwy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnqzz.top/gthcxpjiye.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtvfoxlyrb.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtawvcludg.html

Py:   from module import func
来源：http://hz.quarkkingdee.top/gtrimeevnf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhaomingkeji.xyz/gtxatdtkrx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtvvehysrz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtvakwaclj.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtmopyslzi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.smart0.xyz/gtbqxtwctf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cqqwz.cn/gtofehdpva.html

C#:   using System.Text;
来源：http://hz.jinghuilouyu.cn/gtvbtfubge.html

[C12] 立即执行函数 IIFE
来源：http://hz.sysykeji.top/gticsmxjvh.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigufen.top/gtbqzbwrjr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangdashe.top/gtfmntzeyq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtuyehgbwc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtikwdudra.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.vqdsnc.cn/gthlgvpwat.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.andypj.xyz/gtcwfheyze.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuetiantiany.cn/gtyvzfpoou.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.haohaochexian.top/gtvttzaxap.html

[C13] 类型声明 / 类型注解
来源：http://hz.jyoumei.cn/gtazvrejtw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtbkhrblis.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtjybfvwcm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtdsozkvqz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtaedefqfl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gtuowknmau.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gtkmxflvlp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cashguo.top/gtxdzyadry.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gtzdwfynlj.html

[C14] 泛型函数
来源：http://hz.jqgufenzy.top/gtqjczfwgx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.vqdsnc.cn/gtukdadtne.html

PHP:  // 无泛型
来源：http://hz.xziqi.cn/gtwsbfaodk.html

JS:   // 无泛型
来源：http://hz.yangfankeji.com/gtthodbvli.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gtxcuyahvu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dianchejie.cn/gtjrqvrumz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yvedp.cn/gtonkmabse.html

Ruby: # 无泛型
来源：http://hz.daria6918.cn/gtxnuusfvr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtrjbaukdg.html

[C15] 解构 / 展开参数
来源：http://hz.zhixingplan.top/gtezuisewt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangdashe.top/gttwpwokth.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zycfv.cn/gtodtztizx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtcbfbpdcy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtunvvzkrm.html

Java: // 无解构
来源：http://hz.yangfankeji.com/gtgyflkruv.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gtzwksgkfj.html

Ruby: a, b = pair
来源：http://hz.havefunace.top/gtszfsznav.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangtech.top/gtcaowvdkk.html

[C16] 函数 / 方法重载
来源：http://hz.hnqzz.top/gtoansmqub.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xinyue.icu/gtjyiachwr.html

PHP:  // 无重载
来源：http://hz.sysykeji.top/gtefzdppii.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhaomingkeji.xyz/gtbkwkxnuz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgufenzy.top/gtymxtnhhb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtzuevbohw.html

Go:   // 无重载：用不同函数名
来源：http://hz.quarkkingdee.top/gtkxmotgwc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtiibnwlre.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gaohongyu789.top/gtvbjnwdvl.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtovnphhxr.html

D. 数组 / 列表 / 集合
来源：http://hz.shanyushiyangkeji.top/gtkrjndvno.html

================================================================================
来源：http://hz.yangfankeji.com/gtosrhonne.html

[D01] 创建数组 / 列表
来源：http://hz.guannengcc.top/gtwewysinf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hfpthk.cn/gtapjlymqv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhongyouzk.top/gtddbljrqh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.smart0.xyz/gtoimoqvsf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daria6918.cn/gtwlsbtium.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gthgaipifc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtvymwmuiz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.fengsongda.top/gtougeclym.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hnqzz.top/gtrgtgyjua.html

[D02] 追加元素到末尾
来源：http://hz.gogol.net.cn/gtybcezqqs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tian-w.cn/gteriswnun.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tianlin.xyz/gtzfvvhtqo.html

JS:   arr.push(4);
来源：http://hz.yj20258888.top/gtycqhsgck.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtmsluamsl.html

Java: list.add(4);
来源：http://hz.cheryme.top/gthqbqauis.html

Go:   arr = append(arr, 4)
来源：http://hz.yongpay.top/gtrdzcynmc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtbowxgmmc.html

C#:   list.Add(4);
来源：http://hz.gotoacloud.top/gtdvzvnbuw.html

[D03] 在指定位置插入元素
来源：http://hz.aizwys.cn/gtvusefytl.html

Py:   arr.insert(0, 0)
来源：http://hz.xinyue.icu/gtpmkvegub.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yanxiufei.cn/gtlokhovfl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtzskmsvjs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtvzypnaoc.html

Java: list.add(0, 0);
来源：http://hz.wangshuangyany.cn/gtnlmyhcrt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhaomingkeji.xyz/gtfinvztmw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.redwolf501.top/gtihixfmhg.html

C#:   list.Insert(0, 0);
来源：http://hz.ppjwa.cn/gtbmguvlqv.html

[D04] 删除元素
来源：http://hz.jinyuanbaomall.cn/gtxivaoggi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtgscbseye.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gtdyojtmzd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cheryme.top/gtmfjqpxsx.html

TS:   arr.splice(0, 1);
来源：http://hz.snrcjt.cn/gtarljbqaw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.smart0.xyz/gtgxpnosuj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.meibo888.top/gtqqcvbqzy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ehwqpu.com/gtzqjergjs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtkgdxnjsa.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtphrylvsb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtznafikdp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtxtwfqzmx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.c1oappe.top/gttkyzofqj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ivvv.top/gthjtdkext.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hysaishi.cn/gtamdplcco.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258888.top/gtqemprzxc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtmvaxhftp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtcrlszgjb.html

[D06] 数组长度
来源：http://hz.aizwys.cn/gtevkwxbmx.html

Py:   len(arr)
来源：http://hz.yj202588.top/gtecbdajeq.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtqqenfhtk.html

JS:   arr.length
来源：http://hz.haohaochexian.top/gtbgqvtibf.html

TS:   arr.length
来源：http://hz.nwbrower.top/gtjyzuvcax.html

Java: list.size();
来源：http://hz.tian-w.cn/gtzjhgkydi.html

Go:   len(arr)
来源：http://hz.ehwqpu.com/gtkvbenigx.html

Ruby: arr.length; arr.size
来源：http://hz.dianchejie.cn/gtgfdxnjzu.html

C#:   list.Count;
来源：http://hz.cqqwz.cn/gtqvnuulfb.html

[D07] 切片 / 取子数组
来源：http://hz.pengpengdd.cyou/gtbhrytnxz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhaomingkeji.xyz/gtdsxgtbqs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhongyouzk.top/gtcfqsbenq.html

JS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtraqcatuz.html


<!-- 参考信息 -->