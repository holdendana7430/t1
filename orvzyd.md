代发 wailian999

[B09] break 与 continue
来源：http://hz.fzhhl.top/gtoizokpsq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hammf.cn/gtrkcbplaa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cucudq.cn/gtfkamcgkm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtchaujgqt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtqpiflthb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtcmxqcyvf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigfzy.top/gtfghyypme.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jianghu66.top/gtfukomgpq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtwhhuoaxk.html

[B10] 遍历同时拿索引
来源：http://hz.zycfv.cn/gtgjozrouw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nanxinkj.top/gttuoxtnkn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj20258888.top/gtinoogfau.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gogol.net.cn/gtyxmmrxbn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenzaomai.com/gtpfecpwvx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fengsongda.top/gtgnujnvpk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.birdmap.top/gtybepedwo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hysaishi.cn/gtiowrmflz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gzhubu.top/gtswikwqmj.html

[B11] 生成数字序列 / 区间
来源：http://hz.shuidangran.top/gtysvlrisw.html

Py:   list(range(0, 10, 2))
来源：http://hz.quarkkingdee.top/gtprhkqyye.html

PHP:  range(0, 10, 2);
来源：http://hz.zhongyouzk.top/gtwkopsxsb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cheryme.top/gtmkfcoxwg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtikkkfcrd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.vqdsnc.cn/gthhisgbgb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.316326.xyz/gtouzisppb.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sxryk.cn/gtkkjuqbnm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ybcxt.top/gtttuvlvaj.html

[B12] 跳出多层循环
来源：http://hz.gaohongyu789.top/gthhddjgsd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhaomingkeji.xyz/gtazswvpjt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuxming.cn/gthfqqlofe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gthuxznzzn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.mhx1999.top/gtzxbbekwy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtpzqrqvly.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtgcitijeh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ehwqpu.com/gtyubuelqk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.pycfn.com/gtyxeegnhc.html

[B13] 判断是否为数字
来源：http://hz.yanxiufei.cn/gthxrivqac.html

Py:   isinstance(x, (int, float))
来源：http://hz.andypj.xyz/gtibqmdbrt.html

PHP:  is_numeric($x)
来源：http://hz.xinyue.icu/gtdkksicqv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtoeftefal.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxinkj.top/gtzesnavjz.html

Java: x instanceof Number
来源：http://hz.c1oappe.top/gtmpmyqyik.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jlsjyb.cn/gtpleqbvva.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenzaomai.com/gtnakrvzja.html

C#:   x is int or double or decimal
来源：http://hz.yangfankeji.com/gtjsfypbnv.html

[B14] 判断值是否在集合内
来源：http://hz.yj20258888.top/gtjywfvigs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gzhubu.top/gtafnzdzxq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hysaishi.cn/gtfqyfpvoa.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cqqwz.cn/gtukhkjfcq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtvflfltbo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtxznkhhip.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.havefunace.top/gtpstkckvd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhongyouzk.top/gtqrngunlu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cashguo.top/gtbgqhsabb.html

[B15] 布尔运算与取反
来源：http://hz.tian-w.cn/gtwryfgjun.html

Py:   a and b or not c
来源：http://hz.daxiang520.top/gtvvqrivuk.html

PHP:  $a && $b || !$c
来源：http://hz.dianchejie.cn/gtheprxaql.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtscazpqid.html

TS:   a && b || !c
来源：http://hz.aizwys.cn/gtpbvlqtff.html

Java: a && b || !c
来源：http://hz.hfpthk.cn/gtjloxhdur.html

Go:   a && b || !c
来源：http://hz.zhengqikj.top/gtrqveizeo.html

Ruby: a && b || !c
来源：http://hz.yangfankeji.com/gtlqdbeneg.html

C#:   a && b || !c
来源：http://hz.nanxuanxn.top/gtlyyggzgc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhixingplan.top/gtvuubeqsp.html

Py:   if not data: return
来源：http://hz.kuanghao11.cn/gtjvltkwjv.html

PHP:  if (!$data) { return; }
来源：http://hz.andypj.xyz/gtxjardyla.html

JS:   if (!data) return;
来源：http://hz.ybcxt.top/gtueqpsecv.html

TS:   if (!data) return;
来源：http://hz.yonumen.top/gtlfmyvcht.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtueqhnsfe.html

Go:   if data == nil { return }
来源：http://hz.jinqigufen.top/gtvmuhpzwx.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangkeji.top/gtxfeezqvm.html

C#:   if (data == null) return;
来源：http://hz.yonumen.top/gtafpsrsnj.html

================================================================================
来源：http://hz.snrcjt.cn/gtrhrukolp.html

C. 函数与作用域
来源：http://hz.hnqzz.top/gtxspqtyis.html

================================================================================
来源：http://hz.jianghu66.top/gtibjvdzgs.html

[C01] 定义函数
来源：http://hz.kuanghao11.cn/gtngzqlxro.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtvkerubkx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtuepeeryu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zdqjudy.top/gtvdefrdut.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtwqyrjzkt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtjjywxvrn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ehwqpu.com/gtwcccdubr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tian-w.cn/gtfapkkwct.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtrjzdszgj.html

[C02] 默认参数
来源：http://hz.bjfxy.top/gtemqpoolp.html

Py:   def greet(name="World"): return name
来源：http://hz.gogol.net.cn/gtzgchbran.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guowangkeji.top/gthvgguzhp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yuanzhike.top/gtmhrwgtkt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gtzzjqqkgc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xinyue.icu/gtusqpozmy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ivvv.top/gtzdnpomcd.html

Ruby: def greet(name = "World") = name
来源：http://hz.fzhhl.top/gtnslrnebr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.c1oappe.top/gtwxxlpleg.html

[C03] 可变参数
来源：http://hz.shzxlz.cn/gtveiygvxa.html

Py:   def total(*args): return sum(args)
来源：http://hz.jqgufenzy.top/gtbgdlmrhd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.quarkkingdee.top/gtmolwvger.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydzc1.top/gteagmhrgm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtovveeuze.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cashguo.top/gtusgnqzso.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtnfqzcvfg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cheryme.top/gthqvauuwm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gterlqxizb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.guowangkeji.top/gtwpmwsmhq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenzaomai.com/gtedpdocmi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hongshengwenyu.top/gtjylhazrq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pycfn.com/gtxluvnxrn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258.top/gtjzxrrkmk.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daxiang520.top/gtghghkqbb.html

Go:   // 无：用配置结构体参数
来源：http://hz.jqgufenzy.top/gtoicpddsx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtmwgpfuwe.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtebyypnck.html

[C05] 返回多个值
来源：http://hz.andypj.xyz/gtvhwaksdo.html

Py:   return a, b
来源：http://hz.hammf.cn/gtjqsxlquv.html

PHP:  return [$a, $b];
来源：http://hz.aizwys.cn/gtwkuahwji.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtaqelvdrx.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtztuamraq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.meibo888.top/gtqohcwwuh.html

Go:   return a, b
来源：http://hz.svipenyu.cn/gtgprrodib.html

Ruby: return a, b
来源：http://hz.nanxinkj.top/gtvwdtujht.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yonumen.top/gtduhxothq.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgfzy.top/gtjlotowil.html

Py:   square = lambda x: x * x
来源：http://hz.ppjwa.cn/gtnsfvdeju.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtgdtkroew.html

JS:   const square = x => x * x;
来源：http://hz.zhixingplan.top/gtrdkvscve.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ivvv.top/gtofvhxjjh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pycfn.com/gtirtrktyc.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.52xcode.cn/gtymwtujwv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj20258888.top/gtqxchtifi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhiwuduotai.top/gtrrropzyj.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtzrwqjamb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.c1oappe.top/gtyjjuxrdn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yangfankeji.com/gtkslmlyng.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.redwolf501.top/gtigpqguzl.html

TS:   arr.map(String)
来源：http://hz.svipenyu.cn/gtkxlnhksa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhaomingkeji.xyz/gtguitygbm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sufxvd.cn/gttlwmxdaz.html

Ruby: arr.map(&:upcase)
来源：http://hz.nwbrower.top/gtwvcrwlxi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yonumen.top/gtmjyombwo.html

[C08] 闭包
来源：http://hz.cucudq.cn/gtdkayyckp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnqzz.top/gtzplyjfzm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hammf.cn/gtfgeldfyp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtdzytlthz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gttjavujqt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhijiandao.cn/gtgezlnkuy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yvedp.cn/gtakdwxrfb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.52xcode.cn/gtpnmpfafp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtqdwgaxgg.html

[C09] 递归
来源：http://hz.9152youxi.cn/gtzncgvfkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ivvv.top/gtkfppxzaj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yueranfly.top/gtejczxhnx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgufenzy.top/gtefjbezep.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtbzghppdz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydjk.org.cn/gtdoeilouh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.andypj.xyz/gtohekqgmh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.haohaochexian.top/gtxeljxidr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhiwuduotai.top/gtghdqybkf.html

[C10] 变量作用域
来源：http://hz.zhaomingkeji.xyz/gtsgvyoasv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuetiantiany.cn/gtjwlhmxju.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.havefunace.top/gtfvudiebv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinghuilouyu.cn/gttoxzuaqz.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtuwhwrdvu.html

Java: 方法内为块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtsoyzadlg.html

Go:   花括号块级作用域
来源：http://hz.pycfn.com/gtptbmiwxg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenjidiqi.icu/gttfqwwfkw.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtywndgqlv.html

[C11] 模块导入与导出
来源：http://hz.316326.xyz/gtqvkzgksz.html

Py:   from module import func
来源：http://hz.zhijiandao.cn/gtwlvqrmoc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aibaodan.cn/gtygyvkdak.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtrfwotjhx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgfzy.top/gtcndsqtoh.html

Java: import java.util.List;
来源：http://hz.iojbl.cn/gtdsjwqkot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258.top/gtuuxjxplc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shanyushiyangtech.top/gtrkpcrmyo.html

C#:   using System.Text;
来源：http://hz.snrcjt.cn/gtodcgfrtq.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gtyqqpgzad.html

Py:   (lambda: print("run"))()
来源：http://hz.xylfe.cn/gtwzmqvclw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.svipenyu.cn/gtqlmesjcv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtvpejkvqa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtgnanztei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yanxiufei.cn/gtjwhqosvd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtmscenrfs.html

Ruby: -> { puts "run" }.call
来源：http://hz.tanke756.top/gtqbhnuhuu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guowangkeji.top/gtbbyyyrxi.html

[C13] 类型声明 / 类型注解
来源：http://hz.jyoumei.cn/gtatpjmqca.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ppjwa.cn/gttvjshpha.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtdoldwghx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtclorujrq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtssqbocmg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtpfwqxqwa.html

Go:   func add(a, b int) int
来源：http://hz.fengsongda.top/gtvmzdgxgd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.quarkkingdee.top/gtzxdymqmn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guannengcc.top/gtudfwwtnb.html

[C14] 泛型函数
来源：http://hz.cdnleiting.top/gtmswfomcv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtzzosksmm.html

PHP:  // 无泛型
来源：http://hz.zhijiandao.cn/gteswervii.html

JS:   // 无泛型
来源：http://hz.jqgfzy.top/gtluxyampn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtrrxeyklm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.havefunace.top/gtilbcgucw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sxryk.cn/gtkkxdolxr.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtqdfjldka.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtpoixjjqb.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gtjbmzadcg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuanzx.com/gtxqdanqkg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtddklmpzj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.0kj1m.cn/gtvnjechjo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtyxsjanxf.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtxjwtywqy.html

Go:   // 无解构
来源：http://hz.nanxuanxn.top/gtxssgdqnt.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtceawvknb.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtrzohkgzp.html

[C16] 函数 / 方法重载
来源：http://hz.jqgfzy.top/gtxjbezslp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jyoumei.cn/gtzslfibig.html

PHP:  // 无重载
来源：http://hz.shuidangran.top/gtjogjnlxh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinghuilouyu.cn/gtftcmtgty.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangkeji.top/gtbvvkdzcj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtzmukdbck.html

Go:   // 无重载：用不同函数名
来源：http://hz.shzxlz.cn/gtihfvvref.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yonumen.top/gtrkbbfqja.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.9152youxi.cn/gtyiahrffe.html

================================================================================
来源：http://hz.c1oappe.top/gtitcxullr.html

D. 数组 / 列表 / 集合
来源：http://hz.hnqzz.top/gtybweiaoq.html

================================================================================
来源：http://hz.tanke756.top/gtzwywaumn.html

[D01] 创建数组 / 列表
来源：http://hz.hongshengwenyu.top/gtrexscykp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.smart0.xyz/gtqaiwbxll.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtevfumswd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenzaomai.com/gturhprdyr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangshuangyany.cn/gtixrmtdjv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gtoigrnsem.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258.top/gtrlgewzbt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hysaishi.cn/gtnsjmxnfv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gttnftimlr.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtthlwkokg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fzhhl.top/gtddwufhlj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guowangkeji.top/gtitshqymm.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gtwwelpftz.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtflcorsdf.html

Java: list.add(4);
来源：http://hz.9152youxi.cn/gtoltxhkyd.html

Go:   arr = append(arr, 4)
来源：http://hz.redwolf501.top/gtrfpkqexv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.vqdsnc.cn/gtxaauntyd.html

C#:   list.Add(4);
来源：http://hz.sufxvd.cn/gtjwxuxmqj.html

[D03] 在指定位置插入元素
来源：http://hz.hfpthk.cn/gtgkohnlta.html

Py:   arr.insert(0, 0)
来源：http://hz.zhaomingkeji.xyz/gtxqbixcxx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuxming.cn/gtaijakosa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shuidangran.top/gtddhledgi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.316326.xyz/gtqygeiuhi.html

Java: list.add(0, 0);
来源：http://hz.yvedp.cn/gtydkwwfdo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cheryme.top/gtnmwgypyq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ppjwa.cn/gtmflbcjbu.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtlnuaztcq.html

[D04] 删除元素
来源：http://hz.hnxiangtu.top/gtalahwdvi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtdufpiycz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtflierxxg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ivvv.top/gtdfqczjtm.html

TS:   arr.splice(0, 1);
来源：http://hz.fengsongda.top/gtmsnzsydq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtymilksix.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yanxiufei.cn/gtqeavycbt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhengqikj.top/gtujgjnskh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtsraxlbbw.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gtocectqwi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gthtvdhncc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.haohaochexian.top/gtcqdfzlki.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gtjyydgsck.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nwbrower.top/gtjcasmfaa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnqzz.top/gtfhugrlbi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtwhxqxkmd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtrmbovgna.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sweek.top/gtgevidzsd.html

[D06] 数组长度
来源：http://hz.vqdsnc.cn/gtmczgzxsd.html

Py:   len(arr)
来源：http://hz.jinqigfzy.top/gtpddabxam.html

PHP:  count($arr);
来源：http://hz.daria6918.cn/gtaetdgmlj.html

JS:   arr.length
来源：http://hz.wangdashe.top/gtkktuddud.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gtsmsvsgdr.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtutenmbvj.html

Go:   len(arr)
来源：http://hz.feifeiyinyue.top/gtxfmocmdo.html

Ruby: arr.length; arr.size
来源：http://hz.zhoulong.xyz/gtseyvmoeg.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtnyetuvju.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gtrnmuckjj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnqzz.top/gtyjctszkq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtntmpfqax.html

JS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtpbwxuntz.html

TS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtvxrogwvu.html

Java: list.subList(1, 4);
来源：http://hz.ppjwa.cn/gtldzvzvtp.html

Go:   arr[1:4]
来源：http://hz.xylfe.cn/gtndpyrbac.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangtech.top/gtwymiutct.html

C#:   list.GetRange(1, 3);
来源：http://hz.vqdsnc.cn/gtznipukuh.html

[D08] 合并两个数组
来源：http://hz.nwbrower.top/gttekpatll.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtbicppkkc.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gtxnexsrbx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gtitkanzoe.html

TS:   [...a, ...b];
来源：http://hz.zhijiandao.cn/gtqjrvtdij.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sysykeji.top/gtprwrerdw.html

Go:   append(a, b...)
来源：http://hz.sxryk.cn/gtimxfaixx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gtxnixtoqz.html

C#:   a.Concat(b).ToList()
来源：http://hz.c1oappe.top/gttoomwwtl.html

[D09] 排序（升序）
来源：http://hz.xuetiantiany.cn/gtkwybwioz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtctvftzza.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtcarthcqq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yonumen.top/gttijlccze.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gtfiljtlud.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tianlin.xyz/gtpgapmqrb.html


<!-- 参考信息 -->