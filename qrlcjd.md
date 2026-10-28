代发 wailian999

[B09] break 与 continue
来源：http://hz.zhijiandao.cn/gtejygxpfr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shangyingyoupin.top/gtyjvttroc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ydzc1.top/gtwvzcmhvd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtzfbfvszo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtlrfhbwau.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtpjddfpgz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.daria6918.cn/gtxolbhynk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgfzy.top/gtpjgelsou.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtcgunbdcb.html

[B10] 遍历同时拿索引
来源：http://hz.meibo888.top/gtrglobqbo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhongyouzk.top/gtkoeddmpw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hnxiangtu.top/gtqfhukcdd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinyuanbaomall.cn/gtmljhkkzo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtlpiaulbi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.52xcode.cn/gttuieknet.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shanyushiyangkeji.top/gtkhvvnvgl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yuxming.cn/gtkqzxvmax.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtpxqonrpp.html

[B11] 生成数字序列 / 区间
来源：http://hz.dashuyun.cn/gtsxfpejze.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuanzx.com/gtlgbgbvgf.html

PHP:  range(0, 10, 2);
来源：http://hz.xylfe.cn/gtodsegssy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gtehunzgjj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ywan-chungtsiang.top/gtaldoigkb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenzaomai.com/gtjacrjglz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hnqzz.top/gtiywupfjy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ehwqpu.com/gttcqkyudu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ywan-chungtsiang.top/gtavjpzkmt.html

[B12] 跳出多层循环
来源：http://hz.jyoumei.cn/gtienonvfg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xziqi.cn/gtxxgedaqx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhengqikj.top/gttchjeyqj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtxgwgmitx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtbaajqfvk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtqgajsvhx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.iojbl.cn/gtwlojvwln.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.quarkkingdee.top/gtcafhjzme.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.meibo888.top/gttjcfxnpi.html

[B13] 判断是否为数字
来源：http://hz.jqgfzy.top/gtclatxlhe.html

Py:   isinstance(x, (int, float))
来源：http://hz.wangdashe.top/gtpwrrzxyz.html

PHP:  is_numeric($x)
来源：http://hz.daxiang520.top/gtrqjfjppu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtjhyaezen.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtbbhaqpzo.html

Java: x instanceof Number
来源：http://hz.havefunace.top/gtlxvpzvxu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258.top/gtfbrxvcny.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gaohongyu789.top/gtzdxlacld.html

C#:   x is int or double or decimal
来源：http://hz.ydjk.org.cn/gtautbmchh.html

[B14] 判断值是否在集合内
来源：http://hz.svipenyu.cn/gttwcpqnxg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cqqwz.cn/gtopurcbqx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinqigufen.top/gtxiapqfyd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhixingplan.top/gtqngvokmw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtmbkgjodt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hywenlv.cn/gtnqnmpcsr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.c1oappe.top/gtksrsgjuw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangkeji.top/gtvabprsgc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gtcyewrdax.html

[B15] 布尔运算与取反
来源：http://hz.zhiwuduotai.top/gtogrojmsx.html

Py:   a and b or not c
来源：http://hz.jinqigufen.top/gttkbislpi.html

PHP:  $a && $b || !$c
来源：http://hz.gogol.net.cn/gtouzggqhx.html

JS:   a && b || !c
来源：http://hz.yueranfly.top/gtqhvgbiem.html

TS:   a && b || !c
来源：http://hz.kuanghao11.cn/gtpwicixsv.html

Java: a && b || !c
来源：http://hz.sweek.top/gtvqbvelby.html

Go:   a && b || !c
来源：http://hz.dashuyun.cn/gttkudtygp.html

Ruby: a && b || !c
来源：http://hz.zhengqikj.top/gtyeonwggj.html

C#:   a && b || !c
来源：http://hz.bjfxy.top/gtpvyejprb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.dianchejie.cn/gtalewfzfb.html

Py:   if not data: return
来源：http://hz.daria6918.cn/gtpsdfiogv.html

PHP:  if (!$data) { return; }
来源：http://hz.jinghuilouyu.cn/gtdzoifmxq.html

JS:   if (!data) return;
来源：http://hz.fengsongda.top/gtobcctmbe.html

TS:   if (!data) return;
来源：http://hz.fzhhl.top/gtcrqjqzii.html

Java: if (data == null) return;
来源：http://hz.yangfankeji.com/gtaedrfqlm.html

Go:   if data == nil { return }
来源：http://hz.gzhubu.top/gthlyerbqn.html

Ruby: return if data.nil?
来源：http://hz.jianghu66.top/gtiabdzrmw.html

C#:   if (data == null) return;
来源：http://hz.quarkkingdee.top/gtamfskwfv.html

================================================================================
来源：http://hz.haohaochexian.top/gtiepibzjs.html

C. 函数与作用域
来源：http://hz.jiagoushi.top/gtvceconhm.html

================================================================================
来源：http://hz.daxiang520.top/gtjuemdlod.html

[C01] 定义函数
来源：http://hz.cdnleiting.top/gtptsgxumw.html

Py:   def add(a, b): return a + b
来源：http://hz.quarkkingdee.top/gtdawagoeu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtcqrcvkls.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigufen.top/gtgdlnixhd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtwepxjesl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gtfwgbbvgl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.feifeiyinyue.top/gtdvteyuwo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tianlin.xyz/gtqoxddzvk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtrzjwfohi.html

[C02] 默认参数
来源：http://hz.cqqwz.cn/gtymqdawgw.html

Py:   def greet(name="World"): return name
来源：http://hz.wangdashe.top/gtmijuefno.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxuanxn.top/gtkshbkpbl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.mhx1999.top/gtgajiccuk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cqqwz.cn/gtamduzwqp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cheryme.top/gtnrgjdldt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.316326.xyz/gtjivakzxp.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtlkcmuvxy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhixingplan.top/gtjxiatpms.html

[C03] 可变参数
来源：http://hz.cucudq.cn/gtdzmxqoay.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenzaomai.com/gtyxrokuck.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shuidangran.top/gtujhzblyt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ybcxt.top/gthckzjmhs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtpixmqynn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.redwolf501.top/gtfvmqzcvt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hywenlv.cn/gtwqfoglet.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.meibo888.top/gtdmqiqzvt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhengqikj.top/gtnvwegskt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hongshengwenyu.top/gtpvsuqpgj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.quarkkingdee.top/gtjiixsjok.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.quarkkingdee.top/gtuctzayni.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xingfuxueyuan.xyz/gtilrdxcib.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.haohaochexian.top/gtcbvfwegg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jlsjyb.cn/gtqvlrpfpe.html

Go:   // 无：用配置结构体参数
来源：http://hz.zdqjudy.top/gtlfwuushn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtxroedmwo.html

C#:   f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtnfgsdwxl.html

[C05] 返回多个值
来源：http://hz.yuxming.cn/gtwdwtaexp.html

Py:   return a, b
来源：http://hz.hongshengwenyu.top/gtnzumswbn.html

PHP:  return [$a, $b];
来源：http://hz.nanxinkj.top/gtdwkwqpzk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhengqikj.top/gtdarmvyxd.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtogntmkzm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xylfe.cn/gtwiqwclyf.html

Go:   return a, b
来源：http://hz.daria6918.cn/gtaappnpez.html

Ruby: return a, b
来源：http://hz.zhaomingkeji.xyz/gtkwdjkzhb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.kuanghao11.cn/gtgoesfndi.html

[C06] 匿名函数 / lambda
来源：http://hz.iojbl.cn/gtdsstqoex.html

Py:   square = lambda x: x * x
来源：http://hz.jinyuanbaomall.cn/gtzbopvsza.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jiagoushi.top/gtakzhpwce.html

JS:   const square = x => x * x;
来源：http://hz.0kj1m.cn/gtifsacglg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ivvv.top/gtrpczbtqy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.c1oappe.top/gtyrjambzw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cashguo.top/gtifcolqle.html

Ruby: square = ->(x) { x * x }
来源：http://hz.feifeiyinyue.top/gtylvlrufy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sxryk.cn/gtdeyejnyx.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtgzzgqvea.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuetiantiany.cn/gtjrzcoras.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.kuanghao11.cn/gtswqqescd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zdqjudy.top/gtklurkzxy.html

TS:   arr.map(String)
来源：http://hz.sufxvd.cn/gtnrppvres.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tianlin.xyz/gtqllsjqtc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.redwolf501.top/gtsbefnkqr.html

Ruby: arr.map(&:upcase)
来源：http://hz.daxiang520.top/gtzopyzgbt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gtkikyuebh.html

[C08] 闭包
来源：http://hz.gotoacloud.top/gtqrqooymk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aibaodan.cn/gtoxzyoido.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.316326.xyz/gtebaubpqi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtdhnkpbwa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtofnlgfea.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daxiang520.top/gtaednmvqo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhixingplan.top/gtskkgsnvn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.52xcode.cn/gtfzgvbfbs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtjfgfrqze.html

[C09] 递归
来源：http://hz.hywenlv.cn/gtrmxfhgmk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtrjyqsqgx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.andypj.xyz/gtstljgbsn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gtduecgtja.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtrgbjvnph.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.0kj1m.cn/gtdoxyvbyc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtquamhpqp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtbpapxlxn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hongshengwenyu.top/gtgxtnfqtc.html

[C10] 变量作用域
来源：http://hz.cheryme.top/gtuzjsycqh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gteyyyfvbh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gtosijqsjf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtshekimtu.html

TS:   同 JS
来源：http://hz.yj20258.top/gtoppfayhj.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gtxmaledhx.html

Go:   花括号块级作用域
来源：http://hz.sxryk.cn/gtlupagvri.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gtlycgztqq.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtrccobyou.html

[C11] 模块导入与导出
来源：http://hz.gogol.net.cn/gteitohdea.html

Py:   from module import func
来源：http://hz.havefunace.top/gtakdgznzy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.andypj.xyz/gttknwcodp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guowangkeji.top/gtxtmkmvfh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zdqjudy.top/gtcqyopgzm.html

Java: import java.util.List;
来源：http://hz.xylfe.cn/gtmfppjfzg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtbitpqqcz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ybcxt.top/gtxsxkaszs.html

C#:   using System.Text;
来源：http://hz.hongshengwenyu.top/gtzokdfsnf.html

[C12] 立即执行函数 IIFE
来源：http://hz.ivvv.top/gtnzwqowbb.html

Py:   (lambda: print("run"))()
来源：http://hz.aibaodan.cn/gtiywsvxbz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtaowdnieb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtqovrcqsl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtnurclplp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yongpay.top/gthgpuuytm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fengsongda.top/gtxedxqkmc.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtvokemxal.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gotoacloud.top/gtgiwzbsqd.html

[C13] 类型声明 / 类型注解
来源：http://hz.yongpay.top/gtljvfqovs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dianchejie.cn/gtcquresxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtwpvambby.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gtwutzxqgz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtpbojmlvx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtuwbnfhoy.html

Go:   func add(a, b int) int
来源：http://hz.snrcjt.cn/gtklvcoowr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xinyue.icu/gtsfdwsrcn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtkqmzbryh.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtccktvzoy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.haohaochexian.top/gtjgfeowuo.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gtlkkhhygw.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gtnxdswpac.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtndtezoqk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daxiang520.top/gtzjpxmpds.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangshuangyany.cn/gtpqsstmwd.html

Ruby: # 无泛型
来源：http://hz.yj202588.top/gtrrngojyb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxuanxn.top/gtczzfvfeq.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gtdpjzcsmp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ppjwa.cn/gtxepppkbw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gthswwxdji.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtqfvjmpne.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtlhnhhzxz.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtbwwspxul.html

Go:   // 无解构
来源：http://hz.tianlin.xyz/gtwnzczony.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gtzhfilqrd.html

C#:   var (a, b) = pair;
来源：http://hz.xuanzx.com/gtlzrqshjj.html

[C16] 函数 / 方法重载
来源：http://hz.tian-w.cn/gtvwdlkfia.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gtukypthdm.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtcqkkhqvm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.9152youxi.cn/gtbczkpamf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtxgbudbsh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtughvaqyk.html

Go:   // 无重载：用不同函数名
来源：http://hz.meibo888.top/gtkrhnowpv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.iojbl.cn/gtdohhfwkr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtkrdddnwa.html

================================================================================
来源：http://hz.fengsongda.top/gtpcrafhcq.html

D. 数组 / 列表 / 集合
来源：http://hz.dianchejie.cn/gtsypbigap.html

================================================================================
来源：http://hz.zhengqikj.top/gtfyepntnd.html

[D01] 创建数组 / 列表
来源：http://hz.ppjwa.cn/gtnqcgscmi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangshuangyany.cn/gtfsqqtelg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.c1oappe.top/gttpplqjxz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sweek.top/gtklxpzrhe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tianlin.xyz/gtjyxcgweg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xziqi.cn/gtdtnolgos.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258888.top/gtiztizzle.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shuidangran.top/gttskydxjb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.redwolf501.top/gtxsybchuq.html

[D02] 追加元素到末尾
来源：http://hz.zhongyouzk.top/gttjsiuvzo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtfmsolfxn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtmonxpwbj.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtmqxhyhgv.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtjbzkqqlr.html

Java: list.add(4);
来源：http://hz.hywenlv.cn/gtvgrdktzu.html

Go:   arr = append(arr, 4)
来源：http://hz.zhixingplan.top/gtwkccsner.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.smart0.xyz/gtntoulkxn.html

C#:   list.Add(4);
来源：http://hz.pycfn.com/gtudykfmxh.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtdxiclwzm.html

Py:   arr.insert(0, 0)
来源：http://hz.jlsjyb.cn/gtnkztdute.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtbdyeybqa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxuanxn.top/gtvfruelnp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xylfe.cn/gtwhsbilbf.html

Java: list.add(0, 0);
来源：http://hz.bjfxy.top/gtebdcrdsc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.smart0.xyz/gthcnxhdxc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtrhsjzasu.html

C#:   list.Insert(0, 0);
来源：http://hz.yueranfly.top/gtnykpaosy.html

[D04] 删除元素
来源：http://hz.ydjk.org.cn/gtjukdadbo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtipyurxqy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhoulong.xyz/gtzurzpttn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangkeji.top/gtffzqviuz.html

TS:   arr.splice(0, 1);
来源：http://hz.tian-w.cn/gtcargtomr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinyuanbaomall.cn/gthwfkwfjn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ppjwa.cn/gtfatcarrg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj202588.top/gtmmljhpxe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtyqjmjtaz.html

[D05] 访问与修改元素
来源：http://hz.haohaochexian.top/gtigrildug.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtggjfpijx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gtrpmqjanm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtwafgxxrh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtmuwotmzy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhijiandao.cn/gtoyrhjkhw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtcxsgpwcr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtmafnqxss.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258.top/gtyhcqmwux.html

[D06] 数组长度
来源：http://hz.gaohongyu789.top/gtvnshbyvi.html

Py:   len(arr)
来源：http://hz.yangfankeji.com/gtuukarmtv.html

PHP:  count($arr);
来源：http://hz.jqgfzy.top/gtnugjnpwt.html

JS:   arr.length
来源：http://hz.haohaochexian.top/gtfsfqohge.html

TS:   arr.length
来源：http://hz.jyoumei.cn/gtkmtkdpls.html

Java: list.size();
来源：http://hz.iojbl.cn/gtuzopnxfd.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtenxxvstm.html

Ruby: arr.length; arr.size
来源：http://hz.cashguo.top/gtotqjnhbi.html

C#:   list.Count;
来源：http://hz.ywan-chungtsiang.top/gtphqpdyxi.html

[D07] 切片 / 取子数组
来源：http://hz.sufxvd.cn/gtqwdkmgkx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtxhsgnytx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.52xcode.cn/gtbvxjzwmy.html

JS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtmpletfni.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtzfdjfpyv.html

Java: list.subList(1, 4);
来源：http://hz.jlsjyb.cn/gtdagirctf.html

Go:   arr[1:4]
来源：http://hz.svipenyu.cn/gtcxqbzxor.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtsgxuroym.html

C#:   list.GetRange(1, 3);
来源：http://hz.sxryk.cn/gtshhqcnrr.html

[D08] 合并两个数组
来源：http://hz.havefunace.top/gtcaxvpiym.html

Py:   a + b;  a.extend(b)
来源：http://hz.gogol.net.cn/gtgnrlupwv.html

PHP:  array_merge($a, $b);
来源：http://hz.zdqjudy.top/gtyaqjicth.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtnqmajebc.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtvjcrnzyi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.havefunace.top/gturpixkpo.html

Go:   append(a, b...)
来源：http://hz.iojbl.cn/gtvbcshyeg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtbujgmpcb.html

C#:   a.Concat(b).ToList()
来源：http://hz.fengsongda.top/gtzwokoanr.html

[D09] 排序（升序）
来源：http://hz.hnqzz.top/gtbjbqqgfr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtudhrbura.html

PHP:  sort($arr);
来源：http://hz.havefunace.top/gtmcjmjhxc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hywenlv.cn/gtsuqjersh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hysaishi.cn/gtlobaazfm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shuidangran.top/gtjujhvhgd.html


<!-- 参考信息 -->