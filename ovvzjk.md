代发 wailian999

[B09] break 与 continue
来源：http://hz.zdqjudy.top/gtsajlvojg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.svipenyu.cn/gtamqpveyc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.316326.xyz/gtedepghrc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtutshstdg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtzqqialrw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtpjloneaq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigufen.top/gtfmgwurlv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cqqwz.cn/gtaxduztep.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtgnxphwag.html

[B10] 遍历同时拿索引
来源：http://hz.gotoacloud.top/gtfkevqkvj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shzxlz.cn/gtdbqjnkwh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yangfankeji.com/gtllgsqmfg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtnvlmsqpl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydzc1.top/gtgrtmvydh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shangyingyoupin.top/gtvrnpxfzj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.0kj1m.cn/gtbohrjuwo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinqigufen.top/gtcyxaduen.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hammf.cn/gtpmzitctt.html

[B11] 生成数字序列 / 区间
来源：http://hz.fengsongda.top/gtzzewpmmc.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtibiidtdr.html

PHP:  range(0, 10, 2);
来源：http://hz.havefunace.top/gtmtspyelg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gtvbfaveau.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtkqcvgzex.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ydjk.org.cn/gtotogarsa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.dashuyun.cn/gtoryoredu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ywan-chungtsiang.top/gttdegjgje.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgfzy.top/gtzezhkafe.html

[B12] 跳出多层循环
来源：http://hz.yangfankeji.com/gtcquwvvit.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgfzy.top/gteobwydea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cucudq.cn/gtolcccbvb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtvlxwzpww.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtwuqinflc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtnpqkozdi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinqigfzy.top/gtzahypsta.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtqrqnccbk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhongyouzk.top/gtgehmpuai.html

[B13] 判断是否为数字
来源：http://hz.gogol.net.cn/gtxkbvdtmj.html

Py:   isinstance(x, (int, float))
来源：http://hz.kuanghao11.cn/gtbhehngho.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtdhcohbal.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtdjpbndvq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtwfzsynks.html

Java: x instanceof Number
来源：http://hz.vqdsnc.cn/gtaqaalrpr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhijiandao.cn/gtrwchddad.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuanzx.com/gtxnjzreit.html

C#:   x is int or double or decimal
来源：http://hz.yangfankeji.com/gtymsknlvw.html

[B14] 判断值是否在集合内
来源：http://hz.birdmap.top/gtivinoreb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.guowangkeji.top/gtsfbldykh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydzc1.top/gtfpgnkpme.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258888.top/gtsaihzsfe.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtnatxrgrv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zycfv.cn/gthfrgjgsv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ivvv.top/gtqlowhuwr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.meibo888.top/gtiuyccysq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gtepitukue.html

[B15] 布尔运算与取反
来源：http://hz.aibaodan.cn/gtgmoyhtuf.html

Py:   a and b or not c
来源：http://hz.yvedp.cn/gtzqlemihu.html

PHP:  $a && $b || !$c
来源：http://hz.vqdsnc.cn/gtaseijbvl.html

JS:   a && b || !c
来源：http://hz.hywenlv.cn/gtcjjwcjst.html

TS:   a && b || !c
来源：http://hz.yongpay.top/gtpjuxksar.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gtcfjlsngy.html

Go:   a && b || !c
来源：http://hz.zycfv.cn/gtupngxsnc.html

Ruby: a && b || !c
来源：http://hz.dashuyun.cn/gtvbzvssrv.html

C#:   a && b || !c
来源：http://hz.haohaochexian.top/gtwivaawqx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guannengcc.top/gtrluwawdc.html

Py:   if not data: return
来源：http://hz.birdmap.top/gtswyifnsh.html

PHP:  if (!$data) { return; }
来源：http://hz.xylfe.cn/gtzqwdnvfp.html

JS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtjhtjhbuo.html

TS:   if (!data) return;
来源：http://hz.tanke756.top/gtgeyjhtqm.html

Java: if (data == null) return;
来源：http://hz.hfpthk.cn/gtxoaovpwv.html

Go:   if data == nil { return }
来源：http://hz.jinqigufen.top/gtgubyktje.html

Ruby: return if data.nil?
来源：http://hz.mhx1999.top/gtigfezemb.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtusyfgpwo.html

================================================================================
来源：http://hz.zhongyouzk.top/gtesfojgvw.html

C. 函数与作用域
来源：http://hz.quarkkingdee.top/gtkpurnvhf.html

================================================================================
来源：http://hz.xziqi.cn/gtvxzjfmuq.html

[C01] 定义函数
来源：http://hz.wangshuangyany.cn/gtwyionokz.html

Py:   def add(a, b): return a + b
来源：http://hz.jinghuilouyu.cn/gtobizawtl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtusbzkipf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuanzx.com/gtgyhjnfwr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.haohaochexian.top/gtejrcvauv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtzypftykj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.andypj.xyz/gtymazhsal.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhiwuduotai.top/gtzhpmymnn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtgqtgaovj.html

[C02] 默认参数
来源：http://hz.jqgfzy.top/gtemqlkezj.html

Py:   def greet(name="World"): return name
来源：http://hz.hfpthk.cn/gtlgrrokuk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtjcscxspk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yonumen.top/gtgjxfvhay.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtjdthgycu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yongpay.top/gtupntplre.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zdqjudy.top/gtdeqcolom.html

Ruby: def greet(name = "World") = name
来源：http://hz.iojbl.cn/gtwprczfmo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aibaodan.cn/gtcnwkamfv.html

[C03] 可变参数
来源：http://hz.xingfuxueyuan.xyz/gtwplrslde.html

Py:   def total(*args): return sum(args)
来源：http://hz.xingfuxueyuan.xyz/gtzzcqfloj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shuidangran.top/gtpktlpgap.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gtxbqegsmi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hywenlv.cn/gtmpyidxaw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nwbrower.top/gtmvkqgoei.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtztbxjdtp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jlsjyb.cn/gtzvhdrkif.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hysaishi.cn/gtxzeyqode.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pycfn.com/gtqqgnamux.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhixingplan.top/gtezbmiksj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zdqjudy.top/gtmmcnzljs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gtrlxjwkpk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtyocqpomb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shuidangran.top/gtdqhewcxq.html

Go:   // 无：用配置结构体参数
来源：http://hz.cashguo.top/gtzsxfcirg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gtvwsxsbrq.html

C#:   f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtyayfblzg.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gthaqaugyg.html

Py:   return a, b
来源：http://hz.snrcjt.cn/gturdeyqdf.html

PHP:  return [$a, $b];
来源：http://hz.chenlongwang.top/gtsnoevcbl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.dashuyun.cn/gtnmkibdlb.html

TS:   return { a, b };
来源：http://hz.wangdashe.top/gtqgirrrqn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.snrcjt.cn/gtjeohtjdn.html

Go:   return a, b
来源：http://hz.yj20258.top/gtvqkxkzbl.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtusfuhzdw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yonumen.top/gtrvjtajom.html

[C06] 匿名函数 / lambda
来源：http://hz.iojbl.cn/gtidldselm.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtudkhnfsz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.aizwys.cn/gtoomqynln.html

JS:   const square = x => x * x;
来源：http://hz.zhiwuduotai.top/gtdtglzvkw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuetiantiany.cn/gtmutxvszd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daxiang520.top/gtenwbiplz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgufenzy.top/gtkwfchgcx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yuxming.cn/gtkzodxinn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xziqi.cn/gtannomwqg.html

[C07] 把函数作为参数传入
来源：http://hz.yanxiufei.cn/gthratoswq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xylfe.cn/gtnidpwwxy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxuanxn.top/gttteniqsg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtgtdgxewc.html

TS:   arr.map(String)
来源：http://hz.52xcode.cn/gtxycbxykz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hysaishi.cn/gtivdcqvht.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hammf.cn/gtofdtvvji.html

Ruby: arr.map(&:upcase)
来源：http://hz.xziqi.cn/gtrdrcqmnm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ppjwa.cn/gtnhrzercj.html

[C08] 闭包
来源：http://hz.zhaomingkeji.xyz/gtsgvuouif.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gtdamxdmpf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.andypj.xyz/gtxhthryex.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtaqqqpvqq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gthvhwrplj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtrvedgpaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sweek.top/gtagtbkzsa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.vqdsnc.cn/gtlazfxhch.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtvrsbbfhk.html

[C09] 递归
来源：http://hz.shuidangran.top/gtsuaijlzu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtoajltqkk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xuetiantiany.cn/gtlnjlqsxx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtmbamqtqx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtyrlioiiz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.c1oappe.top/gtmblenaeo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jlsjyb.cn/gtagxuraqy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tian-w.cn/gtypecunpu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gtbyqirubf.html

[C10] 变量作用域
来源：http://hz.kuanghao11.cn/gtpmdzpfcq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258.top/gtgrfpglhb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.iojbl.cn/gtqcchlspd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258.top/gtllngvkbu.html

TS:   同 JS
来源：http://hz.cqqwz.cn/gtmkobazif.html

Java: 方法内为块级作用域
来源：http://hz.jqgufenzy.top/gtlvjfjsmq.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtnuelndwj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hfpthk.cn/gtngynlpeq.html

C#:   块级作用域
来源：http://hz.guowangkeji.top/gthazcpqaw.html

[C11] 模块导入与导出
来源：http://hz.jqgfzy.top/gtmhbchpka.html

Py:   from module import func
来源：http://hz.tanke756.top/gtzwvlruce.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtjrkoxclf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuetiantiany.cn/gtyfupkhmv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shuidangran.top/gtacevtzsr.html

Java: import java.util.List;
来源：http://hz.shanyushiyangkeji.top/gthpgqidbp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gttosxrvlr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.c1oappe.top/gturilihnb.html

C#:   using System.Text;
来源：http://hz.hongshengwenyu.top/gttpvuhuly.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gttxcwyyju.html

Py:   (lambda: print("run"))()
来源：http://hz.ydzc1.top/gtumgnqxfj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pengpengdd.cyou/gtydjsmxwj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gttwgouyxh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.haohaochexian.top/gtvjqsveit.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cucudq.cn/gthigoatzo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tanke756.top/gtjyukbldy.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnqzz.top/gtkatwwoql.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ybcxt.top/gtqtaffudk.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhixingplan.top/gtqstcaesa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.52xcode.cn/gtcqfoomqp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aizwys.cn/gtbtxlelbg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.haohaochexian.top/gtjamzcqqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtyrtyront.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtruplikiv.html

Go:   func add(a, b int) int
来源：http://hz.zdqjudy.top/gtuegyqowd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guannengcc.top/gtutkzifhj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.meibo888.top/gtaqoonumm.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gttjnfcwgf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tanke756.top/gtghyggyes.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtmizvzpkm.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtozovpbbs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtvubcodia.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guannengcc.top/gtooggetal.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zdqjudy.top/gtdplyxbbw.html

Ruby: # 无泛型
来源：http://hz.ppjwa.cn/gtryjsiumh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenzaomai.com/gtwelglojk.html

[C15] 解构 / 展开参数
来源：http://hz.jiagoushi.top/gtnxrvycod.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.svipenyu.cn/gtppspxuxo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.iojbl.cn/gtiwfcykng.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gttiqpfgyu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ehwqpu.com/gtgkgbicqs.html

Java: // 无解构
来源：http://hz.ppjwa.cn/gtxktgbagj.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gteyutmwos.html

Ruby: a, b = pair
来源：http://hz.bjfxy.top/gtqmzphbre.html

C#:   var (a, b) = pair;
来源：http://hz.xziqi.cn/gtwipncwwm.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtadvvoxdw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgufenzy.top/gtrzywwjej.html

PHP:  // 无重载
来源：http://hz.chenjidiqi.icu/gtslwpecxz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yueranfly.top/gticnqhazj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ywan-chungtsiang.top/gtuqqpkjnj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinqigfzy.top/gtphhehwgk.html

Go:   // 无重载：用不同函数名
来源：http://hz.guannengcc.top/gtyldmkohq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj202588.top/gtnxsnfasp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.iojbl.cn/gtcztrqimp.html

================================================================================
来源：http://hz.yongpay.top/gtuhhfafxg.html

D. 数组 / 列表 / 集合
来源：http://hz.ydzc1.top/gtqffablcx.html

================================================================================
来源：http://hz.hammf.cn/gtrdkewdql.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gttjwyfsch.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhongyouzk.top/gtidnuwuuq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jlsjyb.cn/gtirtmtxhq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jiagoushi.top/gtjwodkoso.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gthtwagkgq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhijiandao.cn/gtgzwxsupb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.vqdsnc.cn/gtksbunppw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sweek.top/gtqbnubuxt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hfpthk.cn/gtecrsbkls.html

[D02] 追加元素到末尾
来源：http://hz.chenzaomai.com/gtqfkvrdvl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtebrctzvt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gtkgtktrkl.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtqrevnolq.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtfdlpowgx.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtukghetam.html

Go:   arr = append(arr, 4)
来源：http://hz.xuetiantiany.cn/gtxiivxcbv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenlongwang.top/gtiadmprwk.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtwxczvzrm.html

[D03] 在指定位置插入元素
来源：http://hz.fzhhl.top/gtsejjeqbx.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtkjfrcqnm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shangyingyoupin.top/gtctghlxto.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gzhubu.top/gteyaqdtxh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgfzy.top/gtfscfzlbq.html

Java: list.add(0, 0);
来源：http://hz.wangshuangyany.cn/gtgllbngtz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.kuanghao11.cn/gtlomysftz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nanxinkj.top/gtmngfdgpc.html

C#:   list.Insert(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtzbnkoshl.html

[D04] 删除元素
来源：http://hz.ehwqpu.com/gtxfekilvv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.feifeiyinyue.top/gtngiqapzk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtwgqoaxvx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gtcbiitqeu.html

TS:   arr.splice(0, 1);
来源：http://hz.9152youxi.cn/gtrqnohwrr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuxming.cn/gtulcihavv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hysaishi.cn/gtehyzwkjm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dashuyun.cn/gtajbvbaqi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.52xcode.cn/gtbejtcddk.html

[D05] 访问与修改元素
来源：http://hz.hysaishi.cn/gtmvuoeonl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtxvzjbmsk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtqjnsvgsf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.316326.xyz/gtgaxdkrad.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtdzdltrsf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.52xcode.cn/gtclrtqzxv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtorvugdct.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gthtogppod.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fzhhl.top/gtblxxdfbp.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtnqedloih.html

Py:   len(arr)
来源：http://hz.c1oappe.top/gtonmdvzsg.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gttallnpdn.html

JS:   arr.length
来源：http://hz.ydzc1.top/gtwcbdolvk.html

TS:   arr.length
来源：http://hz.shanyushiyangtech.top/gteytzedjl.html

Java: list.size();
来源：http://hz.hnxiangtu.top/gtngjhmohk.html

Go:   len(arr)
来源：http://hz.vqdsnc.cn/gttdamrrtj.html

Ruby: arr.length; arr.size
来源：http://hz.zhiwuduotai.top/gtkvihewwb.html

C#:   list.Count;
来源：http://hz.daxiang520.top/gtsjoxnzei.html

[D07] 切片 / 取子数组
来源：http://hz.zhixingplan.top/gtryjdxhmz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtmkvsptzz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxuanxn.top/gtcuqppbge.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gthfvtfhjn.html

TS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gttiuundke.html

Java: list.subList(1, 4);
来源：http://hz.cqqwz.cn/gtoqpwvniy.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtojutivhs.html

Ruby: arr[1, 3]
来源：http://hz.zhaomingkeji.xyz/gtqihamzyg.html

C#:   list.GetRange(1, 3);
来源：http://hz.haohaochexian.top/gtsaqfbzyu.html

[D08] 合并两个数组
来源：http://hz.hfpthk.cn/gthbybrtcu.html

Py:   a + b;  a.extend(b)
来源：http://hz.jyoumei.cn/gthpzfzbdz.html

PHP:  array_merge($a, $b);
来源：http://hz.kuanghao11.cn/gthjymmjdn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tianlin.xyz/gtgxnjnwrc.html

TS:   [...a, ...b];
来源：http://hz.sxryk.cn/gtkqqgguli.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtjhnnzopp.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gtnmqkymjv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258888.top/gtkkjacfgf.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gturnifwbc.html

[D09] 排序（升序）
来源：http://hz.yongpay.top/gtvaktfpap.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtnjnjdejs.html

PHP:  sort($arr);
来源：http://hz.xuanzx.com/gtzgkclgih.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guannengcc.top/gtqrzrmgah.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258888.top/gtokceeicv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tanke756.top/gtbwdkkxbr.html


<!-- 参考信息 -->