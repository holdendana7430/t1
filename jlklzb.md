代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.haohaochexian.top/gtzllbmvly.html

JS:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtwladohqk.html

TS:   while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtpzwowcut.html

Java: while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtlhdhnwkm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xylfe.cn/gtjkgftzpy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nwbrower.top/gtjrhqyxhc.html

C#:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtjmztxkqg.html

[B08] do-while（至少执行一次）
来源：http://hz.redwolf501.top/gtirgrxleu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258888.top/gtpwdvtiwh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gtohkdelae.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtuprnmlld.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtddpwbhlk.html

Java: do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtrnwbtkbm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xuanzx.com/gtiioibodx.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zdqjudy.top/gtmkrbxhop.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtowbnkgsj.html

[B09] break 与 continue
来源：http://hz.cashguo.top/gtvahyxqcu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.andypj.xyz/gtvlzawrxn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cashguo.top/gtjbvztwyb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtlwagvmgf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtsdnzzflb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zycfv.cn/gtsxokobuc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.bjfxy.top/gtezautfdx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.snrcjt.cn/gtwusdexcb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gthfascaki.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gtkgoasicr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangdashe.top/gtfduolhsq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daria6918.cn/gtzbpzizub.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gttlpwanjz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.daria6918.cn/gtvjfmjgfm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guowangkeji.top/gtdvjvygce.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sxryk.cn/gtsiakpcxz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.c1oappe.top/gtfplvqugs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sxryk.cn/gtlujlnsew.html

[B11] 生成数字序列 / 区间
来源：http://hz.ehwqpu.com/gtquebuadz.html

Py:   list(range(0, 10, 2))
来源：http://hz.52xcode.cn/gttyohvrcw.html

PHP:  range(0, 10, 2);
来源：http://hz.c1oappe.top/gtqmmywnvx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.316326.xyz/gtfcftkgfe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cheryme.top/gtrelwlugl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.daxiang520.top/gtinjiswbs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258.top/gtarnzfhui.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenlongwang.top/gtmpnciqux.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gzhubu.top/gtnpehlupn.html

[B12] 跳出多层循环
来源：http://hz.haohaochexian.top/gtgepmnshn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ydjk.org.cn/gtqvhkrswd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aibaodan.cn/gtnfwsiafs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hfpthk.cn/gtlaofdkdr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtdxnzjcqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtfclqlbhi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jqgfzy.top/gtkhxrxhvg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ywan-chungtsiang.top/gtufsfqtps.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daxiang520.top/gtjnienerb.html

[B13] 判断是否为数字
来源：http://hz.gzhubu.top/gttxqtipbw.html

Py:   isinstance(x, (int, float))
来源：http://hz.feifeiyinyue.top/gtkhweyqst.html

PHP:  is_numeric($x)
来源：http://hz.snrcjt.cn/gtqkssfude.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guannengcc.top/gtpnacniiy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtttfunmdo.html

Java: x instanceof Number
来源：http://hz.ybcxt.top/gtbfuujqaf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hywenlv.cn/gthzsaoonj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gtlfebngrf.html

C#:   x is int or double or decimal
来源：http://hz.quarkkingdee.top/gtzfqczrco.html

[B14] 判断值是否在集合内
来源：http://hz.shanyushiyangkeji.top/gtxeifbofa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.fzhhl.top/gtjtnqlvhs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinqigufen.top/gtpirlilpt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gttjwaoxbl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gthqbjgihs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yueranfly.top/gtdzfztrtc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtcsproemg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.svipenyu.cn/gtnijmiuhm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jianghu66.top/gtwpdeuvud.html

[B15] 布尔运算与取反
来源：http://hz.smart0.xyz/gtexlopiff.html

Py:   a and b or not c
来源：http://hz.0kj1m.cn/gtahxbgabv.html

PHP:  $a && $b || !$c
来源：http://hz.cucudq.cn/gtakdbabhe.html

JS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtnskvdwof.html

TS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gthyanlome.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gteiijvbjt.html

Go:   a && b || !c
来源：http://hz.nanxinkj.top/gtcseinjzm.html

Ruby: a && b || !c
来源：http://hz.cqqwz.cn/gtjechhdmr.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtaodgijdw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ppjwa.cn/gtwhbfwkxn.html

Py:   if not data: return
来源：http://hz.zhixingplan.top/gtzsdrrmbw.html

PHP:  if (!$data) { return; }
来源：http://hz.smart0.xyz/gtwnqiapjk.html

JS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtsjwnizkb.html

TS:   if (!data) return;
来源：http://hz.snrcjt.cn/gtixgxrilq.html

Java: if (data == null) return;
来源：http://hz.sysykeji.top/gthunqybyb.html

Go:   if data == nil { return }
来源：http://hz.tianlin.xyz/gtjahdgket.html

Ruby: return if data.nil?
来源：http://hz.dashuyun.cn/gtqpvuamsp.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtaglqcive.html

================================================================================
来源：http://hz.yonumen.top/gtcvonyczm.html

C. 函数与作用域
来源：http://hz.gogol.net.cn/gtpargcwlm.html

================================================================================
来源：http://hz.gotoacloud.top/gteyurnglu.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gtjmtpqdfb.html

Py:   def add(a, b): return a + b
来源：http://hz.hnxiangtu.top/gthgqjpqdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtiupqudjw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtwsgyjrbw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtfvdezjgq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtffjkrlkw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgfzy.top/gtuhibwdhe.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258.top/gtwajonbmu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtkmgtodce.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtodzkvhni.html

Py:   def greet(name="World"): return name
来源：http://hz.zycfv.cn/gtwliwlxqx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shuidangran.top/gtdcsldktu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigfzy.top/gtdxpstavz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jiagoushi.top/gtmgswsbcs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xziqi.cn/gtmafsgrdw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hysaishi.cn/gtfivfcyif.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtlgyoikgv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.pengpengdd.cyou/gtkrmzatug.html

[C03] 可变参数
来源：http://hz.zdqjudy.top/gtztxvflrv.html

Py:   def total(*args): return sum(args)
来源：http://hz.aizwys.cn/gtmhikqszf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xziqi.cn/gtncvogwpx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gtnkwnxjmu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtikvwabwn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenlongwang.top/gtwplelmwf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.kuanghao11.cn/gthymazqrp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ivvv.top/gtotkfwzff.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hongshengwenyu.top/gtjoddjjiq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtiqmjefrp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.9152youxi.cn/gtnlhntvba.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shangyingyoupin.top/gtbqjcwuhz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.fengsongda.top/gtmjkccwqf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.quarkkingdee.top/gthwdoqcjy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gtgopbmalw.html

Go:   // 无：用配置结构体参数
来源：http://hz.havefunace.top/gtzbmnafai.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtzberychh.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtwvkgwpyf.html

[C05] 返回多个值
来源：http://hz.ehwqpu.com/gtbgdiibng.html

Py:   return a, b
来源：http://hz.ehwqpu.com/gttyypofdv.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gtixwijvrk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.iojbl.cn/gtpgcmuweb.html

TS:   return { a, b };
来源：http://hz.zhoulong.xyz/gtcgkusmid.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258888.top/gtrmwzgqja.html

Go:   return a, b
来源：http://hz.hfpthk.cn/gtqwmofzls.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gteewsdfdw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtkwqmkthn.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtypddgddr.html

Py:   square = lambda x: x * x
来源：http://hz.zhengqikj.top/gtkvacekdw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xinyue.icu/gtlqaiovfs.html

JS:   const square = x => x * x;
来源：http://hz.quarkkingdee.top/gtlhxoqppx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.haohaochexian.top/gtrrtzmqce.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.bjfxy.top/gtijkcxpte.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.haohaochexian.top/gtcxfmbfrr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangdashe.top/gtnrdwcatb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.fzhhl.top/gtohzpgkil.html

[C07] 把函数作为参数传入
来源：http://hz.shangyingyoupin.top/gtnfdtcvdd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhixingplan.top/gtcblazyef.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhiwuduotai.top/gtnmztjdft.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gtohimefuh.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gtyslgkbiz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenzaomai.com/gtqszwmbrt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuxming.cn/gtkzyjjsyd.html

Ruby: arr.map(&:upcase)
来源：http://hz.cheryme.top/gtnuektqzc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guowangkeji.top/gtavrkqajj.html

[C08] 闭包
来源：http://hz.meibo888.top/gtptjjkiuj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ppjwa.cn/gtaldnhwyf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cdnleiting.top/gtprihpqrs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtmeyigxkt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtcqwtgkrb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ppjwa.cn/gtwvqzkomv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgfzy.top/gtcwvkdcst.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ybcxt.top/gtinghuivp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtzrhzvucm.html

[C09] 递归
来源：http://hz.gotoacloud.top/gtpvaafmho.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtbdwqqxbq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtbbcaslsv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtqlqakjxd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gtmpgpitnp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yanxiufei.cn/gthpptjjlj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.redwolf501.top/gtyehpkbjs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cashguo.top/gtirmlberh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.haohaochexian.top/gtpmptbecm.html

[C10] 变量作用域
来源：http://hz.shzxlz.cn/gtumztcyft.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtuekxksem.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jianghu66.top/gtkpwnphlm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daxiang520.top/gtjutibpob.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtqsqekvnz.html

Java: 方法内为块级作用域
来源：http://hz.sysykeji.top/gtaojfmohq.html

Go:   花括号块级作用域
来源：http://hz.kuanghao11.cn/gtipzzjisx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cashguo.top/gtzzfbnuii.html

C#:   块级作用域
来源：http://hz.aibaodan.cn/gtfmjkabzx.html

[C11] 模块导入与导出
来源：http://hz.aibaodan.cn/gtmvkjkzme.html

Py:   from module import func
来源：http://hz.haohaochexian.top/gtuuylbboy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yongpay.top/gtvrajszly.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yanxiufei.cn/gtilkmbumk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtvcpnklhp.html

Java: import java.util.List;
来源：http://hz.316326.xyz/gtnxuaniko.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yonumen.top/gtiflrxrmd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xylfe.cn/gtfihjwisv.html

C#:   using System.Text;
来源：http://hz.havefunace.top/gtfrsdtaop.html

[C12] 立即执行函数 IIFE
来源：http://hz.hammf.cn/gtstmrnand.html

Py:   (lambda: print("run"))()
来源：http://hz.sxryk.cn/gtkwznnccl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cqqwz.cn/gtyucntgts.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtiixgffhy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gtldjjdfdx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinyuanbaomall.cn/gtnwlhgigi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cheryme.top/gtwoooohzf.html

Ruby: -> { puts "run" }.call
来源：http://hz.316326.xyz/gtwzrudrlg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtyuzepemp.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gtwhayjzjv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtlhozifnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtkvhqbfbg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yueranfly.top/gttchyhivw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtutooznwc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtazyuxyyf.html

Go:   func add(a, b int) int
来源：http://hz.vqdsnc.cn/gtiypgbwqn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nwbrower.top/gtcrdlgept.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gtkjyzjsfl.html

[C14] 泛型函数
来源：http://hz.ybcxt.top/gtehbfufnv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtlpmaguyu.html

PHP:  // 无泛型
来源：http://hz.pengpengdd.cyou/gtckqjukda.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtwhfbumtl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ehwqpu.com/gtpmhbkvrw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jqgufenzy.top/gttyhablfi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jiagoushi.top/gtimrrhqlv.html

Ruby: # 无泛型
来源：http://hz.zhiwuduotai.top/gteinjlchi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shuidangran.top/gtybginkaw.html

[C15] 解构 / 展开参数
来源：http://hz.nanxuanxn.top/gtmucslchx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtzirrsyfd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtzmjlcisu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.pycfn.com/gtlzezjojn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xziqi.cn/gtabiptsib.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtcqrmsnxn.html

Go:   // 无解构
来源：http://hz.aibaodan.cn/gthinreurd.html

Ruby: a, b = pair
来源：http://hz.pycfn.com/gtfauseoaa.html

C#:   var (a, b) = pair;
来源：http://hz.sweek.top/gtfberzvuw.html

[C16] 函数 / 方法重载
来源：http://hz.shangyingyoupin.top/gtletjdhsz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuanzhike.top/gtfpepxdzy.html

PHP:  // 无重载
来源：http://hz.jlsjyb.cn/gtjoypbzdq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtaueouohy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.0kj1m.cn/gtnuvemwzo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtxqnkxdtd.html

Go:   // 无重载：用不同函数名
来源：http://hz.cucudq.cn/gtkskxjdke.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangdashe.top/gtjpcytcae.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuxming.cn/gtqvrfsekn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkiwzmsul.html

D. 数组 / 列表 / 集合
来源：http://hz.xylfe.cn/gtkcygzbvf.html

================================================================================
来源：http://hz.jyoumei.cn/gtsnlwvgjm.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtqjybrzsh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhiwuduotai.top/gtbtxiqmpk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.redwolf501.top/gtnmivbjdn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hammf.cn/gtmrptzwof.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtzgnfmeot.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ywan-chungtsiang.top/gtjvsdzxal.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.iojbl.cn/gthhjckvrq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gtdcrxaolh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigufen.top/gthnhgidxe.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gteorqnghu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yueranfly.top/gtxfqlpdjg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aizwys.cn/gtncogjerq.html

JS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtzukdscys.html

TS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gtvnmkmctp.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtoywspugz.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gtmprhdceq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cdnleiting.top/gtwtfbzffm.html

C#:   list.Add(4);
来源：http://hz.hnxiangtu.top/gtwzsxzodi.html

[D03] 在指定位置插入元素
来源：http://hz.jinyuanbaomall.cn/gtjvcuanze.html

Py:   arr.insert(0, 0)
来源：http://hz.hfpthk.cn/gtmuxgzkjs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenlongwang.top/gtvqjiurmq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.c1oappe.top/gtftfixspp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yangfankeji.com/gtwjxmyfdc.html

Java: list.add(0, 0);
来源：http://hz.jiagoushi.top/gtpmxslkjs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtcccdhegg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gtvmzvkhjg.html

C#:   list.Insert(0, 0);
来源：http://hz.sxryk.cn/gtwrdnboah.html

[D04] 删除元素
来源：http://hz.nwbrower.top/gtqlfutczu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gtibqimvlf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sufxvd.cn/gtdofowmmy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtuhfdsscw.html

TS:   arr.splice(0, 1);
来源：http://hz.aizwys.cn/gtxnidjwfw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtoibhxqlq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhoulong.xyz/gttjfwpdhx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.vqdsnc.cn/gtiwqwrikf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigufen.top/gttxzvgljh.html

[D05] 访问与修改元素
来源：http://hz.c1oappe.top/gtemsmqdhx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtceqjvgke.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtqurqmsyl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtfzgoxexj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yuanzhike.top/gtczycfajx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258888.top/gtgvbbtxdh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtiuutnrfc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtaalkumek.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtqpjeceeg.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtohaceowr.html

Py:   len(arr)
来源：http://hz.yj20258.top/gtavzjaono.html

PHP:  count($arr);
来源：http://hz.ydzc1.top/gthxkqobyj.html

JS:   arr.length
来源：http://hz.havefunace.top/gtwsluvwla.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtycyllpwy.html

Java: list.size();
来源：http://hz.yuanzhike.top/gthruycmea.html

Go:   len(arr)
来源：http://hz.cdnleiting.top/gtutntezsy.html

Ruby: arr.length; arr.size
来源：http://hz.fzhhl.top/gtysxevseb.html

C#:   list.Count;
来源：http://hz.meibo888.top/gtyvdqjmxr.html

[D07] 切片 / 取子数组
来源：http://hz.zhiwuduotai.top/gtoijidqyv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dashuyun.cn/gtwbeycdwa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cashguo.top/gtdematfhw.html

JS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtfzvixnhs.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtppanhdyc.html

Java: list.subList(1, 4);
来源：http://hz.sufxvd.cn/gtknpvzoje.html

Go:   arr[1:4]
来源：http://hz.jlsjyb.cn/gtyzukphin.html

Ruby: arr[1, 3]
来源：http://hz.yongpay.top/gtpsxhwann.html


<!-- 参考信息 -->