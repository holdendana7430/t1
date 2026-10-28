代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.meibo888.top/gtjnjqzjuz.html

JS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtvzsqnncy.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtxeuvsjcb.html

Java: while (i < 10) { i++; }
来源：http://hz.svipenyu.cn/gtuvsklpbz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cucudq.cn/gtzkvapcnq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jyoumei.cn/gtgmhigjbx.html

C#:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtfjvyqltj.html

[B08] do-while（至少执行一次）
来源：http://hz.andypj.xyz/gtysgkmkat.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sysykeji.top/gtijlebkif.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ivvv.top/gtisyevtrz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtjqbrtrmp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtoiwdlajc.html

Java: do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtaiimbjbc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhixingplan.top/gterhhamqq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinqigufen.top/gtilnqzceg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.pengpengdd.cyou/gtnvepfhkv.html

[B09] break 与 continue
来源：http://hz.kuanghao11.cn/gtltldgjcx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.kuanghao11.cn/gtlqjvyufz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.snrcjt.cn/gtaogcjfps.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtzglofozd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtxxodkljg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtndxmnnaj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258.top/gtyygspudl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cheryme.top/gtcyverrjw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtttbvzyuq.html

[B10] 遍历同时拿索引
来源：http://hz.316326.xyz/gtzntgwtzm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tianlin.xyz/gtnyxzrbwn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zycfv.cn/gtkedqpmpd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtpxytumuy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.316326.xyz/gtmvonackn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.aizwys.cn/gtubffbgbd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258.top/gtikgpqhxk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangshuangyany.cn/gtszbswfcl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.c1oappe.top/gtdqghvrhj.html

[B11] 生成数字序列 / 区间
来源：http://hz.mhx1999.top/gtztmzklhr.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhengqikj.top/gtbbprpqcb.html

PHP:  range(0, 10, 2);
来源：http://hz.ppjwa.cn/gthbunwdjy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigufen.top/gtsnrdrntn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nwbrower.top/gtwuqlpgij.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aibaodan.cn/gtrpovnqyj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.smart0.xyz/gtakfibbux.html

Ruby: (0...10).step(2).to_a
来源：http://hz.meibo888.top/gtbmzdojqz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shzxlz.cn/gtuwfcngqp.html

[B12] 跳出多层循环
来源：http://hz.c1oappe.top/gtdhqnqvyq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yuxming.cn/gtereiufgs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sysykeji.top/gtuirqenzp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtuxqfwuvz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gtgqryjbji.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gogol.net.cn/gtehhatauf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydjk.org.cn/gtjsmtlcvo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhoulong.xyz/gtchyaksqc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tanke756.top/gtlxbenhqh.html

[B13] 判断是否为数字
来源：http://hz.havefunace.top/gtrmayhprp.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhiwuduotai.top/gtswvyeqbk.html

PHP:  is_numeric($x)
来源：http://hz.kuanghao11.cn/gtilgloxoc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gzhubu.top/gtjwfuqiop.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gtokqodssp.html

Java: x instanceof Number
来源：http://hz.gogol.net.cn/gtvhbuvctz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zycfv.cn/gtqsckvrsn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hywenlv.cn/gthtftxlwj.html

C#:   x is int or double or decimal
来源：http://hz.jlsjyb.cn/gteuumiqfw.html

[B14] 判断值是否在集合内
来源：http://hz.wangdashe.top/gtdvxzhvub.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gotoacloud.top/gtkpxpphvy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhoulong.xyz/gtighhqkpn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gotoacloud.top/gtcwdsrbpt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtkiifyubv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tian-w.cn/gtppuxgksx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.c1oappe.top/gtsjnnhmye.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258.top/gthwgwzobe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cqqwz.cn/gtwdnmcatd.html

[B15] 布尔运算与取反
来源：http://hz.meibo888.top/gtzsdttnyd.html

Py:   a and b or not c
来源：http://hz.tianlin.xyz/gtqsvkwyoy.html

PHP:  $a && $b || !$c
来源：http://hz.cdnleiting.top/gtqrxvagup.html

JS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtkfjugdqx.html

TS:   a && b || !c
来源：http://hz.tianlin.xyz/gtprginfpg.html

Java: a && b || !c
来源：http://hz.daxiang520.top/gtlkjxwajz.html

Go:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtrhqmgsuk.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gtpvvfahmt.html

C#:   a && b || !c
来源：http://hz.52xcode.cn/gtvuutwged.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xuetiantiany.cn/gtuliwbssh.html

Py:   if not data: return
来源：http://hz.quarkkingdee.top/gtwxtmiaqj.html

PHP:  if (!$data) { return; }
来源：http://hz.smart0.xyz/gtdhgnrwwz.html

JS:   if (!data) return;
来源：http://hz.hysaishi.cn/gtcflpuojs.html

TS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gtannxpsqn.html

Java: if (data == null) return;
来源：http://hz.fengsongda.top/gtiwvryqpl.html

Go:   if data == nil { return }
来源：http://hz.jiagoushi.top/gtbbsomsmh.html

Ruby: return if data.nil?
来源：http://hz.ehwqpu.com/gtdyjfmtnw.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtwhgdnuaj.html

================================================================================
来源：http://hz.redwolf501.top/gthbghiygm.html

C. 函数与作用域
来源：http://hz.guowangkeji.top/gtsibeioto.html

================================================================================
来源：http://hz.zhoulong.xyz/gtahjzamtr.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtygjfnivc.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtktkglglf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtiaojvbqg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gttdvzysky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtbieffmng.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtftvleyjy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.9152youxi.cn/gtotuzbgun.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnxiangtu.top/gtnlxttniv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtrxxjtxgb.html

[C02] 默认参数
来源：http://hz.zycfv.cn/gtzsaigawd.html

Py:   def greet(name="World"): return name
来源：http://hz.cheryme.top/gtmzoukvfw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aizwys.cn/gtzehittpg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtacxamxpe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gogol.net.cn/gtfuplqwfc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.svipenyu.cn/gtdfldccuw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tianlin.xyz/gtqdmnxfpc.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuxming.cn/gtgauogwbr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhixingplan.top/gtgtbzqnzx.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gtitziqizi.html

Py:   def total(*args): return sum(args)
来源：http://hz.guowangkeji.top/gtvbqiozpj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ybcxt.top/gtktgkdyxi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sweek.top/gtryzvybyt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtsqbskenl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258.top/gthxhxkpao.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yanxiufei.cn/gtzlzknwtd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jqgufenzy.top/gtuxcxzdyi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gtonblbaeh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgfzy.top/gtelskwuwp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhoulong.xyz/gtdmzcpycz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenlongwang.top/gtdfaaoquu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtcexumjbo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yongpay.top/gtozgtbomj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guowangkeji.top/gttgicnxar.html

Go:   // 无：用配置结构体参数
来源：http://hz.tanke756.top/gtcxgjteqx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtabhpdylj.html

C#:   f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gteybluwgs.html

[C05] 返回多个值
来源：http://hz.ywan-chungtsiang.top/gtykiqxdne.html

Py:   return a, b
来源：http://hz.bjfxy.top/gtetpgzgth.html

PHP:  return [$a, $b];
来源：http://hz.hywenlv.cn/gttzoygpar.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.316326.xyz/gtiiktlerq.html

TS:   return { a, b };
来源：http://hz.tian-w.cn/gtmgeqxkzx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.c1oappe.top/gtsjzsbrwp.html

Go:   return a, b
来源：http://hz.daxiang520.top/gtbytvouhl.html

Ruby: return a, b
来源：http://hz.nwbrower.top/gttzsvejaz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.mhx1999.top/gtywgysily.html

[C06] 匿名函数 / lambda
来源：http://hz.nanxuanxn.top/gtsccxlsek.html

Py:   square = lambda x: x * x
来源：http://hz.jianghu66.top/gtkglmvujg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangkeji.top/gttsuecerh.html

JS:   const square = x => x * x;
来源：http://hz.ivvv.top/gtwcmsacyk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtgwunseiw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gtfzogqirg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tian-w.cn/gtckrxkftk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangtech.top/gthoopjjoo.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.iojbl.cn/gtyfapyscy.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigfzy.top/gtippzoeyb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yvedp.cn/gtdrlcdedq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.9152youxi.cn/gtjisgosmr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnqzz.top/gtzcxfivuf.html

TS:   arr.map(String)
来源：http://hz.ydjk.org.cn/gtarhloyvu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.kuanghao11.cn/gttsmgwxra.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.quarkkingdee.top/gtfumexwmj.html

Ruby: arr.map(&:upcase)
来源：http://hz.xziqi.cn/gtlcakeyxl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ybcxt.top/gtrucmjjxh.html

[C08] 闭包
来源：http://hz.tanke756.top/gtsmkpbhuk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aizwys.cn/gtqfypdwum.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtazwytbzf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gttjajkvbf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtrkdahgkd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtctcqfyhb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhiwuduotai.top/gtkqylgacy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinyuanbaomall.cn/gtoytkucvg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtaxucgmmc.html

[C09] 递归
来源：http://hz.yueranfly.top/gtbjcostkl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.tanke756.top/gtrdupubbr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gotoacloud.top/gtzxeawchj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtcvzlndln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtyilpqtld.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gtcytbscmt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.bjfxy.top/gtqhbhkqbc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xinyue.icu/gtktvvxbzu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gtyqjqpirn.html

[C10] 变量作用域
来源：http://hz.gzhubu.top/gtajdajdmw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhoulong.xyz/gtulieurpq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cdnleiting.top/gtelietdwg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtdlofdaar.html

TS:   同 JS
来源：http://hz.gogol.net.cn/gtqgmxrvvl.html

Java: 方法内为块级作用域
来源：http://hz.redwolf501.top/gtoqwzegjq.html

Go:   花括号块级作用域
来源：http://hz.yanxiufei.cn/gtoisgfpxb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sweek.top/gtpcrjoxlc.html

C#:   块级作用域
来源：http://hz.ydjk.org.cn/gtyapldufx.html

[C11] 模块导入与导出
来源：http://hz.yj20258888.top/gtswfhsxjr.html

Py:   from module import func
来源：http://hz.iojbl.cn/gtjnzyztop.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yanxiufei.cn/gtqxdvptku.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hfpthk.cn/gtiixqmrbg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.feifeiyinyue.top/gtsdtpnxob.html

Java: import java.util.List;
来源：http://hz.jlsjyb.cn/gtzjknwdbt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.daria6918.cn/gtkwwdgnhn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtnlrymtlp.html

C#:   using System.Text;
来源：http://hz.zhongyouzk.top/gtwxcvsqpo.html

[C12] 立即执行函数 IIFE
来源：http://hz.haohaochexian.top/gtaegyzqdc.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gtmuakcsdj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigufen.top/gteqcmlfyn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtpzbtfudk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtborgmnvi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yangfankeji.com/gtusosjaap.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtntdwqwva.html

Ruby: -> { puts "run" }.call
来源：http://hz.yvedp.cn/gtsxdcwiet.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhijiandao.cn/gtjofbnfhc.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtcpyfnbcn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtqcewwdas.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtdqumeien.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxuanxn.top/gtnzrggftn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtcjerhhtb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtfjejxjdg.html

Go:   func add(a, b int) int
来源：http://hz.zhijiandao.cn/gtqtifxoib.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtascaltmj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xinyue.icu/gtvaybrkvu.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtgvempbup.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ydzc1.top/gtfyczysic.html

PHP:  // 无泛型
来源：http://hz.tanke756.top/gtlfuxqiux.html

JS:   // 无泛型
来源：http://hz.hnqzz.top/gtqydjzpmr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zycfv.cn/gtdxhfxoaq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtygbvshwe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinghuilouyu.cn/gtzhoabcox.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gtyakwmkmz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gogol.net.cn/gtcmjqumey.html

[C15] 解构 / 展开参数
来源：http://hz.zdqjudy.top/gtolkbwluh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigfzy.top/gtecllrjow.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhoulong.xyz/gttjgbwrav.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtehwlofxw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dianchejie.cn/gtkjnijmpn.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtfiwsxcdv.html

Go:   // 无解构
来源：http://hz.zhixingplan.top/gtvovqzras.html

Ruby: a, b = pair
来源：http://hz.nwbrower.top/gtbuawkrzx.html

C#:   var (a, b) = pair;
来源：http://hz.andypj.xyz/gtunbjzgna.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangkeji.top/gtdobipbtg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtkicfcpig.html

PHP:  // 无重载
来源：http://hz.dashuyun.cn/gteilmyquh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnxiangtu.top/gthvfeobtc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtnecengmq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtonhswhje.html

Go:   // 无重载：用不同函数名
来源：http://hz.fzhhl.top/gtuiwizoaq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhengqikj.top/gttorilsme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnxiangtu.top/gtqntdqwjy.html

================================================================================
来源：http://hz.jqgfzy.top/gteyjjxgox.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtsgbqlhah.html

================================================================================
来源：http://hz.0kj1m.cn/gtvttipnxe.html

[D01] 创建数组 / 列表
来源：http://hz.316326.xyz/gtukilvqsr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gtveucvtqs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinyuanbaomall.cn/gtcrjalihc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtuvwyawhi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cashguo.top/gtuofamefe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gtfsckbbim.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.haohaochexian.top/gtkwgovdad.html

Ruby: arr = [1, 2, 3]
来源：http://hz.svipenyu.cn/gtfmnhwjuw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.havefunace.top/gtbgsplqeg.html

[D02] 追加元素到末尾
来源：http://hz.9152youxi.cn/gtykslqhtx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuetiantiany.cn/gtfkrkufac.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yanxiufei.cn/gtdsbnfzbw.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtkdghkstb.html

TS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtcgtykptv.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtvwezhfru.html

Go:   arr = append(arr, 4)
来源：http://hz.9152youxi.cn/gtgtxncksn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xingfuxueyuan.xyz/gtjzgjojqu.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtafcuejku.html

[D03] 在指定位置插入元素
来源：http://hz.ydzc1.top/gtgybfwopb.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gtgpulekbe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtylphdlbl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.meibo888.top/gtzraidqxe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xylfe.cn/gtuctazgyq.html

Java: list.add(0, 0);
来源：http://hz.chenjidiqi.icu/gtlukeriph.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangdashe.top/gtgfsozhju.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.havefunace.top/gtadayfrft.html

C#:   list.Insert(0, 0);
来源：http://hz.zhiwuduotai.top/gtbhosayhl.html

[D04] 删除元素
来源：http://hz.quarkkingdee.top/gtqpchtfye.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtzsbzqqxe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xinyue.icu/gtfshzyfkr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydjk.org.cn/gtxkewfpya.html

TS:   arr.splice(0, 1);
来源：http://hz.yanxiufei.cn/gtfqwpvtoe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gtikztmcec.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ivvv.top/gtayfghuju.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tanke756.top/gtqgmfiwel.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gtfcmwvafe.html

[D05] 访问与修改元素
来源：http://hz.yangfankeji.com/gtsssvtmap.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtwdhyjpoa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtuqqpiqcx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtgtxluqdj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenlongwang.top/gtkzbvibgz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hysaishi.cn/gttbgnrsls.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtihgpicgr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtkazvtqvh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtrozepjnj.html

[D06] 数组长度
来源：http://hz.chenlongwang.top/gtiadkhium.html

Py:   len(arr)
来源：http://hz.hywenlv.cn/gtbamhmsrl.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gtvptebmdy.html

JS:   arr.length
来源：http://hz.xingfuxueyuan.xyz/gtreyluvfi.html

TS:   arr.length
来源：http://hz.fzhhl.top/gtrybwbexq.html

Java: list.size();
来源：http://hz.sufxvd.cn/gtmejhcprs.html

Go:   len(arr)
来源：http://hz.ehwqpu.com/gtczbentpn.html

Ruby: arr.length; arr.size
来源：http://hz.cqqwz.cn/gtggvbsqrq.html

C#:   list.Count;
来源：http://hz.xuetiantiany.cn/gtenpguxcq.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gttcnacuqy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtzbnozovo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtglaxfhlu.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gticceevxq.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtkcuniudj.html

Java: list.subList(1, 4);
来源：http://hz.sxryk.cn/gtyxddhiet.html

Go:   arr[1:4]
来源：http://hz.meibo888.top/gtaatbftfk.html

Ruby: arr[1, 3]
来源：http://hz.zycfv.cn/gtjdjznmxu.html


<!-- 参考信息 -->