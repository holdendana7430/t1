代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.ybcxt.top/gtbumqdmbe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gteboxmujl.html

JS:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtheykdfzm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtyvpvkjsf.html

Java: do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtsiqctiek.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jqgfzy.top/gtrnoxsnkt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ydjk.org.cn/gtlfkqgmcs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtykyaeegj.html

[B09] break 与 continue
来源：http://hz.yj20258.top/gtqqtitmts.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.c1oappe.top/gttijzarny.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cqqwz.cn/gtvbcowawm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtfrnpzmyz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtlecbgbhe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtmdogidkp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtcqogvovv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cucudq.cn/gtniokrrgr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtirhqtnno.html

[B10] 遍历同时拿索引
来源：http://hz.zhongyouzk.top/gtcgtryvnb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sxryk.cn/gtqfojrznt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenlongwang.top/gtadmcjjji.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daria6918.cn/gtllzucrov.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtkdsksfxq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.meibo888.top/gtybzvhcyn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guowangkeji.top/gtjishmnxb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tanke756.top/gtwclswmny.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.bjfxy.top/gtgliclhmb.html

[B11] 生成数字序列 / 区间
来源：http://hz.gzhubu.top/gtzhvsyrwc.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhoulong.xyz/gtzqsdrjzl.html

PHP:  range(0, 10, 2);
来源：http://hz.sysykeji.top/gtadsmmfwb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtonrzkybw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgufenzy.top/gtlvndxxld.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aibaodan.cn/gtewiwsstm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.snrcjt.cn/gtiytjxkce.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yangfankeji.com/gtmjxcpblb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgfzy.top/gtufkkjecy.html

[B12] 跳出多层循环
来源：http://hz.sufxvd.cn/gtxygaudhk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pengpengdd.cyou/gtxmsoogck.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dashuyun.cn/gtteeiimqk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtvuvqcnes.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gturhsyrhd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj202588.top/gtsswmsasn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.pycfn.com/gtcksflsyf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.9152youxi.cn/gtsjfhspgu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.dashuyun.cn/gtkjygvrcx.html

[B13] 判断是否为数字
来源：http://hz.haohaochexian.top/gtpcrmkrng.html

Py:   isinstance(x, (int, float))
来源：http://hz.iojbl.cn/gtiqfqtegs.html

PHP:  is_numeric($x)
来源：http://hz.zhixingplan.top/gtdtniwdmb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtomkdlvqr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gturydlgkt.html

Java: x instanceof Number
来源：http://hz.ybcxt.top/gtjxvxwpqr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.c1oappe.top/gtukslvqks.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangkeji.top/gtjdkcvlhw.html

C#:   x is int or double or decimal
来源：http://hz.hywenlv.cn/gtptzbccjl.html

[B14] 判断值是否在集合内
来源：http://hz.yonumen.top/gtaqjdpvty.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.52xcode.cn/gteowqhftj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hnxiangtu.top/gtcskjqoez.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.bjfxy.top/gtggyjdvvy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cqqwz.cn/gtxezhnqpv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xuetiantiany.cn/gttravocmp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daxiang520.top/gtigkfcssw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zycfv.cn/gtcuddmucw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hfpthk.cn/gtehircezf.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gtcuvofqim.html

Py:   a and b or not c
来源：http://hz.cashguo.top/gtqbznfept.html

PHP:  $a && $b || !$c
来源：http://hz.ppjwa.cn/gtniqrviwq.html

JS:   a && b || !c
来源：http://hz.shzxlz.cn/gtqbfpyysi.html

TS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtrmcqnotb.html

Java: a && b || !c
来源：http://hz.gogol.net.cn/gtzktiwoee.html

Go:   a && b || !c
来源：http://hz.dashuyun.cn/gtpayriaqi.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtjmwarici.html

C#:   a && b || !c
来源：http://hz.yj202588.top/gtoufmwefr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shzxlz.cn/gtmojoqkjo.html

Py:   if not data: return
来源：http://hz.zhixingplan.top/gtdgwcmhzd.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigufen.top/gtdgtquxys.html

JS:   if (!data) return;
来源：http://hz.yonumen.top/gtlzbqklhq.html

TS:   if (!data) return;
来源：http://hz.ydzc1.top/gtozwgbxpq.html

Java: if (data == null) return;
来源：http://hz.fengsongda.top/gtlnqaahbf.html

Go:   if data == nil { return }
来源：http://hz.yj20258888.top/gtaduyqmyq.html

Ruby: return if data.nil?
来源：http://hz.shuidangran.top/gtyatogvku.html

C#:   if (data == null) return;
来源：http://hz.xuanzx.com/gtjkdqmjhg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtmdompbjr.html

C. 函数与作用域
来源：http://hz.cashguo.top/gtwjjitzfi.html

================================================================================
来源：http://hz.hysaishi.cn/gtlemdxtpl.html

[C01] 定义函数
来源：http://hz.yuanzhike.top/gtptumoxuq.html

Py:   def add(a, b): return a + b
来源：http://hz.pycfn.com/gtrimveyzl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtykeiadpl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtpfigsggs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtcwpfpkwe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtkarmpmtg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.9152youxi.cn/gtngspjjwe.html

Ruby: def add(a, b); a + b; end
来源：http://hz.quarkkingdee.top/gtxsmybsng.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtznrovrst.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtgxdlsuti.html

Py:   def greet(name="World"): return name
来源：http://hz.zycfv.cn/gtknsofatk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.wangdashe.top/gtryplldrv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtgjymejjh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.havefunace.top/gtjkznnzhd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinyuanbaomall.cn/gtmqvtlopb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgfzy.top/gtjodwtpej.html

Ruby: def greet(name = "World") = name
来源：http://hz.pycfn.com/gtrmxhlsqj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gtypniumda.html

[C03] 可变参数
来源：http://hz.pycfn.com/gtmbtfapmr.html

Py:   def total(*args): return sum(args)
来源：http://hz.hongshengwenyu.top/gtllkqwxek.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnxiangtu.top/gtbamunffk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtruwdxzlo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtlpqgtuej.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ybcxt.top/gtfduhuhns.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.vqdsnc.cn/gtnyfddbwe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.quarkkingdee.top/gtrludarks.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zdqjudy.top/gtzdboqtlx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sweek.top/gtjtyfeirq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenjidiqi.icu/gtopuaihqa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xingfuxueyuan.xyz/gtxybxhknc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.redwolf501.top/gttspuuhgr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sweek.top/gtbgmbcyta.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sxryk.cn/gtqwwmbbpo.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhengqikj.top/gtuszlnmlv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtrgaizleh.html

C#:   f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtjtkijwkr.html

[C05] 返回多个值
来源：http://hz.jianghu66.top/gtxnuugelh.html

Py:   return a, b
来源：http://hz.zhoulong.xyz/gthasbpgqm.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtjkvjdzas.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hfpthk.cn/gtyfmgszud.html

TS:   return { a, b };
来源：http://hz.yonumen.top/gtpsjluwkz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinqigfzy.top/gtddanxlvn.html

Go:   return a, b
来源：http://hz.xziqi.cn/gtimdbumwc.html

Ruby: return a, b
来源：http://hz.xingfuxueyuan.xyz/gtrbrqdhia.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.fzhhl.top/gtigfhqvuu.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigfzy.top/gthgbrnmnk.html

Py:   square = lambda x: x * x
来源：http://hz.tianlin.xyz/gtfdltfncj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guannengcc.top/gtyzkkvfcs.html

JS:   const square = x => x * x;
来源：http://hz.zycfv.cn/gtzfqtvhlg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gtoiqhahju.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.fzhhl.top/gtdrnfckmr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fengsongda.top/gtkrhdtkim.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenjidiqi.icu/gtsbeuwilh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.smart0.xyz/gtdvsiwoyq.html

[C07] 把函数作为参数传入
来源：http://hz.xziqi.cn/gtvqccxcem.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hywenlv.cn/gteyjzqlzn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtxhljjomu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuanzx.com/gtgutfggfg.html

TS:   arr.map(String)
来源：http://hz.jinqigfzy.top/gtzvmxverw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnqzz.top/gtnvcugnso.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigufen.top/gtpisamvwt.html

Ruby: arr.map(&:upcase)
来源：http://hz.gzhubu.top/gtsuqvylfl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hysaishi.cn/gtscxnqyna.html

[C08] 闭包
来源：http://hz.yvedp.cn/gtkxscvrjm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxinkj.top/gtvsolprff.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.daxiang520.top/gtoscxlkjj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtrgdduxor.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtgseyevcn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.feifeiyinyue.top/gtxwokrfvu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.feifeiyinyue.top/gtzkoywpjj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtuzuruxmv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtvhserwwn.html

[C09] 递归
来源：http://hz.tianlin.xyz/gthirlyvot.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtvimmvukq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xziqi.cn/gtwampkxsd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gteohkmrcf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhongyouzk.top/gttlrnikii.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ivvv.top/gtyspybiat.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhoulong.xyz/gtzywvdkps.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtfairvjim.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ivvv.top/gtuodungpa.html

[C10] 变量作用域
来源：http://hz.dashuyun.cn/gtzivsrsos.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hammf.cn/gtzfmwksfe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgfzy.top/gtnjtevpit.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jianghu66.top/gtngmcizql.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtkudkyazs.html

Java: 方法内为块级作用域
来源：http://hz.mhx1999.top/gtwjilgxhv.html

Go:   花括号块级作用域
来源：http://hz.guowangkeji.top/gtwgexsimi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtezghrozi.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtthpckofk.html

[C11] 模块导入与导出
来源：http://hz.jqgfzy.top/gtomjuqlqg.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gtdngoikdq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.svipenyu.cn/gtpjghwlgp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.birdmap.top/gttkknrzyi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hfpthk.cn/gtvrpniizm.html

Java: import java.util.List;
来源：http://hz.sysykeji.top/gtmptrmwtg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.havefunace.top/gtvruzskhh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhongyouzk.top/gtocprxyru.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtwnvbiikm.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtnfhxrxqi.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtphxajjru.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gogol.net.cn/gtgjlylkvm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtrdfndfnj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gthcnsqfyc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gaohongyu789.top/gtpxfxleoy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ppjwa.cn/gthkfczrbk.html

Ruby: -> { puts "run" }.call
来源：http://hz.jyoumei.cn/gtvhnvrssk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gtfoofqnfg.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258888.top/gtywewmavy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhoulong.xyz/gtmhyfbvrg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtkzpcpblj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxinkj.top/gtlbrlzmxh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtahddjcty.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtgoezpaad.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtgbpamuer.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhixingplan.top/gteankneul.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ppjwa.cn/gtefxlzxtn.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gtooaudlur.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yueranfly.top/gtkrhbskjn.html

PHP:  // 无泛型
来源：http://hz.gogol.net.cn/gtwrukwmjx.html

JS:   // 无泛型
来源：http://hz.feifeiyinyue.top/gtxrqutmul.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gtmnspzmnx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.c1oappe.top/gtwuaxayjq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnxiangtu.top/gtlezlzqir.html

Ruby: # 无泛型
来源：http://hz.yj20258888.top/gtnwlzejnr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinghuilouyu.cn/gttwnuqxyk.html

[C15] 解构 / 展开参数
来源：http://hz.yangfankeji.com/gtivjbsdsz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.9152youxi.cn/gtbavyfogw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtegittdfl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tanke756.top/gtevkhekfo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangdashe.top/gtebixncmd.html

Java: // 无解构
来源：http://hz.jinghuilouyu.cn/gtsorinhgm.html

Go:   // 无解构
来源：http://hz.cucudq.cn/gtbtvxdzvs.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtsbsoqpkl.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gtfsnknang.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtwpytmnqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cqqwz.cn/gtixwwiytv.html

PHP:  // 无重载
来源：http://hz.cheryme.top/gtkozsxtvs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.9152youxi.cn/gtjuncbtfc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.0kj1m.cn/gteesyemtp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtgphmwglt.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtkjaadxfe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xinyue.icu/gtmzvmwgoq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tian-w.cn/gtnnptqwds.html

================================================================================
来源：http://hz.ydzc1.top/gtcrqnhytk.html

D. 数组 / 列表 / 集合
来源：http://hz.0kj1m.cn/gtrpnoodre.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqxgoxgtj.html

[D01] 创建数组 / 列表
来源：http://hz.xylfe.cn/gtfumsjsbt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.pengpengdd.cyou/gtbvabayft.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtblxjeqbi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gtycnfqeke.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtyxkplzgn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuxming.cn/gttxrbgvsm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.smart0.xyz/gtxtcffxma.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtqsrhlokl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtujmvjmqt.html

[D02] 追加元素到末尾
来源：http://hz.fzhhl.top/gthxxemjfg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xinyue.icu/gtrszylnal.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenjidiqi.icu/gtodpjavdd.html

JS:   arr.push(4);
来源：http://hz.fzhhl.top/gtmunmkhwa.html

TS:   arr.push(4);
来源：http://hz.sxryk.cn/gtlszoofzc.html

Java: list.add(4);
来源：http://hz.redwolf501.top/gtjlynksip.html

Go:   arr = append(arr, 4)
来源：http://hz.wangdashe.top/gtqslbzoma.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cashguo.top/gtluqqtdot.html

C#:   list.Add(4);
来源：http://hz.xingfuxueyuan.xyz/gtrmcirejl.html

[D03] 在指定位置插入元素
来源：http://hz.dashuyun.cn/gtqcxyymql.html

Py:   arr.insert(0, 0)
来源：http://hz.birdmap.top/gtytfrzvbj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.smart0.xyz/gtcomfbuas.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinghuilouyu.cn/gtvhqwvhbf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aibaodan.cn/gtrrwkrugd.html

Java: list.add(0, 0);
来源：http://hz.birdmap.top/gtfxhbssxk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.birdmap.top/gtvvalgvmv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gtpcbkrfxz.html

C#:   list.Insert(0, 0);
来源：http://hz.yvedp.cn/gtmddcmyvt.html

[D04] 删除元素
来源：http://hz.cheryme.top/gtbxyvkvuu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhiwuduotai.top/gtphiztuxz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yangfankeji.com/gtgpzxucqc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fzhhl.top/gtirvwnnpg.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtxziebswy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ybcxt.top/gtpegpobye.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gaohongyu789.top/gtxhvbcngo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.andypj.xyz/gtevfcqhpc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtysotqbcs.html

[D05] 访问与修改元素
来源：http://hz.yj20258888.top/gtqppstuty.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtuaqnmatn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gtbefwihzs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgufenzy.top/gtxecgeyou.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jqgfzy.top/gtqimxeawy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtboaokuqf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtmwjrrhbh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtorztzzhl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cdnleiting.top/gtvzgmbdgn.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gtradhqugq.html

Py:   len(arr)
来源：http://hz.ydjk.org.cn/gtyoxmokag.html

PHP:  count($arr);
来源：http://hz.vqdsnc.cn/gtxktffqpz.html

JS:   arr.length
来源：http://hz.sysykeji.top/gtpbbpjuid.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gttngbocfx.html

Java: list.size();
来源：http://hz.ppjwa.cn/gtvwqgqffs.html

Go:   len(arr)
来源：http://hz.daxiang520.top/gtcwnsvcyg.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtkcyxunck.html

C#:   list.Count;
来源：http://hz.yvedp.cn/gtrfrfhsdq.html

[D07] 切片 / 取子数组
来源：http://hz.ywan-chungtsiang.top/gtuabvxuok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gtdmhhncsp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtqyzqpwny.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtgaykegtw.html

TS:   arr.slice(1, 4);
来源：http://hz.sxryk.cn/gtxcjybzme.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtonqznxtr.html

Go:   arr[1:4]
来源：http://hz.0kj1m.cn/gtchlxdtdh.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtwndvmqnn.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtkxcuqjou.html

[D08] 合并两个数组
来源：http://hz.haohaochexian.top/gtmlmvgkoy.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258.top/gtusoeltnn.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gtbwmhxesl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtyfskglsl.html

TS:   [...a, ...b];
来源：http://hz.hnxiangtu.top/gtanwxlads.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj20258.top/gtwdbidcmx.html

Go:   append(a, b...)
来源：http://hz.quarkkingdee.top/gtkwmwpeyo.html


<!-- 参考信息 -->