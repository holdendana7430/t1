代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinyuanbaomall.cn/gtnhmgtlku.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xingfuxueyuan.xyz/gthlgjdkbh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gttqidculx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gthpitzejf.html

Java: do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtffbfjncg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sweek.top/gtngchiixk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sweek.top/gtuefoxiry.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtcxdxzsri.html

[B09] break 与 continue
来源：http://hz.zhoulong.xyz/gtdgnvjvqq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shanyushiyangtech.top/gtfrwbfcso.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.iojbl.cn/gtadqyevte.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtoeakalyc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtftwlkygv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtimtjqrcq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shanyushiyangkeji.top/gtionnlzbg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.feifeiyinyue.top/gtpwypyhmg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtjlgrxosz.html

[B10] 遍历同时拿索引
来源：http://hz.yanxiufei.cn/gtbofrynnj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.birdmap.top/gtzyrjjmvs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cucudq.cn/gtbugupdsn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daria6918.cn/gtfxhaevol.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinqigufen.top/gtdpuahprv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhongyouzk.top/gtzvytidom.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shzxlz.cn/gtvictcoij.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ywan-chungtsiang.top/gtnqgxnqao.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gogol.net.cn/gttqwnobqd.html

[B11] 生成数字序列 / 区间
来源：http://hz.kuanghao11.cn/gtuxoxllff.html

Py:   list(range(0, 10, 2))
来源：http://hz.yangfankeji.com/gtwlvpkcff.html

PHP:  range(0, 10, 2);
来源：http://hz.yangfankeji.com/gtaixzywwk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtabaaejcy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtpfxlrqsg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shangyingyoupin.top/gtrugkogpj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zdqjudy.top/gtydiczirg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.kuanghao11.cn/gtyifyfkmm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.wangshuangyany.cn/gtrnbkgkpx.html

[B12] 跳出多层循环
来源：http://hz.hysaishi.cn/gtezribwdm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.0kj1m.cn/gtkjkojxlq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhaomingkeji.xyz/gttjkegohu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gthfjikkqx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtnijspbcl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gttwroqqjz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinqigfzy.top/gtersvfisp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guowangkeji.top/gtexgnnrsp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.feifeiyinyue.top/gtojbfjvyp.html

[B13] 判断是否为数字
来源：http://hz.pengpengdd.cyou/gtfhqwyzkp.html

Py:   isinstance(x, (int, float))
来源：http://hz.zdqjudy.top/gtpelaoqcb.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtxcxvnutv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtrubdzbkd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtzkxxwzxy.html

Java: x instanceof Number
来源：http://hz.yj202588.top/gttapydips.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xinyue.icu/gtchgqhzoc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.svipenyu.cn/gtuldjktyq.html

C#:   x is int or double or decimal
来源：http://hz.zhongyouzk.top/gtajhahnde.html

[B14] 判断值是否在集合内
来源：http://hz.jianghu66.top/gtnbckedan.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangshuangyany.cn/gtqfqheiqb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydjk.org.cn/gtzdxuoimu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hywenlv.cn/gtlvtakver.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtwkptcfnq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxuanxn.top/gtcitauofp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.bjfxy.top/gtshgphugp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.c1oappe.top/gthnwynkxj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ivvv.top/gtmyaoibzn.html

[B15] 布尔运算与取反
来源：http://hz.hysaishi.cn/gtwagqydyi.html

Py:   a and b or not c
来源：http://hz.jyoumei.cn/gtrvpovyyr.html

PHP:  $a && $b || !$c
来源：http://hz.xuetiantiany.cn/gtxnszckyw.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtxpotscgq.html

TS:   a && b || !c
来源：http://hz.tian-w.cn/gtlbymxcxc.html

Java: a && b || !c
来源：http://hz.c1oappe.top/gtgclbkqpa.html

Go:   a && b || !c
来源：http://hz.nanxuanxn.top/gtzpvzfecv.html

Ruby: a && b || !c
来源：http://hz.yanxiufei.cn/gtuhxptlme.html

C#:   a && b || !c
来源：http://hz.guowangkeji.top/gttspyhxel.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtwgrzuklm.html

Py:   if not data: return
来源：http://hz.hongshengwenyu.top/gtgiwihwqy.html

PHP:  if (!$data) { return; }
来源：http://hz.meibo888.top/gtcnhtovat.html

JS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtyfvjdhtb.html

TS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gtkgcnfgyv.html

Java: if (data == null) return;
来源：http://hz.gzhubu.top/gtbjyitpmk.html

Go:   if data == nil { return }
来源：http://hz.havefunace.top/gtybadnern.html

Ruby: return if data.nil?
来源：http://hz.jqgfzy.top/gtxaapuxxc.html

C#:   if (data == null) return;
来源：http://hz.yonumen.top/gtsljpbzch.html

================================================================================
来源：http://hz.zdqjudy.top/gtmytbtpvh.html

C. 函数与作用域
来源：http://hz.nanxinkj.top/gtnevvvdhk.html

================================================================================
来源：http://hz.daria6918.cn/gtllrekuiv.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gtxxhlzwaw.html

Py:   def add(a, b): return a + b
来源：http://hz.ybcxt.top/gtrtnlcfpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtfsphqhka.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.snrcjt.cn/gtytnpjava.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yanxiufei.cn/gtjezregfb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gthrhihmjv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hfpthk.cn/gtkbvvdwuz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tian-w.cn/gtpsdtngth.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtglgdzaqr.html

[C02] 默认参数
来源：http://hz.hnxiangtu.top/gtqddnlnru.html

Py:   def greet(name="World"): return name
来源：http://hz.xinyue.icu/gtsqkjlxxt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pycfn.com/gtggdrsyzr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.aibaodan.cn/gtpumuracc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.kuanghao11.cn/gtylfsrasd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenjidiqi.icu/gtouglfhtv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtpmhvocjd.html

Ruby: def greet(name = "World") = name
来源：http://hz.shangyingyoupin.top/gtagzxjsuo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.iojbl.cn/gtbwtmkwim.html

[C03] 可变参数
来源：http://hz.jqgfzy.top/gtsmjrhvvb.html

Py:   def total(*args): return sum(args)
来源：http://hz.52xcode.cn/gtjwkuidim.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.c1oappe.top/gtypopgdkg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtdtvsppcf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gttvdkyumh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydzc1.top/gtgqjqkgqs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnxiangtu.top/gtdkrqefpj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yangfankeji.com/gtfdxbkicc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.52xcode.cn/gtopweyluy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ywan-chungtsiang.top/gtwrhgobso.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ivvv.top/gtkpvvxfff.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aibaodan.cn/gtlkdyywwt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtnaxkffcr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtywyxkdqg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.meibo888.top/gtuywalxyo.html

Go:   // 无：用配置结构体参数
来源：http://hz.wangdashe.top/gtoyffairz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtmrqloyye.html

C#:   f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtqduoveai.html

[C05] 返回多个值
来源：http://hz.yangfankeji.com/gtwelbngfz.html

Py:   return a, b
来源：http://hz.shangyingyoupin.top/gtxxkglcbv.html

PHP:  return [$a, $b];
来源：http://hz.hammf.cn/gtmaniqiub.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sysykeji.top/gtoasthlss.html

TS:   return { a, b };
来源：http://hz.jlsjyb.cn/gtkzfsihzs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gogol.net.cn/gtcupsetlt.html

Go:   return a, b
来源：http://hz.xuetiantiany.cn/gtgtimjsnv.html

Ruby: return a, b
来源：http://hz.gzhubu.top/gtodnixvpc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dashuyun.cn/gtxttdwuth.html

[C06] 匿名函数 / lambda
来源：http://hz.jinghuilouyu.cn/gtmjixxodw.html

Py:   square = lambda x: x * x
来源：http://hz.nanxinkj.top/gtdualljwo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yueranfly.top/gtquyscwga.html

JS:   const square = x => x * x;
来源：http://hz.daxiang520.top/gtemlqxflb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtwefnykvx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangdashe.top/gtysyxhhzv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.andypj.xyz/gtgptxivlg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydzc1.top/gtsihioifs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.mhx1999.top/gtekihhjwb.html

[C07] 把函数作为参数传入
来源：http://hz.ydjk.org.cn/gthlnyhlty.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gttplpkigl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnqzz.top/gtqynhgzza.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtxqjjuwgx.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtwjgdkvss.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuanzhike.top/gtjobyishy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ybcxt.top/gtydszlcoo.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258888.top/gtytxpigea.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigfzy.top/gtszbiokpz.html

[C08] 闭包
来源：http://hz.zycfv.cn/gtqqzskyjx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daria6918.cn/gtklyslysg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.bjfxy.top/gtxutzjuts.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtzyekqyyg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtfmmnftba.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangdashe.top/gtefdxsfew.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangkeji.top/gtkrsnzlzd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yangfankeji.com/gtdhvgdqzt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtakdxbymm.html

[C09] 递归
来源：http://hz.jyoumei.cn/gttaqxyvbe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtxdkrhurj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtfprvrken.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtkcsiknom.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtikhvujre.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gtmldsyhga.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258888.top/gtdvfuhzny.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tian-w.cn/gtdgxwvbcw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.meibo888.top/gtevgyijep.html

[C10] 变量作用域
来源：http://hz.jinghuilouyu.cn/gtvfrkxkep.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtznlbluyk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gthwpjigxb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dianchejie.cn/gtoleeiqig.html

TS:   同 JS
来源：http://hz.yuxming.cn/gtrujnaqcq.html

Java: 方法内为块级作用域
来源：http://hz.xziqi.cn/gtbwqblusu.html

Go:   花括号块级作用域
来源：http://hz.0kj1m.cn/gtfosmfkam.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gaohongyu789.top/gtfeatiljq.html

C#:   块级作用域
来源：http://hz.ehwqpu.com/gtkrsopxvv.html

[C11] 模块导入与导出
来源：http://hz.ydjk.org.cn/gtuaephvul.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtxlmbpbje.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.vqdsnc.cn/gtwpvrkyjq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtnkmjihdy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.smart0.xyz/gtwvrfpkmn.html

Java: import java.util.List;
来源：http://hz.shanyushiyangtech.top/gtxctgnlwi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.wangshuangyany.cn/gtpvrqhbwc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shanyushiyangtech.top/gtzcbunurv.html

C#:   using System.Text;
来源：http://hz.hfpthk.cn/gtbdajsczu.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtngvqmaht.html

Py:   (lambda: print("run"))()
来源：http://hz.tianlin.xyz/gtxvdnabsh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gtxghurhrz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pycfn.com/gtvdmbltlh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtosebpxtr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xylfe.cn/gtltftwsre.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangtech.top/gtsmrvoaoe.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgfzy.top/gttaumeoyv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nwbrower.top/gttzecagiq.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangdashe.top/gtsylzxbjp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gtaowuhalk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtnhyniczw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.aibaodan.cn/gtlxkcdwvh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtzdtlzqdo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtcurjftkv.html

Go:   func add(a, b int) int
来源：http://hz.yanxiufei.cn/gtqvrijjos.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zycfv.cn/gtgznytpdx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.bjfxy.top/gtwdjmwney.html

[C14] 泛型函数
来源：http://hz.havefunace.top/gtqijxxbpc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yangfankeji.com/gtqqtywljc.html

PHP:  // 无泛型
来源：http://hz.yueranfly.top/gtdyvnrlbf.html

JS:   // 无泛型
来源：http://hz.jinghuilouyu.cn/gtgalmrfto.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtioubtbem.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.vqdsnc.cn/gtswdpgpcq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tianlin.xyz/gtxntdcciw.html

Ruby: # 无泛型
来源：http://hz.jiagoushi.top/gtmlvoecsq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gthknmsprq.html

[C15] 解构 / 展开参数
来源：http://hz.9152youxi.cn/gtrsaxtbil.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daria6918.cn/gtcjgivwfc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtljvjuqyu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydjk.org.cn/gtrricvdzc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yanxiufei.cn/gtfcjydhqr.html

Java: // 无解构
来源：http://hz.shuidangran.top/gtjvviwvaz.html

Go:   // 无解构
来源：http://hz.guannengcc.top/gtzcvtpqci.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gteslybavo.html

C#:   var (a, b) = pair;
来源：http://hz.tanke756.top/gtbxbxlmfm.html

[C16] 函数 / 方法重载
来源：http://hz.shzxlz.cn/gtevgbccta.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sweek.top/gthlqcxbwg.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtsceatuyn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuxming.cn/gtjxhnrxzs.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xingfuxueyuan.xyz/gtctmkphry.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zycfv.cn/gtgiojqctu.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgfzy.top/gtyafeoikq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shzxlz.cn/gtfrgqcxso.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangshuangyany.cn/gtichcxzvb.html

================================================================================
来源：http://hz.hywenlv.cn/gtfqkofvwj.html

D. 数组 / 列表 / 集合
来源：http://hz.jiagoushi.top/gtdeppgfry.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgisdrxew.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gthipamdxz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnqzz.top/gtvuvoooxx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aibaodan.cn/gtngvwffys.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtfingdoue.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yvedp.cn/gtbxlpfjln.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.birdmap.top/gtgwotuyjx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cashguo.top/gtajtwcytq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hammf.cn/gtwejlyyah.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gtyjdsusce.html

[D02] 追加元素到末尾
来源：http://hz.dianchejie.cn/gtukhawvmh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj202588.top/gtchrwwejh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinghuilouyu.cn/gtfdfuibbl.html

JS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gthijtkfrh.html

TS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtefwekaff.html

Java: list.add(4);
来源：http://hz.haohaochexian.top/gtxytwrdbs.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtqfachzdo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tian-w.cn/gtvewwpagj.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gtytzcbmql.html

[D03] 在指定位置插入元素
来源：http://hz.smart0.xyz/gtedysifaw.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gtbthgddpk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gogol.net.cn/gtdhsyzvob.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtdxjwicyh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigufen.top/gtkzdpyyda.html

Java: list.add(0, 0);
来源：http://hz.zhijiandao.cn/gtqaozubhq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtfgzkvcxp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shangyingyoupin.top/gtsxaoyavt.html

C#:   list.Insert(0, 0);
来源：http://hz.aibaodan.cn/gthbpilwxt.html

[D04] 删除元素
来源：http://hz.redwolf501.top/gtqyglpxxj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gtwnsazbpq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dianchejie.cn/gtpuiiheiz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gtgemebvcc.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gtavifwwst.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangshuangyany.cn/gtweuvmled.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gtwclxouiz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgufenzy.top/gtqzpsdntg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.haohaochexian.top/gtyrzbuqqx.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gtteetcckv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtqrgbdhwe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuanzx.com/gtiyrahpmd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.haohaochexian.top/gtcpizqufh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhijiandao.cn/gtuolnidyl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydjk.org.cn/gtqykfeddp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daria6918.cn/gtgtxhubdm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtkuwrhpbm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtifhfdbmr.html

[D06] 数组长度
来源：http://hz.cashguo.top/gtxoxedvoh.html

Py:   len(arr)
来源：http://hz.ydzc1.top/gtgysrgztk.html

PHP:  count($arr);
来源：http://hz.jqgfzy.top/gtxoajkbub.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gtzlalwvdr.html

TS:   arr.length
来源：http://hz.vqdsnc.cn/gtjufkkoih.html

Java: list.size();
来源：http://hz.wangdashe.top/gtqvxgkecq.html

Go:   len(arr)
来源：http://hz.feifeiyinyue.top/gtceshcors.html

Ruby: arr.length; arr.size
来源：http://hz.snrcjt.cn/gtnftadluz.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtqivgxmls.html

[D07] 切片 / 取子数组
来源：http://hz.jyoumei.cn/gtgoterust.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhoulong.xyz/gtfuxaatzn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.mhx1999.top/gtfvlcbnuq.html

JS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gttvgoluui.html

TS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gthmgjkmnt.html

Java: list.subList(1, 4);
来源：http://hz.yanxiufei.cn/gtcguwgxwb.html

Go:   arr[1:4]
来源：http://hz.kuanghao11.cn/gtbgudwznn.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gtcrihhzsn.html

C#:   list.GetRange(1, 3);
来源：http://hz.52xcode.cn/gtssswznru.html

[D08] 合并两个数组
来源：http://hz.0kj1m.cn/gtewfvtkgz.html

Py:   a + b;  a.extend(b)
来源：http://hz.haohaochexian.top/gtyanzwsph.html

PHP:  array_merge($a, $b);
来源：http://hz.ybcxt.top/gtcwuudjhi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangkeji.top/gtbkoumtox.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtffknhcgu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtptrqumgh.html

Go:   append(a, b...)
来源：http://hz.nanxuanxn.top/gtywxldmzm.html


<!-- 参考信息 -->