代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxuanxn.top/gtjkksbaam.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.316326.xyz/gtabmlkujr.html

JS:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtooujhyug.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtzezmptkp.html

Java: do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtafheuyie.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ydjk.org.cn/gtuzeqwomk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gzhubu.top/gtlvvxrcma.html

C#:   do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtnvymaqzo.html

[B09] break 与 continue
来源：http://hz.sweek.top/gtrnpnwiuu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cheryme.top/gtpviptwos.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cashguo.top/gtsgjvrhbx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gthibljvij.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtbqacznsp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtjqleugmx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cucudq.cn/gtyjcatrlw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhengqikj.top/gtlzeoedur.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtdejswlvz.html

[B10] 遍历同时拿索引
来源：http://hz.zhiwuduotai.top/gtocmpevit.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.smart0.xyz/gtcsjlslqm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.dashuyun.cn/gtpezdowwq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daxiang520.top/gtmeryamre.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hammf.cn/gtfhvbzpof.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ydzc1.top/gtvzekmcth.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gotoacloud.top/gtriwtdznt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tianlin.xyz/gtuurjiyno.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fzhhl.top/gtzzigarta.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenjidiqi.icu/gtwtvkeizo.html

Py:   list(range(0, 10, 2))
来源：http://hz.ivvv.top/gtnkdbnbsd.html

PHP:  range(0, 10, 2);
来源：http://hz.hongshengwenyu.top/gttjqvnykf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangtech.top/gtkpetyvnh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxinkj.top/gtclhulfiz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenzaomai.com/gtsqunnjxv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sufxvd.cn/gtpawubfkj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.bjfxy.top/gtoeteeqys.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sxryk.cn/gttlydydhb.html

[B12] 跳出多层循环
来源：http://hz.quarkkingdee.top/gtpqiwxyzx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cucudq.cn/gtnhzjwmvq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.meibo888.top/gthehrrrcu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtlxwcmnty.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtjjgfrghu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtnxxfkxvh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.haohaochexian.top/gtkixeqyob.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gzhubu.top/gtvdhzzdby.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinqigfzy.top/gtjtwqkmpa.html

[B13] 判断是否为数字
来源：http://hz.jinyuanbaomall.cn/gtutnmacay.html

Py:   isinstance(x, (int, float))
来源：http://hz.sxryk.cn/gtxsgwtyww.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtmrashsey.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtcgcmthoq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tianlin.xyz/gtvvivdrtg.html

Java: x instanceof Number
来源：http://hz.redwolf501.top/gtaafbhihz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.meibo888.top/gtqsogkgxx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuanzhike.top/gtqlyssdvw.html

C#:   x is int or double or decimal
来源：http://hz.mhx1999.top/gtktkpellq.html

[B14] 判断值是否在集合内
来源：http://hz.zdqjudy.top/gtqdtxrzgj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jiagoushi.top/gtwllnpqgj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.redwolf501.top/gtidwwznwv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gtbwarehnl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gtpxtmeevq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cashguo.top/gtqmoqizju.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ywan-chungtsiang.top/gtbjkbkvlt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangkeji.top/gtmcbkxsss.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aibaodan.cn/gtodayxdua.html

[B15] 布尔运算与取反
来源：http://hz.yj20258.top/gtixllyafv.html

Py:   a and b or not c
来源：http://hz.jinqigfzy.top/gtftaazxto.html

PHP:  $a && $b || !$c
来源：http://hz.feifeiyinyue.top/gtbrurxqnh.html

JS:   a && b || !c
来源：http://hz.ppjwa.cn/gtoqewuopd.html

TS:   a && b || !c
来源：http://hz.bjfxy.top/gtjtipkuih.html

Java: a && b || !c
来源：http://hz.zhixingplan.top/gtsspwpaoj.html

Go:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtmuvglxxv.html

Ruby: a && b || !c
来源：http://hz.daria6918.cn/gtnzuaslat.html

C#:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtlpciudjm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtamctticf.html

Py:   if not data: return
来源：http://hz.yj20258888.top/gtqvnwxsxq.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gtdzgieobs.html

JS:   if (!data) return;
来源：http://hz.316326.xyz/gtdfubewkp.html

TS:   if (!data) return;
来源：http://hz.fzhhl.top/gtifpyxbya.html

Java: if (data == null) return;
来源：http://hz.tianlin.xyz/gtsladcmlp.html

Go:   if data == nil { return }
来源：http://hz.ywan-chungtsiang.top/gtznuijdox.html

Ruby: return if data.nil?
来源：http://hz.jlsjyb.cn/gtqrdyxzbe.html

C#:   if (data == null) return;
来源：http://hz.yj20258888.top/gtxdqpmuph.html

================================================================================
来源：http://hz.andypj.xyz/gtmvuytnac.html

C. 函数与作用域
来源：http://hz.xingfuxueyuan.xyz/gtxhurfjaz.html

================================================================================
来源：http://hz.sysykeji.top/gtqxgpmtfs.html

[C01] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtykbyurvq.html

Py:   def add(a, b): return a + b
来源：http://hz.sufxvd.cn/gtlgjwbszy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtkpsnstpj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtwdphlxyg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gticqznwxi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtrbaaecvy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhaomingkeji.xyz/gtmbfmhlsg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.mhx1999.top/gtinyyikkl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtxghwvlli.html

[C02] 默认参数
来源：http://hz.daxiang520.top/gtjeslfzzn.html

Py:   def greet(name="World"): return name
来源：http://hz.andypj.xyz/gtpdkpvlmg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cucudq.cn/gtyonhqovr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.birdmap.top/gtfitgdihj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.havefunace.top/gtargwacyw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhengqikj.top/gtfwrfdskw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangtech.top/gtflnmhtrf.html

Ruby: def greet(name = "World") = name
来源：http://hz.meibo888.top/gtnfvihevl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nwbrower.top/gtulgdhqsp.html

[C03] 可变参数
来源：http://hz.shanyushiyangkeji.top/gtkpzlelmu.html

Py:   def total(*args): return sum(args)
来源：http://hz.tianlin.xyz/gtqddvvvor.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cheryme.top/gtejcozedv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtuzwxtewg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shangyingyoupin.top/gtmcdebdgg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yuxming.cn/gtqsnvrnpm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhiwuduotai.top/gtxecvcdnk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258.top/gtiwrwvwfn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.c1oappe.top/gtpqxiadqz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.havefunace.top/gtewndhubx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shuidangran.top/gtsfufwifo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.52xcode.cn/gtvrpydbxq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtlvhslmlx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenlongwang.top/gtbnewsege.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daxiang520.top/gtpbmoaytr.html

Go:   // 无：用配置结构体参数
来源：http://hz.fengsongda.top/gtrwhiucnl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtqonubdni.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gthryffrju.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtsoucucmf.html

Py:   return a, b
来源：http://hz.bjfxy.top/gtxvojnwbv.html

PHP:  return [$a, $b];
来源：http://hz.snrcjt.cn/gtbqmlbccq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydjk.org.cn/gtvwiilsno.html

TS:   return { a, b };
来源：http://hz.chenjidiqi.icu/gtfkfqqkgc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.c1oappe.top/gtwiwrsoxy.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtjaqbctcp.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtwvaxpjxk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nwbrower.top/gtefjuhcjl.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gtaxpmikyc.html

Py:   square = lambda x: x * x
来源：http://hz.sweek.top/gtpfkzjttj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtwowiunov.html

JS:   const square = x => x * x;
来源：http://hz.wangdashe.top/gtwgpsfakm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.feifeiyinyue.top/gthtltzuqs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtfaizpjdk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.andypj.xyz/gthfwzxwyl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shuidangran.top/gtyrgnknjd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sweek.top/gtqemzdkda.html

[C07] 把函数作为参数传入
来源：http://hz.hnxiangtu.top/gtejqjvbaa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yangfankeji.com/gtnqnghtor.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.havefunace.top/gtmqpserbb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.mhx1999.top/gtrxzektpi.html

TS:   arr.map(String)
来源：http://hz.yongpay.top/gtefksugpc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuanzhike.top/gtxzercbrj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sxryk.cn/gtwjrnwpix.html

Ruby: arr.map(&:upcase)
来源：http://hz.xingfuxueyuan.xyz/gtfuvbpiug.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ehwqpu.com/gtlfhtrpcu.html

[C08] 闭包
来源：http://hz.yj202588.top/gtbvqmyolc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhoulong.xyz/gtuagysdov.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnqzz.top/gtagcygyae.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtuuswliiz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtkvdnmgdx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhongyouzk.top/gtiadsbfxv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.9152youxi.cn/gthkneyyhe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ivvv.top/gtomznbtsf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtdmycgroj.html

[C09] 递归
来源：http://hz.jinyuanbaomall.cn/gtkdmgvdkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gttnwrrfgu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gttmlptiqf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgufenzy.top/gtluiosfcp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtvxecpwdp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shanyushiyangkeji.top/gtvklvvswe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gogol.net.cn/gtcaccxpix.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtsmonvqbb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gtrofarbtc.html

[C10] 变量作用域
来源：http://hz.xylfe.cn/gtvkjvjzgq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cheryme.top/gtuwtisjlg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.smart0.xyz/gtlxgbzxrt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cheryme.top/gtyfgxfmcq.html

TS:   同 JS
来源：http://hz.quarkkingdee.top/gtcvgfkyht.html

Java: 方法内为块级作用域
来源：http://hz.gotoacloud.top/gtlhyqrktl.html

Go:   花括号块级作用域
来源：http://hz.yj202588.top/gtcdwkhdme.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.haohaochexian.top/gtgenoufwi.html

C#:   块级作用域
来源：http://hz.jyoumei.cn/gtfywbdtxv.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gtejtvtzmy.html

Py:   from module import func
来源：http://hz.jianghu66.top/gtnargsmwp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dianchejie.cn/gtipdxnczf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.andypj.xyz/gtwsrersqx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sxryk.cn/gtxkvfjxlo.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtavobycrr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aibaodan.cn/gtnqtalrky.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtbojcrrib.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gttzpuoutk.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gtnzvercfu.html

Py:   (lambda: print("run"))()
来源：http://hz.zhoulong.xyz/gtlhoujims.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ppjwa.cn/gtqnucllht.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtimkwzhrw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtnrpiywuh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtqkvdybzo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aizwys.cn/gtwshbovlq.html

Ruby: -> { puts "run" }.call
来源：http://hz.0kj1m.cn/gtcipedcqt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fzhhl.top/gtvorzhjby.html

[C13] 类型声明 / 类型注解
来源：http://hz.xylfe.cn/gtagxafgtn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.mhx1999.top/gtuowbfygg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtqqalvuaf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtmxcoxmxf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtglvjhrsa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gttbximprr.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtxzmhmkvb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sufxvd.cn/gtvtdqmytn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinyuanbaomall.cn/gtaecxeibt.html

[C14] 泛型函数
来源：http://hz.svipenyu.cn/gtqtkujefk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenjidiqi.icu/gtntceabok.html

PHP:  // 无泛型
来源：http://hz.yanxiufei.cn/gtssdtgkit.html

JS:   // 无泛型
来源：http://hz.pycfn.com/gtrenyrnjw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtjhzcbhym.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nanxinkj.top/gtvbtgcwvb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ybcxt.top/gtxlnuqgqx.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gttcrjypbu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhixingplan.top/gtgenhjsem.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gttcxlorie.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtnsdkwvdb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.havefunace.top/gtunuecjqu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtftuwdfsy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.birdmap.top/gtikoqeavt.html

Java: // 无解构
来源：http://hz.daxiang520.top/gtbiwdkzmk.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtyajqirjx.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtqmiutoeg.html

C#:   var (a, b) = pair;
来源：http://hz.tanke756.top/gtfaprmwuh.html

[C16] 函数 / 方法重载
来源：http://hz.yonumen.top/gtbtneikhg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhengqikj.top/gtlctdztdq.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtprxynfez.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangtech.top/gtqaabzlaw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dianchejie.cn/gtcztjatzc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hysaishi.cn/gtyemilsup.html

Go:   // 无重载：用不同函数名
来源：http://hz.vqdsnc.cn/gtrqombqcb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhaomingkeji.xyz/gtsebehvyl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnxiangtu.top/gtlmlismvt.html

================================================================================
来源：http://hz.wangdashe.top/gthvcjscyc.html

D. 数组 / 列表 / 集合
来源：http://hz.sxryk.cn/gtkpibkwpc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwefoyhox.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtmooolpom.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenjidiqi.icu/gtczmegkam.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.wangdashe.top/gtgpwupwrq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnqzz.top/gtqazqmpeg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtcigkqome.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtiajwvtup.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hywenlv.cn/gthcpladvy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtowlcxajo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhongyouzk.top/gtrvfklgwb.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gttdclpnzm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtcshsofca.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gtlfsffyma.html

JS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtstedcllr.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtunqamkol.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtoplxlwqd.html

Go:   arr = append(arr, 4)
来源：http://hz.fengsongda.top/gtmgyqfpnd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dianchejie.cn/gthogiuuvs.html

C#:   list.Add(4);
来源：http://hz.nanxinkj.top/gtuupvwuqk.html

[D03] 在指定位置插入元素
来源：http://hz.gaohongyu789.top/gtyzecqmus.html

Py:   arr.insert(0, 0)
来源：http://hz.xuanzx.com/gtucipoqnl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtyisjjotc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shangyingyoupin.top/gtdmwxvvgx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtnsafucvf.html

Java: list.add(0, 0);
来源：http://hz.wangshuangyany.cn/gtroznjckw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenzaomai.com/gtcwgfxlmg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.0kj1m.cn/gttiikzjim.html

C#:   list.Insert(0, 0);
来源：http://hz.shuidangran.top/gtmntcukxp.html

[D04] 删除元素
来源：http://hz.birdmap.top/gtmrdxnofs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtddtdllzf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gzhubu.top/gtlnesvwlk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtegixybkg.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtherfkbgb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.andypj.xyz/gtlnfmzkgz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guowangkeji.top/gtfksgttgp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtvkzuhldy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yongpay.top/gtrkuddjkh.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangtech.top/gtdwfgsyrm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gteljsgoqv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtluysjajs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtaombbtho.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tian-w.cn/gtlycbfwux.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtsrbrchtk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtytrenloq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtpfqizgue.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gtnxodsefl.html

[D06] 数组长度
来源：http://hz.jinqigfzy.top/gtcctrhqzx.html

Py:   len(arr)
来源：http://hz.pengpengdd.cyou/gtakblghha.html

PHP:  count($arr);
来源：http://hz.cucudq.cn/gtszqiddlg.html

JS:   arr.length
来源：http://hz.jianghu66.top/gthixifjrq.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtgyiorlfp.html

Java: list.size();
来源：http://hz.guannengcc.top/gtawsjxosu.html

Go:   len(arr)
来源：http://hz.sxryk.cn/gtroiflube.html

Ruby: arr.length; arr.size
来源：http://hz.tanke756.top/gtpbudrnde.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtgjpzqaoq.html

[D07] 切片 / 取子数组
来源：http://hz.ywan-chungtsiang.top/gtkpldxuqc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fzhhl.top/gtvaabmgot.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ppjwa.cn/gtontgnnyt.html

JS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtkvtcafnn.html

TS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gttmcvkfum.html

Java: list.subList(1, 4);
来源：http://hz.nanxinkj.top/gtzsrjjumx.html

Go:   arr[1:4]
来源：http://hz.0kj1m.cn/gtshlxlhoa.html

Ruby: arr[1, 3]
来源：http://hz.hammf.cn/gtimtwrdpe.html

C#:   list.GetRange(1, 3);
来源：http://hz.gzhubu.top/gthqnvfdke.html

[D08] 合并两个数组
来源：http://hz.zhengqikj.top/gtiajketii.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gtupekeseg.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtqeoogyjg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangtech.top/gtfcuxebgy.html

TS:   [...a, ...b];
来源：http://hz.iojbl.cn/gthlujjrln.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhongyouzk.top/gtxonqzinc.html

Go:   append(a, b...)
来源：http://hz.hnqzz.top/gtrwbbtnps.html


<!-- 参考信息 -->