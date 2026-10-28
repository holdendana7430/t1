代发 wailian999

[B09] break 与 continue
来源：http://hz.52xcode.cn/gtnexculry.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jqgufenzy.top/gtqyraemqz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.quarkkingdee.top/gtinplsjsu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtomjcpdqi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtkcqtatsq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtrhnroazm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinghuilouyu.cn/gtfrunyxiy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shanyushiyangtech.top/gtdctvvigh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtceyohiyz.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtxykeoozo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hnqzz.top/gttoqazydr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.iojbl.cn/gtrwelhaez.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jyoumei.cn/gtbumcupjz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xuetiantiany.cn/gtepscvpxw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hywenlv.cn/gtwcstnarh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhijiandao.cn/gtakrzrnkd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guowangkeji.top/gtturfahxu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangkeji.top/gtbgqqbvuv.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuxming.cn/gtqhjdtwth.html

Py:   list(range(0, 10, 2))
来源：http://hz.hysaishi.cn/gtssqrwjxi.html

PHP:  range(0, 10, 2);
来源：http://hz.tianlin.xyz/gtydehdmfs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sufxvd.cn/gtysmmkdui.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zdqjudy.top/gtztoikmrg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.9152youxi.cn/gtiyndzxkz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ybcxt.top/gtsximazxq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jianghu66.top/gtqvgidbkt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenlongwang.top/gtblcgroxr.html

[B12] 跳出多层循环
来源：http://hz.jianghu66.top/gtdgcctrlz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hnqzz.top/gtfxunaaro.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jlsjyb.cn/gtfimqpowh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtpgwddxwd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.bjfxy.top/gttqmozkrc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtzeixxjlo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tian-w.cn/gtzydcrgco.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hysaishi.cn/gtidlkniko.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guowangkeji.top/gtdxithcyt.html

[B13] 判断是否为数字
来源：http://hz.chenzaomai.com/gtchudwkqk.html

Py:   isinstance(x, (int, float))
来源：http://hz.birdmap.top/gtfjzgjykm.html

PHP:  is_numeric($x)
来源：http://hz.havefunace.top/gteihsiauh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gtwejaxjif.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.svipenyu.cn/gtugsyyjps.html

Java: x instanceof Number
来源：http://hz.yvedp.cn/gtrwsghsjv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.chenzaomai.com/gtxoaphuyz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gogol.net.cn/gtcsqgublo.html

C#:   x is int or double or decimal
来源：http://hz.vqdsnc.cn/gtmpcjxhfm.html

[B14] 判断值是否在集合内
来源：http://hz.yangfankeji.com/gtbwaqtkin.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cashguo.top/gthzlbchnb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.mhx1999.top/gtwchymxcl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtffgovjgv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gtypdzwuxn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.feifeiyinyue.top/gtgfknstkp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hnqzz.top/gtddadgpoh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jianghu66.top/gtqppipaza.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aibaodan.cn/gtpracqoyy.html

[B15] 布尔运算与取反
来源：http://hz.jiagoushi.top/gtuakgomvw.html

Py:   a and b or not c
来源：http://hz.pengpengdd.cyou/gtnhdvmlnz.html

PHP:  $a && $b || !$c
来源：http://hz.0kj1m.cn/gtvodjalrn.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtqeynyvxx.html

TS:   a && b || !c
来源：http://hz.chenzaomai.com/gtfbsimczr.html

Java: a && b || !c
来源：http://hz.cashguo.top/gtpfzmuqkk.html

Go:   a && b || !c
来源：http://hz.haohaochexian.top/gtjzqdmlqn.html

Ruby: a && b || !c
来源：http://hz.hammf.cn/gtvnzatslf.html

C#:   a && b || !c
来源：http://hz.svipenyu.cn/gtknoehaqz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gtgmjcuhqm.html

Py:   if not data: return
来源：http://hz.dianchejie.cn/gtdmyenajp.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtmjwaekux.html

JS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtvxmraemw.html

TS:   if (!data) return;
来源：http://hz.zhoulong.xyz/gtoyopeiyr.html

Java: if (data == null) return;
来源：http://hz.cashguo.top/gtghzwhzxj.html

Go:   if data == nil { return }
来源：http://hz.zhijiandao.cn/gtpbgwjilb.html

Ruby: return if data.nil?
来源：http://hz.zhaomingkeji.xyz/gtwzhrgfbx.html

C#:   if (data == null) return;
来源：http://hz.jqgfzy.top/gteesgueak.html

================================================================================
来源：http://hz.yangfankeji.com/gtoxpcyyth.html

C. 函数与作用域
来源：http://hz.meibo888.top/gtkdskmlnq.html

================================================================================
来源：http://hz.zhixingplan.top/gtbxalvwyv.html

[C01] 定义函数
来源：http://hz.jianghu66.top/gtfzxclgye.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gtvsxbafyd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gtkfhvdpvy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtpdtkupqv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtgcuuktgt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtisuzomas.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtzmtgjmtj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daria6918.cn/gtyziotmxg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gthwynqswg.html

[C02] 默认参数
来源：http://hz.hongshengwenyu.top/gtdmkajovw.html

Py:   def greet(name="World"): return name
来源：http://hz.xuetiantiany.cn/gtbxsawjlc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj202588.top/gtmpkqplck.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtiiacphtx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtsjhxdzgk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxuanxn.top/gthoblhnoe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgufenzy.top/gtsifavvlx.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtfucmtvix.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.0kj1m.cn/gtdxbddxjz.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtoldtcgqa.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhiwuduotai.top/gtsdyatzvq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xinyue.icu/gtwhanspop.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gtdksiiviu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shzxlz.cn/gtzrwyrdvt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtzkuehkoh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.9152youxi.cn/gtzmpdqimd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ybcxt.top/gtwslluhkv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.snrcjt.cn/gtyhnwnusp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gtluhjrvqp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yangfankeji.com/gtbvtwzinv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.bjfxy.top/gtlusatrbn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtmxmdyhpk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gogol.net.cn/gtxglrgybg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zdqjudy.top/gtcdrqjnnl.html

Go:   // 无：用配置结构体参数
来源：http://hz.hnxiangtu.top/gtsjxreerk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydjk.org.cn/gtyqvbijxo.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtnrfekrps.html

[C05] 返回多个值
来源：http://hz.quarkkingdee.top/gttwcxqhbf.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gtgxxadjbf.html

PHP:  return [$a, $b];
来源：http://hz.birdmap.top/gtwifuxjpb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gtrxxkdail.html

TS:   return { a, b };
来源：http://hz.zhongyouzk.top/gtxtcpoxkz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gtqxalbeur.html

Go:   return a, b
来源：http://hz.zycfv.cn/gteqsdevhn.html

Ruby: return a, b
来源：http://hz.gaohongyu789.top/gthvtpztna.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.iojbl.cn/gtxyggeclf.html

[C06] 匿名函数 / lambda
来源：http://hz.andypj.xyz/gtsmnpjude.html

Py:   square = lambda x: x * x
来源：http://hz.316326.xyz/gtjvwfsnbf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhaomingkeji.xyz/gthpzohaak.html

JS:   const square = x => x * x;
来源：http://hz.nwbrower.top/gtapoxoxbc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cqqwz.cn/gtzfvdhzfz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtrzflploh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cdnleiting.top/gtfmobembz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tian-w.cn/gtdglkkwlr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sysykeji.top/gttxqawnch.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtedmgzxyu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhengqikj.top/gtkudntttn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinqigfzy.top/gtypzkkntw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.redwolf501.top/gtpiupgnil.html

TS:   arr.map(String)
来源：http://hz.nwbrower.top/gtsjjbutyn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.52xcode.cn/gtxllefadn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sufxvd.cn/gtuoeqmsij.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtgzvqswtn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ybcxt.top/gtlwltgbhs.html

[C08] 闭包
来源：http://hz.gotoacloud.top/gtulkgjpwd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gtpbxzcxdc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hysaishi.cn/gtkgngtycy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtelgxooba.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtzpabsfkb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fzhhl.top/gtxlhpcuvx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtpmoicbbc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tianlin.xyz/gtfprpmrgn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gthbincmeh.html

[C09] 递归
来源：http://hz.yanxiufei.cn/gtnsmxrzbj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hammf.cn/gtzoadiday.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydjk.org.cn/gtrhdglowi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtossutyms.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgufenzy.top/gthpquvtbc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhijiandao.cn/gtsfvthrmt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtsdhagjln.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtsrtwriki.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangtech.top/gtjkrnmwks.html

[C10] 变量作用域
来源：http://hz.ywan-chungtsiang.top/gttrtweusc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigfzy.top/gtuwtzzlmp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuetiantiany.cn/gtcowrrxzc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xylfe.cn/gtnqvtbggq.html

TS:   同 JS
来源：http://hz.ehwqpu.com/gtyuofciyo.html

Java: 方法内为块级作用域
来源：http://hz.jinyuanbaomall.cn/gtudsnalnb.html

Go:   花括号块级作用域
来源：http://hz.birdmap.top/gtjptshfan.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.mhx1999.top/gtliaxlxlm.html

C#:   块级作用域
来源：http://hz.aibaodan.cn/gtgtfrpvpw.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtvxpgxhmx.html

Py:   from module import func
来源：http://hz.9152youxi.cn/gtwbyxlsmx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aizwys.cn/gtcpthpgwn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.bjfxy.top/gtkftjmygb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtnulavgqo.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtbljultgw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtdchliysd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.dashuyun.cn/gtigvgswvg.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtrqctjpls.html

[C12] 立即执行函数 IIFE
来源：http://hz.haohaochexian.top/gtcxmxnofh.html

Py:   (lambda: print("run"))()
来源：http://hz.316326.xyz/gtifohtrcw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hysaishi.cn/gtvddxrhqd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtllbyijcf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtdntlcosg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.haohaochexian.top/gtbemrujub.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gthuwaotkh.html

Ruby: -> { puts "run" }.call
来源：http://hz.svipenyu.cn/gtvwkyabwo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtfbcpqjcx.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtifrrcxrt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenjidiqi.icu/gtvgrgfjcx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtoqxpbqwo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuetiantiany.cn/gtfpqkrqeu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gttykznoxf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtyooaatnm.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gthtijbhau.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.0kj1m.cn/gtljleyugf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhoulong.xyz/gtwlmlxbgo.html

[C14] 泛型函数
来源：http://hz.aibaodan.cn/gtatuoxicd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shuidangran.top/gtrkcdzrwd.html

PHP:  // 无泛型
来源：http://hz.gogol.net.cn/gtwewvzgec.html

JS:   // 无泛型
来源：http://hz.dianchejie.cn/gtrxfipfsx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtcveudptl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aizwys.cn/gtfwjcyosn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zdqjudy.top/gtkyvyfscb.html

Ruby: # 无泛型
来源：http://hz.shzxlz.cn/gtqhypnscs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.snrcjt.cn/gtatwovsgi.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtchjaqurh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nwbrower.top/gtqxeyuael.html

PHP:  [$a, $b] = $pair;
来源：http://hz.wangshuangyany.cn/gtzrogaubs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtideyfwxr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.vqdsnc.cn/gtabeszase.html

Java: // 无解构
来源：http://hz.zhengqikj.top/gthkwlinck.html

Go:   // 无解构
来源：http://hz.ppjwa.cn/gtdsrluxfo.html

Ruby: a, b = pair
来源：http://hz.zhengqikj.top/gtsobjynwl.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtylbondgu.html

[C16] 函数 / 方法重载
来源：http://hz.316326.xyz/gtcyrsznqz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.0kj1m.cn/gtbwmyemez.html

PHP:  // 无重载
来源：http://hz.daxiang520.top/gtkfgoizgo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fzhhl.top/gtyzrgmzgw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xylfe.cn/gtpamytxla.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtodisshlm.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhiwuduotai.top/gttmhqovoa.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fzhhl.top/gtmjbahoup.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtqhtbpikw.html

================================================================================
来源：http://hz.jqgfzy.top/gtyaobuxej.html

D. 数组 / 列表 / 集合
来源：http://hz.ydzc1.top/gtklcenunk.html

================================================================================
来源：http://hz.ehwqpu.com/gtozowzwnk.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258888.top/gtqyetkefa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtkrugrspl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.meibo888.top/gtgkwmopia.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xingfuxueyuan.xyz/gtjeuoxswu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gzhubu.top/gtuibmuoii.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.fzhhl.top/gthklxvqfz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gtadetzopu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtxxmmpmkb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuetiantiany.cn/gtnvzibvay.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gtyshtxvzf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hfpthk.cn/gtsfavdrvu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gtevoojvav.html

JS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtcbkxsajs.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtmegewuvm.html

Java: list.add(4);
来源：http://hz.jinghuilouyu.cn/gtkczzdsiq.html

Go:   arr = append(arr, 4)
来源：http://hz.yanxiufei.cn/gtftdwjxhf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhiwuduotai.top/gtfosfbqqr.html

C#:   list.Add(4);
来源：http://hz.jinqigfzy.top/gtozmkromv.html

[D03] 在指定位置插入元素
来源：http://hz.zhoulong.xyz/gtajhatcbv.html

Py:   arr.insert(0, 0)
来源：http://hz.zdqjudy.top/gtxwektmcm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhijiandao.cn/gthpcnoqaq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aizwys.cn/gtutvzohqs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangkeji.top/gtdqveahta.html

Java: list.add(0, 0);
来源：http://hz.fzhhl.top/gtkchuzwgz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hfpthk.cn/gtvegeadcd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yonumen.top/gtbxtudash.html

C#:   list.Insert(0, 0);
来源：http://hz.ydjk.org.cn/gtfzfocvkw.html

[D04] 删除元素
来源：http://hz.snrcjt.cn/gthykjlehx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.guowangkeji.top/gteyuoszuz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gtfkqgtyup.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ywan-chungtsiang.top/gtktyneyhh.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtssmuakbc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258888.top/gtdemxlcfs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtfklwunyh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtneckvfor.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gtqdcraybw.html

[D05] 访问与修改元素
来源：http://hz.daria6918.cn/gtfzyfahwn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtsxxmrvhz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jlsjyb.cn/gtgegkjahc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tian-w.cn/gtvolihtts.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jianghu66.top/gtfqlmkiua.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daria6918.cn/gtxqfykxdv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtpzwtkctr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtmowguezr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtfxwuteuo.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtrqrliwim.html

Py:   len(arr)
来源：http://hz.pycfn.com/gtuyeopzid.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtldiymyyc.html

JS:   arr.length
来源：http://hz.gzhubu.top/gtubwntvge.html

TS:   arr.length
来源：http://hz.birdmap.top/gtvwqbfsxf.html

Java: list.size();
来源：http://hz.ydzc1.top/gtkrrhnuqx.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtgpqhluhh.html

Ruby: arr.length; arr.size
来源：http://hz.zhijiandao.cn/gtpzygrdqf.html

C#:   list.Count;
来源：http://hz.9152youxi.cn/gtipdfihbm.html

[D07] 切片 / 取子数组
来源：http://hz.ywan-chungtsiang.top/gturzulpye.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.feifeiyinyue.top/gtqrswogas.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pengpengdd.cyou/gthcgkhvaq.html

JS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtuwajanow.html

TS:   arr.slice(1, 4);
来源：http://hz.sxryk.cn/gtjnoxmvxb.html

Java: list.subList(1, 4);
来源：http://hz.yonumen.top/gtxzggelgq.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtunieqcwl.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gthwpbtjoe.html

C#:   list.GetRange(1, 3);
来源：http://hz.fzhhl.top/gtngyhhoxv.html

[D08] 合并两个数组
来源：http://hz.meibo888.top/gtrvznpjpl.html

Py:   a + b;  a.extend(b)
来源：http://hz.bjfxy.top/gthaytbrjb.html

PHP:  array_merge($a, $b);
来源：http://hz.yuanzhike.top/gtpeyqevtw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shangyingyoupin.top/gttoozgrdy.html

TS:   [...a, ...b];
来源：http://hz.daria6918.cn/gtpubmhvdd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtvchljjbc.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtweabmqbf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtjuzzaxmw.html

C#:   a.Concat(b).ToList()
来源：http://hz.ehwqpu.com/gtzkndizvl.html

[D09] 排序（升序）
来源：http://hz.sysykeji.top/gtujxkzlho.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtsjzmeaww.html

PHP:  sort($arr);
来源：http://hz.wangdashe.top/gtqbkhrcqd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gotoacloud.top/gtpowyjixh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gtcfxfqdph.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cheryme.top/gtyznkfkuq.html


<!-- 参考信息 -->