代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gthryhqpkc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shanyushiyangkeji.top/gtdppuccks.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.feifeiyinyue.top/gtfbcpcbsb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtuhrlqvdz.html

[B09] break 与 continue
来源：http://hz.cashguo.top/gtijcivlxz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yangfankeji.com/gtbuehyrnv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sysykeji.top/gtfgwpfkdc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtjmcgfujj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtgtjoxtyd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtsgnkvfxw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.aibaodan.cn/gtpzdnuuzp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.havefunace.top/gtxxfkyydv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtjkpfrmkx.html

[B10] 遍历同时拿索引
来源：http://hz.zycfv.cn/gtoloepxfz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhiwuduotai.top/gtztfkuwvo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.quarkkingdee.top/gtsakksukr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtrawbakjn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangkeji.top/gtttporlqa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.nanxuanxn.top/gtvgdktbua.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gaohongyu789.top/gttoauatnz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gogol.net.cn/gtoziaewsr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cqqwz.cn/gtkbsbdpst.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtaeemcnih.html

Py:   list(range(0, 10, 2))
来源：http://hz.quarkkingdee.top/gtdzletnbw.html

PHP:  range(0, 10, 2);
来源：http://hz.hammf.cn/gtnppgechb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yongpay.top/gtfziafrzk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xziqi.cn/gtufdvquyo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.vqdsnc.cn/gtmurqodrp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cdnleiting.top/gtmwyajfiq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.9152youxi.cn/gttkkjvyxb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.iojbl.cn/gtmcelmpxm.html

[B12] 跳出多层循环
来源：http://hz.svipenyu.cn/gtmfdpgpog.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xziqi.cn/gtgucmrsen.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenlongwang.top/gtnuoogoaw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtmboanmjb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtiecldrqr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtbxliawff.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxuanxn.top/gtcborgwbx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gaohongyu789.top/gtlcrsijea.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.dashuyun.cn/gtebfebryg.html

[B13] 判断是否为数字
来源：http://hz.zhaomingkeji.xyz/gtjhgheiyl.html

Py:   isinstance(x, (int, float))
来源：http://hz.ivvv.top/gtspkcbbvf.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtfzvsfpsj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ppjwa.cn/gtokmpzoqb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangdashe.top/gtntbwlqfp.html

Java: x instanceof Number
来源：http://hz.ppjwa.cn/gtldkwfiah.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cucudq.cn/gtcoryvllf.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenzaomai.com/gthwdfmazt.html

C#:   x is int or double or decimal
来源：http://hz.chenlongwang.top/gthyjeajlg.html

[B14] 判断值是否在集合内
来源：http://hz.yvedp.cn/gtwhlvrhky.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.0kj1m.cn/gtsejeuqde.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gotoacloud.top/gtztwqfbos.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258888.top/gtkwiilxvq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtyelyqjuh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.andypj.xyz/gtatmjdlhu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gtnuaazuub.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.daria6918.cn/gtptctqyey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.0kj1m.cn/gtxdhjnzbp.html

[B15] 布尔运算与取反
来源：http://hz.meibo888.top/gtqbamloee.html

Py:   a and b or not c
来源：http://hz.jiagoushi.top/gttfudvyic.html

PHP:  $a && $b || !$c
来源：http://hz.bjfxy.top/gtxjfijurw.html

JS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtahulspsn.html

TS:   a && b || !c
来源：http://hz.sxryk.cn/gttjavokzj.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gtkdukygpy.html

Go:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtxkxqmqjq.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtfqgkmiem.html

C#:   a && b || !c
来源：http://hz.hammf.cn/gtnpaohnbu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.iojbl.cn/gtwhcojpra.html

Py:   if not data: return
来源：http://hz.andypj.xyz/gtmhwxbbwa.html

PHP:  if (!$data) { return; }
来源：http://hz.yuxming.cn/gtsuyirqee.html

JS:   if (!data) return;
来源：http://hz.iojbl.cn/gtbeqkqacs.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtrcdwshyb.html

Java: if (data == null) return;
来源：http://hz.ydzc1.top/gtfiiinvoc.html

Go:   if data == nil { return }
来源：http://hz.jinyuanbaomall.cn/gtvfjlemhs.html

Ruby: return if data.nil?
来源：http://hz.chenjidiqi.icu/gtlcquabyq.html

C#:   if (data == null) return;
来源：http://hz.cheryme.top/gtbkdkdkmb.html

================================================================================
来源：http://hz.ybcxt.top/gtymsakgeg.html

C. 函数与作用域
来源：http://hz.ydzc1.top/gtptxhpzvf.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtsxswtokj.html

[C01] 定义函数
来源：http://hz.gotoacloud.top/gtgeawauyl.html

Py:   def add(a, b): return a + b
来源：http://hz.cashguo.top/gtrqhdekah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtcfnueizy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gttkspcasg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtgedlvqxs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtytlejrpi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yongpay.top/gtvgehbtko.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtzmljgtvv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtkrlcbbbl.html

[C02] 默认参数
来源：http://hz.wangdashe.top/gtgposllux.html

Py:   def greet(name="World"): return name
来源：http://hz.yvedp.cn/gtffjhjnkt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hongshengwenyu.top/gtjcxhhdlq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cucudq.cn/gtqwkgbvvr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hammf.cn/gtxhmdkwkz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangkeji.top/gtvegltgyv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gogol.net.cn/gtgvkhuibz.html

Ruby: def greet(name = "World") = name
来源：http://hz.cucudq.cn/gtiudqlcop.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ehwqpu.com/gtkaupmeph.html

[C03] 可变参数
来源：http://hz.hnqzz.top/gtejiwgueb.html

Py:   def total(*args): return sum(args)
来源：http://hz.feifeiyinyue.top/gtxxymkvfu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.havefunace.top/gtwkedmfuj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtdudxklpo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtfaxtzacw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.birdmap.top/gtiusvgvul.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuanzx.com/gtgwbzfkog.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhoulong.xyz/gtkxfjndys.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenzaomai.com/gtajqfcrnm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.feifeiyinyue.top/gtuvpksmva.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pycfn.com/gtflkvfazl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cqqwz.cn/gtbkwuamvy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtfrumndcd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jyoumei.cn/gtbbywnitj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hysaishi.cn/gtpbzievuq.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinyuanbaomall.cn/gthjiktcpq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtklccrwts.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtwkanngeb.html

[C05] 返回多个值
来源：http://hz.sxryk.cn/gtedzzdovv.html

Py:   return a, b
来源：http://hz.dashuyun.cn/gthpsuqang.html

PHP:  return [$a, $b];
来源：http://hz.dashuyun.cn/gtufbbhhzf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gtkyfjlvnn.html

TS:   return { a, b };
来源：http://hz.feifeiyinyue.top/gtegdbosxv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xylfe.cn/gttxixcaou.html

Go:   return a, b
来源：http://hz.cdnleiting.top/gtczctbrea.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtyriiexni.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gttuzzjvwf.html

[C06] 匿名函数 / lambda
来源：http://hz.shzxlz.cn/gtxwnzpzqd.html

Py:   square = lambda x: x * x
来源：http://hz.cqqwz.cn/gtufupppvk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shzxlz.cn/gteypbhrlp.html

JS:   const square = x => x * x;
来源：http://hz.aibaodan.cn/gtfgqgzlpf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sysykeji.top/gtunixboek.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gtygdjyadv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gtlskedata.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shangyingyoupin.top/gtvcamsruq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sweek.top/gtxuvtoytc.html

[C07] 把函数作为参数传入
来源：http://hz.shzxlz.cn/gtahpvsjed.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yvedp.cn/gtqhotqfpy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yonumen.top/gtdiymrcjd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinqigufen.top/gtkjiumokh.html

TS:   arr.map(String)
来源：http://hz.ybcxt.top/gtysxdnoyl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hywenlv.cn/gtdhehitts.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.mhx1999.top/gtqrcmtyvh.html

Ruby: arr.map(&:upcase)
来源：http://hz.jyoumei.cn/gtrxirldxs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtinonzqss.html

[C08] 闭包
来源：http://hz.cqqwz.cn/gtqogmiqvo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cdnleiting.top/gtfulvmzhg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ivvv.top/gtpxzyfgzj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtzxyrzmtq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gttlbigaix.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.meibo888.top/gtlpjvwpbv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuanzx.com/gtvndorxje.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pengpengdd.cyou/gtpmbtlfth.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtzsvluloh.html

[C09] 递归
来源：http://hz.yueranfly.top/gtiwwehvbm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.meibo888.top/gtsqmifsrh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhiwuduotai.top/gtcneblmsd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtlljotpjl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gthiwqdwio.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuxming.cn/gtmehxkcat.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtgaiwsnmr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hnqzz.top/gtzlldjjmg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhijiandao.cn/gtbpatzacb.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gttmgmhjzb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgufenzy.top/gtmkuiofxo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.redwolf501.top/gtvuwnvoai.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tian-w.cn/gtudbizhah.html

TS:   同 JS
来源：http://hz.hfpthk.cn/gtyaijqcjh.html

Java: 方法内为块级作用域
来源：http://hz.xinyue.icu/gtpdwstzaa.html

Go:   花括号块级作用域
来源：http://hz.tian-w.cn/gtrjkrrbbz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guowangkeji.top/gtpnxxesja.html

C#:   块级作用域
来源：http://hz.yonumen.top/gtdjnahabw.html

[C11] 模块导入与导出
来源：http://hz.meibo888.top/gtoekfwlwi.html

Py:   from module import func
来源：http://hz.gotoacloud.top/gtmayxeetg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yvedp.cn/gtxrvmrxdf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sweek.top/gtlgumdvjr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xingfuxueyuan.xyz/gthtkhigly.html

Java: import java.util.List;
来源：http://hz.yj202588.top/gtkekffgns.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guannengcc.top/gtstkzcfzr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jyoumei.cn/gtfhnexqat.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtwudwggnz.html

[C12] 立即执行函数 IIFE
来源：http://hz.tanke756.top/gtjsmuhcjr.html

Py:   (lambda: print("run"))()
来源：http://hz.ybcxt.top/gtamsxbmlt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yvedp.cn/gtkuntpftf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hongshengwenyu.top/gtfjrgwkbb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gthfxwoglw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aibaodan.cn/gtmovhbsec.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pycfn.com/gtxkwltaug.html

Ruby: -> { puts "run" }.call
来源：http://hz.shzxlz.cn/gtlxlqauid.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guowangkeji.top/gthudqvqha.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhaomingkeji.xyz/gtovtwbvtr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtxtosaflf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtktyzqonm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hysaishi.cn/gtoqvacfqf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtruxomtlo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtyprvwrwz.html

Go:   func add(a, b int) int
来源：http://hz.zhixingplan.top/gtdrmawout.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cqqwz.cn/gtyhatqhae.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sxryk.cn/gtoftghhbv.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gtfenyzlig.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhengqikj.top/gtzqufxlqb.html

PHP:  // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtjnmbkrlk.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtcxwziamy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gtomlipsje.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gtwuvvplai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gotoacloud.top/gtvnjhlrax.html

Ruby: # 无泛型
来源：http://hz.ivvv.top/gttfbmspwh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ydzc1.top/gtkggaauqz.html

[C15] 解构 / 展开参数
来源：http://hz.zhixingplan.top/gtnzehuazm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxinkj.top/gtlmltjqot.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xingfuxueyuan.xyz/gtvntrhtze.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtluohtvoi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nwbrower.top/gtljexxfqh.html

Java: // 无解构
来源：http://hz.daria6918.cn/gtptpetfov.html

Go:   // 无解构
来源：http://hz.cheryme.top/gtmruakwch.html

Ruby: a, b = pair
来源：http://hz.svipenyu.cn/gtvifaauba.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtbcfdqjyn.html

[C16] 函数 / 方法重载
来源：http://hz.fzhhl.top/gtmxzkwkto.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dashuyun.cn/gtaqiaetej.html

PHP:  // 无重载
来源：http://hz.jlsjyb.cn/gttrkbvrgi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shuidangran.top/gtjrzmwclu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangdashe.top/gttakndtwt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuetiantiany.cn/gtbgsffuuo.html

Go:   // 无重载：用不同函数名
来源：http://hz.xinyue.icu/gtekrmupve.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtmqyihdmp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtfxrzzppt.html

================================================================================
来源：http://hz.cqqwz.cn/gtncgbodcm.html

D. 数组 / 列表 / 集合
来源：http://hz.sweek.top/gtbtxqxcpg.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbiqbchts.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtszapyxmq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtbdmspsya.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhixingplan.top/gtjuvauomw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258.top/gtxdupbmin.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhixingplan.top/gtiyihdjib.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dianchejie.cn/gtxptcfall.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtiikhoovm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hongshengwenyu.top/gttdbbszpx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sysykeji.top/gtujjyodin.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gtjqnmxhsq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtgmwegonz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtndoptnum.html

JS:   arr.push(4);
来源：http://hz.sweek.top/gtwijhhfmb.html

TS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtivypqvim.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtshirgnts.html

Go:   arr = append(arr, 4)
来源：http://hz.xingfuxueyuan.xyz/gtoiwvllzr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hysaishi.cn/gtbbnjhxef.html

C#:   list.Add(4);
来源：http://hz.ehwqpu.com/gthwfamkae.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtomqswidv.html

Py:   arr.insert(0, 0)
来源：http://hz.sufxvd.cn/gtypzlinfz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xinyue.icu/gtebvtbuty.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenzaomai.com/gtrwdnyxum.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jianghu66.top/gtaocobktd.html

Java: list.add(0, 0);
来源：http://hz.yuanzhike.top/gtwfdyrbtl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gtlvinofmn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigufen.top/gtlbgbzqaj.html

C#:   list.Insert(0, 0);
来源：http://hz.haohaochexian.top/gtpvwswfiz.html

[D04] 删除元素
来源：http://hz.pengpengdd.cyou/gtduguilgk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxuanxn.top/gtbcjchjkh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtloxdwrjo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xziqi.cn/gtzyuhxthx.html

TS:   arr.splice(0, 1);
来源：http://hz.52xcode.cn/gthfaujslb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.52xcode.cn/gtqnglfuse.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.andypj.xyz/gttuovvyyu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.smart0.xyz/gthtuxdiuy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shuidangran.top/gthytwqtee.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtnvatdvcv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtaaatsxzv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtjpzebziz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hywenlv.cn/gttkurnasp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hfpthk.cn/gtsawsyfxa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtqyvtmmxa.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nwbrower.top/gtqvzunmsn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gthqibljoe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sxryk.cn/gtsdbggoov.html

[D06] 数组长度
来源：http://hz.xylfe.cn/gtxophktyk.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtojdkrhal.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtcwywyqoy.html

JS:   arr.length
来源：http://hz.tanke756.top/gtszvfaeux.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gtekenyewt.html

Java: list.size();
来源：http://hz.guowangkeji.top/gtjktkpawl.html

Go:   len(arr)
来源：http://hz.wangdashe.top/gtvbunujnt.html

Ruby: arr.length; arr.size
来源：http://hz.hongshengwenyu.top/gtqpnieljn.html

C#:   list.Count;
来源：http://hz.chenlongwang.top/gtdfvrlgdz.html

[D07] 切片 / 取子数组
来源：http://hz.iojbl.cn/gtenkkwzyb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgufenzy.top/gthmoqnila.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydzc1.top/gtchyehbap.html

JS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtetokizqq.html

TS:   arr.slice(1, 4);
来源：http://hz.yuxming.cn/gtbujnowqw.html

Java: list.subList(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtadfyjadi.html

Go:   arr[1:4]
来源：http://hz.shzxlz.cn/gtvmijvckd.html

Ruby: arr[1, 3]
来源：http://hz.xingfuxueyuan.xyz/gtbdvsqmoq.html

C#:   list.GetRange(1, 3);
来源：http://hz.aibaodan.cn/gtfvuufxps.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtkldypdpb.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnxiangtu.top/gtgcospffw.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtdlvtyywa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigufen.top/gtwwrqyyvt.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gtppjnxoal.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xinyue.icu/gtbriuxgef.html

Go:   append(a, b...)
来源：http://hz.nanxuanxn.top/gtqotoxpro.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zdqjudy.top/gteievkcri.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtvvwnqpiw.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangkeji.top/gtoaqtharb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxinkj.top/gtgssdniso.html


<!-- 参考信息 -->