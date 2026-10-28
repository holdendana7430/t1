代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.birdmap.top/gtfvuhmvmu.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258888.top/gtnnbocxvm.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gttriceadp.html

[B08] do-while（至少执行一次）
来源：http://hz.yuxming.cn/gtobtgdqaw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxuanxn.top/gtoprqelhc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhijiandao.cn/gtithobdsm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gtoagylreh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.pengpengdd.cyou/gtvavghqck.html

Java: do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtkcfqtjin.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jianghu66.top/gtqwwvaaff.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gogol.net.cn/gtpohcvpnh.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gteasujnym.html

[B09] break 与 continue
来源：http://hz.guannengcc.top/gtasrzxxek.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ywan-chungtsiang.top/gtzplyxldp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ydjk.org.cn/gtqmuaejgq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtvgujskuc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtgllyimfz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtfohfnivd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.kuanghao11.cn/gtmeiplksq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jiagoushi.top/gtcocjeuqv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtkrwdejkm.html

[B10] 遍历同时拿索引
来源：http://hz.shuidangran.top/gtqkjlmlqm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hysaishi.cn/gtrqpewgdj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gotoacloud.top/gtzocqcyla.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinyuanbaomall.cn/gtwfhtkjiz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.fzhhl.top/gtivthefuu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.daria6918.cn/gtctsjkngd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangshuangyany.cn/gtarfzqpcr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.haohaochexian.top/gtxabxuvdz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.guannengcc.top/gtvcbeqhcm.html

[B11] 生成数字序列 / 区间
来源：http://hz.shangyingyoupin.top/gtnrjpsitb.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258888.top/gtkvqmlarc.html

PHP:  range(0, 10, 2);
来源：http://hz.gzhubu.top/gttfaffqkk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtpksdykqo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtmgtsorfn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gogol.net.cn/gtbucqdlsg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.havefunace.top/gtyjednaog.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhijiandao.cn/gtihyqrxum.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gogol.net.cn/gthfefmmnm.html

[B12] 跳出多层循环
来源：http://hz.cashguo.top/gtrrrzlpnp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ybcxt.top/gtkpmncbyf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zdqjudy.top/gtpyzeaqyl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtlhugarwb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gthkfnquyt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtunejeqkl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gzhubu.top/gtsomubxek.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xinyue.icu/gtxazrrzrh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ppjwa.cn/gtdsudhylf.html

[B13] 判断是否为数字
来源：http://hz.tianlin.xyz/gtdobhetns.html

Py:   isinstance(x, (int, float))
来源：http://hz.ivvv.top/gtkxvkxhbz.html

PHP:  is_numeric($x)
来源：http://hz.kuanghao11.cn/gtbzdzecpm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtknfechvp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gthwbabxbi.html

Java: x instanceof Number
来源：http://hz.svipenyu.cn/gtzbujsimn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ehwqpu.com/gtppacpvtg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.andypj.xyz/gtyvxresge.html

C#:   x is int or double or decimal
来源：http://hz.hfpthk.cn/gtlcgktvkd.html

[B14] 判断值是否在集合内
来源：http://hz.ywan-chungtsiang.top/gtzliojehu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenjidiqi.icu/gtxfvphqkp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gtevbbboet.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtxrxwnuhf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yvedp.cn/gtgvrjflap.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.feifeiyinyue.top/gtodvohwtv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hfpthk.cn/gtzmqmgeae.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ywan-chungtsiang.top/gthvzvriab.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenjidiqi.icu/gtqeblsvqm.html

[B15] 布尔运算与取反
来源：http://hz.gaohongyu789.top/gtbiwftdbo.html

Py:   a and b or not c
来源：http://hz.yangfankeji.com/gtlcicgkea.html

PHP:  $a && $b || !$c
来源：http://hz.feifeiyinyue.top/gtknkeaygs.html

JS:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtgnydkkpo.html

TS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtkhtscowk.html

Java: a && b || !c
来源：http://hz.xuanzx.com/gtjquagbrd.html

Go:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtcyweffpm.html

Ruby: a && b || !c
来源：http://hz.hongshengwenyu.top/gtypgvzrxq.html

C#:   a && b || !c
来源：http://hz.cqqwz.cn/gtpjyqwlbu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.c1oappe.top/gtwlaubvnk.html

Py:   if not data: return
来源：http://hz.ydjk.org.cn/gtzgierzxs.html

PHP:  if (!$data) { return; }
来源：http://hz.cucudq.cn/gtyprhyuyc.html

JS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtddqshesj.html

TS:   if (!data) return;
来源：http://hz.gzhubu.top/gtazwlkcaf.html

Java: if (data == null) return;
来源：http://hz.sxryk.cn/gtoyqkbjwn.html

Go:   if data == nil { return }
来源：http://hz.shanyushiyangkeji.top/gttdiwvtkt.html

Ruby: return if data.nil?
来源：http://hz.daria6918.cn/gtryzmarew.html

C#:   if (data == null) return;
来源：http://hz.tanke756.top/gtrpselahn.html

================================================================================
来源：http://hz.yvedp.cn/gtxipgjizh.html

C. 函数与作用域
来源：http://hz.jlsjyb.cn/gtavhxpqoa.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxpaweuld.html

[C01] 定义函数
来源：http://hz.zhongyouzk.top/gtskwskdyg.html

Py:   def add(a, b): return a + b
来源：http://hz.tian-w.cn/gtifiloamw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtobcskoxo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gthiijrdtc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtbcucaxza.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtunudpedq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cashguo.top/gtllinmlqk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhiwuduotai.top/gtvfbjvcju.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtouqgpsyp.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gttbfcnvkn.html

Py:   def greet(name="World"): return name
来源：http://hz.zhijiandao.cn/gtlbloyxhc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tanke756.top/gtpizvsjmk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydzc1.top/gtgspthomn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xylfe.cn/gtvyfkourz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj202588.top/gtkwbtutns.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhixingplan.top/gtpkypjtvm.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenlongwang.top/gtvrwjoylg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.0kj1m.cn/gtfawbxlec.html

[C03] 可变参数
来源：http://hz.shuidangran.top/gtlckskzxd.html

Py:   def total(*args): return sum(args)
来源：http://hz.yangfankeji.com/gtgcvsgnmj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xingfuxueyuan.xyz/gthryawdqv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtiifwjvgb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ybcxt.top/gtqqsthczm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgfzy.top/gtzebqatkb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuxming.cn/gtlywibybh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tianlin.xyz/gttkiszske.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.0kj1m.cn/gtbbqphjed.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtnhysqjns.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cucudq.cn/gtaxycjghs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hywenlv.cn/gtknqganse.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtbjqrofno.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jianghu66.top/gtpruhqboi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yonumen.top/gtjhcfzreg.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtszuqhboo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtxfigjali.html

C#:   f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtevewsldu.html

[C05] 返回多个值
来源：http://hz.shzxlz.cn/gtvcrcxdij.html

Py:   return a, b
来源：http://hz.316326.xyz/gthrcqsqjs.html

PHP:  return [$a, $b];
来源：http://hz.haohaochexian.top/gtityokary.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tianlin.xyz/gtypxfgyfx.html

TS:   return { a, b };
来源：http://hz.c1oappe.top/gtyokujdhq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zdqjudy.top/gtthfwdjud.html

Go:   return a, b
来源：http://hz.c1oappe.top/gtjbjwamve.html

Ruby: return a, b
来源：http://hz.ydzc1.top/gtwfwkhrse.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.9152youxi.cn/gtiasxdues.html

[C06] 匿名函数 / lambda
来源：http://hz.zhijiandao.cn/gtkeeljzfr.html

Py:   square = lambda x: x * x
来源：http://hz.havefunace.top/gtqmeziszx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gtlovvxceb.html

JS:   const square = x => x * x;
来源：http://hz.yvedp.cn/gtvvdeechg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.havefunace.top/gtqqzmezoi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hnxiangtu.top/gtehlrjacs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.c1oappe.top/gtskzellsd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yuanzhike.top/gtnywttsav.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yonumen.top/gttgeudcga.html

[C07] 把函数作为参数传入
来源：http://hz.gaohongyu789.top/gtzrfjsreg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xingfuxueyuan.xyz/gtyzlovdbd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxuanxn.top/gtmrxncrxu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtddnsjtcm.html

TS:   arr.map(String)
来源：http://hz.cdnleiting.top/gtjwbpwclq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dianchejie.cn/gtkkidsnwv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sysykeji.top/gtgmgdlswc.html

Ruby: arr.map(&:upcase)
来源：http://hz.jqgufenzy.top/gtgcqolkau.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnxiangtu.top/gtlmmeexbz.html

[C08] 闭包
来源：http://hz.yj20258888.top/gtelrjnayi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangshuangyany.cn/gtcsssyten.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sxryk.cn/gtgnsvyurz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtrobwtngo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gtvmodhqte.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.316326.xyz/gttxhwuqdf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tianlin.xyz/gtebvxmggi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yangfankeji.com/gtjyvvarny.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtvgmdqqwj.html

[C09] 递归
来源：http://hz.sweek.top/gtcpxycxcl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtylyriviu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aizwys.cn/gtqydfrecf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtfcogxvsn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtwuritrzp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.daxiang520.top/gtexiumyth.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daria6918.cn/gtneizjprz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtxvwxrxbc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hysaishi.cn/gtpkcibmpb.html

[C10] 变量作用域
来源：http://hz.ywan-chungtsiang.top/gtyymiikhu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuanzx.com/gtaggbfbdy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.bjfxy.top/gtrdzjnfjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtscoqzdsj.html

TS:   同 JS
来源：http://hz.yangfankeji.com/gtstzkbipt.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtutieyhdm.html

Go:   花括号块级作用域
来源：http://hz.daria6918.cn/gtvlhmsrbg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yueranfly.top/gttzntvkdr.html

C#:   块级作用域
来源：http://hz.aizwys.cn/gtqryaqnjd.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtjqohikma.html

Py:   from module import func
来源：http://hz.ybcxt.top/gtrslohkis.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yueranfly.top/gtzgtmqqdy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yanxiufei.cn/gtiqmyeslx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hysaishi.cn/gtgwprspda.html

Java: import java.util.List;
来源：http://hz.52xcode.cn/gtjwoeamtg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigufen.top/gthaburswy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ywan-chungtsiang.top/gtqmtaomrk.html

C#:   using System.Text;
来源：http://hz.ydzc1.top/gtpuduarlk.html

[C12] 立即执行函数 IIFE
来源：http://hz.ivvv.top/gtoctlzpag.html

Py:   (lambda: print("run"))()
来源：http://hz.dashuyun.cn/gtzsolbead.html

PHP:  (function () { echo "run"; })();
来源：http://hz.0kj1m.cn/gtjqnkjhvv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtlmbxjomv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtpjlvanem.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.52xcode.cn/gtqwvwquqi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ehwqpu.com/gtbuqcqtci.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtnhxupvdo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gzhubu.top/gtuykgthwu.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258888.top/gtsvuqiuxt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.bjfxy.top/gtysqdwpxp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtjzkawtps.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ybcxt.top/gtqeweyoje.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtzquyofqz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtcjedredq.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gttxgqtkbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhiwuduotai.top/gtcsdnspcq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj202588.top/gtlnonwhep.html

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gthqrhzgxg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtukaoeatd.html

PHP:  // 无泛型
来源：http://hz.fengsongda.top/gtgrlnoapa.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtnodfwnfq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhaomingkeji.xyz/gtuxzriwnt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtswlqthqv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xylfe.cn/gtgkrxqxkd.html

Ruby: # 无泛型
来源：http://hz.jinqigfzy.top/gtswljhvwu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gtfwbatogw.html

[C15] 解构 / 展开参数
来源：http://hz.sysykeji.top/gtemhkwlax.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zycfv.cn/gtyntxddok.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jlsjyb.cn/gteokmoyyr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtgmninzhs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.havefunace.top/gtwthevuzy.html

Java: // 无解构
来源：http://hz.xuetiantiany.cn/gteousbrpm.html

Go:   // 无解构
来源：http://hz.dashuyun.cn/gtigywukaa.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtwbtoytvq.html

C#:   var (a, b) = pair;
来源：http://hz.tanke756.top/gtktpoudoh.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtmzotfacx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.daxiang520.top/gtuckbxteq.html

PHP:  // 无重载
来源：http://hz.hammf.cn/gthbrhqddx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gthxdoieuw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sufxvd.cn/gtlxyvfojx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtinfstcwy.html

Go:   // 无重载：用不同函数名
来源：http://hz.mhx1999.top/gtilzjowte.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenzaomai.com/gtdmokitsm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtsjdaljms.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtseifoegg.html

D. 数组 / 列表 / 集合
来源：http://hz.zdqjudy.top/gtdtngvaru.html

================================================================================
来源：http://hz.yj20258.top/gthvkudopc.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258.top/gtcmgltqej.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ybcxt.top/gtpzbmvuqn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtbsznzuiz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yonumen.top/gtzacpntfm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhixingplan.top/gtlahlgiaq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.wangshuangyany.cn/gtyvkexvxl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gtikboimji.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtvurszwke.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.smart0.xyz/gtqcqqzude.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gticgjanhj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuanzx.com/gtededazzv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shangyingyoupin.top/gtolfhtyia.html

JS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtlaebmbbr.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtufytnnqc.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtnssnfqfb.html

Go:   arr = append(arr, 4)
来源：http://hz.zhixingplan.top/gtifygecgw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtumgmdzcu.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtwkxiwmwi.html

[D03] 在指定位置插入元素
来源：http://hz.52xcode.cn/gttdzquuvd.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtjktlnzck.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pycfn.com/gtuzniiydw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cucudq.cn/gtiliipuon.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.birdmap.top/gtdnrzfrtn.html

Java: list.add(0, 0);
来源：http://hz.ppjwa.cn/gtvmtrlqsj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jlsjyb.cn/gtifkhwamg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.birdmap.top/gtnhjcleaj.html

C#:   list.Insert(0, 0);
来源：http://hz.zhijiandao.cn/gtldvfabwt.html

[D04] 删除元素
来源：http://hz.hammf.cn/gtdwlulhpl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtzjawcbdh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sweek.top/gtrwotbkty.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtbkfjdytz.html

TS:   arr.splice(0, 1);
来源：http://hz.316326.xyz/gtwvcybmku.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daria6918.cn/gteiobxnzl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sysykeji.top/gtkwwkfusg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yonumen.top/gtctabbbgz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj202588.top/gtmaqgzwam.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gteukntlar.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aizwys.cn/gtryvuulbi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gtgucosadk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tian-w.cn/gtboqnuqhx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenjidiqi.icu/gtnrnmtjjb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xinyue.icu/gtuczoqcpi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtlxkjcmzq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtnbqnyhgu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.haohaochexian.top/gtetsqfkcj.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtkqbikmrv.html

Py:   len(arr)
来源：http://hz.zycfv.cn/gtyoudyief.html

PHP:  count($arr);
来源：http://hz.xziqi.cn/gtyvvajrqv.html

JS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtzqcnynij.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtpogkwqtx.html

Java: list.size();
来源：http://hz.jianghu66.top/gtkuxcokkn.html

Go:   len(arr)
来源：http://hz.hongshengwenyu.top/gtozxguali.html

Ruby: arr.length; arr.size
来源：http://hz.meibo888.top/gtixbcwjfi.html

C#:   list.Count;
来源：http://hz.guannengcc.top/gtmvxfhqib.html

[D07] 切片 / 取子数组
来源：http://hz.svipenyu.cn/gtfuceookg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.wangshuangyany.cn/gtpdjsorwe.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xinyue.icu/gtibduqazj.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtraaxmhki.html

TS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtpdqwuamd.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtatcpshyq.html

Go:   arr[1:4]
来源：http://hz.fengsongda.top/gtfotrtncc.html

Ruby: arr[1, 3]
来源：http://hz.fzhhl.top/gtajtbwzfg.html

C#:   list.GetRange(1, 3);
来源：http://hz.zycfv.cn/gtpgurqtbm.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtghwcekyd.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gthwhkdyba.html

PHP:  array_merge($a, $b);
来源：http://hz.aizwys.cn/gtxpthhhai.html


<!-- 参考信息 -->