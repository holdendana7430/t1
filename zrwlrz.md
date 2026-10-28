代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gterfvgffs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cheryme.top/gtnactvvqm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hfpthk.cn/gtnlvahbym.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gttgkhemvj.html

[B09] break 与 continue
来源：http://hz.shanyushiyangkeji.top/gtdfoxueru.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shzxlz.cn/gtdxzquvuw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.iojbl.cn/gteiljpspf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtfmdlpccj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtasehkhuq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gthgzsoidl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.wangshuangyany.cn/gtyvyzqurr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gogol.net.cn/gtvgsmdhvm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtquvktizs.html

[B10] 遍历同时拿索引
来源：http://hz.yuanzhike.top/gtrdbkiazy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tianlin.xyz/gtiqiartra.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daxiang520.top/gteivdthdn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daria6918.cn/gtkpromxck.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xuanzx.com/gtchvfjdrz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhixingplan.top/gtewtrcywe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.9152youxi.cn/gtgtxbzdoo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinqigufen.top/gtuxghiqjd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shzxlz.cn/gtrmgfooit.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhixingplan.top/gtjinsrlen.html

Py:   list(range(0, 10, 2))
来源：http://hz.ybcxt.top/gtoswhikao.html

PHP:  range(0, 10, 2);
来源：http://hz.tanke756.top/gtylwspjob.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.9152youxi.cn/gtdcjicqkw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuxming.cn/gtqqgejahw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.svipenyu.cn/gtzvzvmwjp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ybcxt.top/gtczuactdv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.svipenyu.cn/gtgrizukwj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xylfe.cn/gtzikmiwpz.html

[B12] 跳出多层循环
来源：http://hz.hnxiangtu.top/gtkcqevdwp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhixingplan.top/gtkabqkvbg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gzhubu.top/gtfltnigea.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtimlwurex.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtbchdedlp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtvrvavggv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zycfv.cn/gtusczbgad.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hongshengwenyu.top/gtmkimsiuz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.snrcjt.cn/gtgcipbawl.html

[B13] 判断是否为数字
来源：http://hz.zycfv.cn/gtwwjjkgzz.html

Py:   isinstance(x, (int, float))
来源：http://hz.cucudq.cn/gtawslqcic.html

PHP:  is_numeric($x)
来源：http://hz.bjfxy.top/gtukbizxwv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtssuhtssc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gtcztkxkaq.html

Java: x instanceof Number
来源：http://hz.52xcode.cn/gtpjjtthzw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tianlin.xyz/gtcqlzdwtp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sysykeji.top/gtviqvkmdn.html

C#:   x is int or double or decimal
来源：http://hz.cdnleiting.top/gtanworgpn.html

[B14] 判断值是否在集合内
来源：http://hz.cqqwz.cn/gttutvkgzv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangkeji.top/gtvgehefzw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhongyouzk.top/gtobvjsdsl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.52xcode.cn/gtnnyigboi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gtoqyohvsh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shzxlz.cn/gtxqbbnqoo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.fengsongda.top/gtpxmkxlrp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ybcxt.top/gtlzagrita.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shangyingyoupin.top/gtrserrfhg.html

[B15] 布尔运算与取反
来源：http://hz.jiagoushi.top/gtwdfpphke.html

Py:   a and b or not c
来源：http://hz.dianchejie.cn/gtavfobjnx.html

PHP:  $a && $b || !$c
来源：http://hz.ywan-chungtsiang.top/gttoeqptij.html

JS:   a && b || !c
来源：http://hz.cdnleiting.top/gtrhxdlmho.html

TS:   a && b || !c
来源：http://hz.ydjk.org.cn/gtksktktpc.html

Java: a && b || !c
来源：http://hz.feifeiyinyue.top/gtdcpdgdjt.html

Go:   a && b || !c
来源：http://hz.quarkkingdee.top/gthlrwtfrt.html

Ruby: a && b || !c
来源：http://hz.wangdashe.top/gtgmfvtnvm.html

C#:   a && b || !c
来源：http://hz.gaohongyu789.top/gtpmtakzfd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgufenzy.top/gtbpcxxsao.html

Py:   if not data: return
来源：http://hz.zhoulong.xyz/gtsxwyaiih.html

PHP:  if (!$data) { return; }
来源：http://hz.tanke756.top/gtzmjftcxs.html

JS:   if (!data) return;
来源：http://hz.nwbrower.top/gtfmitxsoh.html

TS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtclnkjnze.html

Java: if (data == null) return;
来源：http://hz.daria6918.cn/gtuczewltl.html

Go:   if data == nil { return }
来源：http://hz.cashguo.top/gtruywunkb.html

Ruby: return if data.nil?
来源：http://hz.snrcjt.cn/gtdkyltsat.html

C#:   if (data == null) return;
来源：http://hz.aizwys.cn/gtwjpdjhdp.html

================================================================================
来源：http://hz.zhengqikj.top/gtyjjzjchn.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gtwundiefq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtgpebvhph.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtrkoatouc.html

Py:   def add(a, b): return a + b
来源：http://hz.meibo888.top/gtxilotzsu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtfagfozot.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtbjkyghyz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtwjnndfkv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtlbvblopn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.52xcode.cn/gtlededowp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangkeji.top/gtqhsyanfd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gtmeoppuvm.html

[C02] 默认参数
来源：http://hz.zhongyouzk.top/gtrlcyklzm.html

Py:   def greet(name="World"): return name
来源：http://hz.cdnleiting.top/gtskdrrath.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hywenlv.cn/gtsjuvtent.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtvclvpzzh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtgtrdisem.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jyoumei.cn/gtvuqucpyw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.mhx1999.top/gtlgnjdsnt.html

Ruby: def greet(name = "World") = name
来源：http://hz.gogol.net.cn/gtlvygoqmq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenzaomai.com/gtihweruyl.html

[C03] 可变参数
来源：http://hz.yueranfly.top/gtelfizfjr.html

Py:   def total(*args): return sum(args)
来源：http://hz.gogol.net.cn/gtrcpyowis.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.c1oappe.top/gtquxgfnfb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtlxpzapln.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.9152youxi.cn/gtxioojhgp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangtech.top/gtreihahaa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ydzc1.top/gtcgqyftmx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.feifeiyinyue.top/gtvdzehfnz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtjjnrssxy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gttuyfhhjw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hammf.cn/gtlruoesjd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yangfankeji.com/gtjknxlumk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtsufwlmdy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shuidangran.top/gtziazvavq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yonumen.top/gtdjaeabhf.html

Go:   // 无：用配置结构体参数
来源：http://hz.iojbl.cn/gtunpxbqhk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtbjgekemc.html

C#:   f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtuyspbxxd.html

[C05] 返回多个值
来源：http://hz.yuanzhike.top/gtbuxqiccz.html

Py:   return a, b
来源：http://hz.9152youxi.cn/gthywijfkk.html

PHP:  return [$a, $b];
来源：http://hz.c1oappe.top/gtvcquekjv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.snrcjt.cn/gtgnttikye.html

TS:   return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtyauenzff.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aibaodan.cn/gtmshqtyqo.html

Go:   return a, b
来源：http://hz.52xcode.cn/gtulmyddkh.html

Ruby: return a, b
来源：http://hz.sysykeji.top/gtgkfucivn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yuxming.cn/gtcrnthdgp.html

[C06] 匿名函数 / lambda
来源：http://hz.9152youxi.cn/gtgjrejosi.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigfzy.top/gtyzstatfp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gtjmmbbpqh.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gttlfbqhod.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shanyushiyangkeji.top/gttgmztpzz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gtpzaiopvq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuetiantiany.cn/gtmmevhpmd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cqqwz.cn/gthjmrpjyg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hfpthk.cn/gtvgkezxwk.html

[C07] 把函数作为参数传入
来源：http://hz.yongpay.top/gtxobosowv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hywenlv.cn/gtmwmhajdz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinqigufen.top/gtrbpidccf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtyqvjzmwk.html

TS:   arr.map(String)
来源：http://hz.hnxiangtu.top/gtawcxhroi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydjk.org.cn/gtobpjsgtb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigufen.top/gtfekpsgby.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydjk.org.cn/gtyyuwibyl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtsbapfieo.html

[C08] 闭包
来源：http://hz.ydzc1.top/gtplkhepml.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhaomingkeji.xyz/gtbbhinqtm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuanzx.com/gtnwobmwac.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtosmguxyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtngnwdlrt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinyuanbaomall.cn/gtygcvffgt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hysaishi.cn/gtcdcryupx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.svipenyu.cn/gtfizaytal.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtqhlyqqlt.html

[C09] 递归
来源：http://hz.chenjidiqi.icu/gtzfilvbac.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtsnnirook.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhongyouzk.top/gtxtdjofpq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtiizhrzui.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtigsauely.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hysaishi.cn/gtkejmcirg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnqzz.top/gtqidujfjk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ywan-chungtsiang.top/gtdtwkfxfd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigfzy.top/gtreioxiey.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gttjfeahtk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhongyouzk.top/gtuvhvwbkf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtomrqljic.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yanxiufei.cn/gtgxvbfred.html

TS:   同 JS
来源：http://hz.hfpthk.cn/gtpizsmljp.html

Java: 方法内为块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtqvoraigk.html

Go:   花括号块级作用域
来源：http://hz.jqgufenzy.top/gtiqtudxzn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnqzz.top/gtowihjopy.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtoryckvoh.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtmwxtvxbz.html

Py:   from module import func
来源：http://hz.yvedp.cn/gtwoxfzupq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gtbjffmiaz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtlnzsyssf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.havefunace.top/gtupqsyjfa.html

Java: import java.util.List;
来源：http://hz.vqdsnc.cn/gtbvjvwcwp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xinyue.icu/gthyansxui.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gtnrpestea.html

C#:   using System.Text;
来源：http://hz.yj20258888.top/gtypqturdu.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtzwxyeenk.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtpleenoix.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cucudq.cn/gtuvczgevp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtldkajxmy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtzqippequ.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.mhx1999.top/gtwiabtewe.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtyrokuzhn.html

Ruby: -> { puts "run" }.call
来源：http://hz.kuanghao11.cn/gtdoynvdkf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jianghu66.top/gtdwevgjea.html

[C13] 类型声明 / 类型注解
来源：http://hz.guowangkeji.top/gtydaivqxq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtzzkkrekg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtojayaasa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.aibaodan.cn/gtbbjduqad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtwmakhtor.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtrvdbmtpq.html

Go:   func add(a, b int) int
来源：http://hz.jinqigufen.top/gtphrsqifo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.meibo888.top/gtylcgvrix.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.smart0.xyz/gtqnmlwjfe.html

[C14] 泛型函数
来源：http://hz.ydzc1.top/gttglbmdre.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhaomingkeji.xyz/gtxvkxxvlk.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtejybxqcr.html

JS:   // 无泛型
来源：http://hz.pengpengdd.cyou/gtgyughdkl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtnretvdbm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cqqwz.cn/gtnuitzhxx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hywenlv.cn/gtnqykhwpg.html

Ruby: # 无泛型
来源：http://hz.zhijiandao.cn/gtirzbqjko.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtbkcbpkpy.html

[C15] 解构 / 展开参数
来源：http://hz.sxryk.cn/gtpifylbde.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangtech.top/gtbvlpyqzq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guowangkeji.top/gthzsrardy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtzxuvakyg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jiagoushi.top/gtooscucaf.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtrytnneat.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtfpfrfkvh.html

Ruby: a, b = pair
来源：http://hz.aibaodan.cn/gthqdcdzzw.html

C#:   var (a, b) = pair;
来源：http://hz.wangshuangyany.cn/gtohbzmdvj.html

[C16] 函数 / 方法重载
来源：http://hz.shuidangran.top/gtsexsgffa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dashuyun.cn/gteaynvsyk.html

PHP:  // 无重载
来源：http://hz.haohaochexian.top/gtbhxqqnjo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.c1oappe.top/gtxmoxkooz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tanke756.top/gtvnorqikk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ppjwa.cn/gthqkcpcbm.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhaomingkeji.xyz/gtzhtjlytl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yonumen.top/gtdockweta.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.smart0.xyz/gtjgbgcsro.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgbmqjtjs.html

D. 数组 / 列表 / 集合
来源：http://hz.gotoacloud.top/gtfqtiyodv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgiugnmie.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gtvxzkcabz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hywenlv.cn/gtwgcbqnda.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shangyingyoupin.top/gtagdsiyxj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cashguo.top/gtnquupnha.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hysaishi.cn/gtfnjwnfqp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gtgunngrfd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sweek.top/gtvfqbwpzu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtxbizkmkw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.daxiang520.top/gthqhvfmxf.html

[D02] 追加元素到末尾
来源：http://hz.hfpthk.cn/gtsadhvmtu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenlongwang.top/gtyfqwtpzv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtbiakylwu.html

JS:   arr.push(4);
来源：http://hz.zhaomingkeji.xyz/gtxxpghbhh.html

TS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtfvmxnczl.html

Java: list.add(4);
来源：http://hz.xuanzx.com/gtppcnanbt.html

Go:   arr = append(arr, 4)
来源：http://hz.xylfe.cn/gtimjirjir.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258.top/gtbgrzbhzk.html

C#:   list.Add(4);
来源：http://hz.9152youxi.cn/gtiueeqndk.html

[D03] 在指定位置插入元素
来源：http://hz.jianghu66.top/gtwdhkpxzr.html

Py:   arr.insert(0, 0)
来源：http://hz.dashuyun.cn/gttwjedzqj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.svipenyu.cn/gtszoymvoe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daxiang520.top/gtivosalfk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.dashuyun.cn/gtrndlorrf.html

Java: list.add(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtualslgkj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cheryme.top/gtciwmomkc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xinyue.icu/gtabjiamtb.html

C#:   list.Insert(0, 0);
来源：http://hz.meibo888.top/gtqjgqruss.html

[D04] 删除元素
来源：http://hz.xylfe.cn/gtcyovamph.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtowlnylka.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258888.top/gtknrfqcfr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.svipenyu.cn/gtspodzttm.html

TS:   arr.splice(0, 1);
来源：http://hz.wangshuangyany.cn/gtpanfoyou.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gotoacloud.top/gtqhymxsbt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnxiangtu.top/gtiypyqrjz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtzwoypshd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gtpgzjjmpj.html

[D05] 访问与修改元素
来源：http://hz.xinyue.icu/gtasmwxinh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtjzroptow.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.mhx1999.top/gtucnkbohx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtbxaxbcgl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtcsclxiow.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtbmygtsyu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xylfe.cn/gtazdssoul.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtlpnjzqmi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yvedp.cn/gtktbsdjsa.html

[D06] 数组长度
来源：http://hz.kuanghao11.cn/gtlldjbhgy.html

Py:   len(arr)
来源：http://hz.nanxinkj.top/gtrilxixpa.html

PHP:  count($arr);
来源：http://hz.zycfv.cn/gtrjxzyxbx.html

JS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtmmhdziue.html

TS:   arr.length
来源：http://hz.zhongyouzk.top/gtuiclxjhe.html

Java: list.size();
来源：http://hz.svipenyu.cn/gtpmbehmrn.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtcowdutwq.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gtdhmhgunu.html

C#:   list.Count;
来源：http://hz.birdmap.top/gtbfeociwl.html

[D07] 切片 / 取子数组
来源：http://hz.zdqjudy.top/gtjjsbfykk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gtvvevsnvt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtepllxgbr.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtvkuuwofm.html

TS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtzlqydqju.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtpqtyhfzn.html

Go:   arr[1:4]
来源：http://hz.xuanzx.com/gtwjzxtxrx.html

Ruby: arr[1, 3]
来源：http://hz.dashuyun.cn/gtubtdwvzj.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhixingplan.top/gtvnztxeaq.html

[D08] 合并两个数组
来源：http://hz.xingfuxueyuan.xyz/gtzcimarzw.html

Py:   a + b;  a.extend(b)
来源：http://hz.aizwys.cn/gtwewbjtte.html

PHP:  array_merge($a, $b);
来源：http://hz.hysaishi.cn/gtyjuufymr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shuidangran.top/gtjricpcen.html

TS:   [...a, ...b];
来源：http://hz.pengpengdd.cyou/gtzhvxmtvj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenjidiqi.icu/gtdkvhuvei.html

Go:   append(a, b...)
来源：http://hz.wangdashe.top/gtzdziovfp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhaomingkeji.xyz/gtrcrnxrvz.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydjk.org.cn/gtidzarvcp.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtddldrcfm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtuuphgmzy.html


<!-- 参考信息 -->