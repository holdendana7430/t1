代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gturnhvqzw.html

[B10] 遍历同时拿索引
来源：http://hz.dianchejie.cn/gtbsxflubh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ybcxt.top/gthjwiurur.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.nanxuanxn.top/gtwmygtprv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sxryk.cn/gtdbxamlbd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sufxvd.cn/gtdodrdflz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinghuilouyu.cn/gtthhitrao.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hfpthk.cn/gtzotztuhn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gotoacloud.top/gtzgcmqnrr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.kuanghao11.cn/gtaxxmofem.html

[B11] 生成数字序列 / 区间
来源：http://hz.cdnleiting.top/gtnxojoryy.html

Py:   list(range(0, 10, 2))
来源：http://hz.jiagoushi.top/gtohsnlqdz.html

PHP:  range(0, 10, 2);
来源：http://hz.wangdashe.top/gtjueuvgcd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aibaodan.cn/gtiwaqjika.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.52xcode.cn/gtgufdurzo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shuidangran.top/gtgqfmzejp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinghuilouyu.cn/gtckgmreqy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinqigufen.top/gtogoyxyju.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tanke756.top/gtjuhebtwz.html

[B12] 跳出多层循环
来源：http://hz.sxryk.cn/gtwdcbdbyi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xylfe.cn/gtlixucryx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenzaomai.com/gtvatvbbnj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtqrkwvjcy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtipdtqszx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtzsjeujzg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.feifeiyinyue.top/gtsszeocix.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cheryme.top/gtgwizddcy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yanxiufei.cn/gtasbupyry.html

[B13] 判断是否为数字
来源：http://hz.daxiang520.top/gtouhbzabd.html

Py:   isinstance(x, (int, float))
来源：http://hz.cashguo.top/gtvsdxyrqi.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtqttykezj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtzccswkgw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangtech.top/gtsnfdhzbj.html

Java: x instanceof Number
来源：http://hz.c1oappe.top/gtizmihgrc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tian-w.cn/gtfbrizzdr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daxiang520.top/gtejrmmkoi.html

C#:   x is int or double or decimal
来源：http://hz.fengsongda.top/gtwoefmkne.html

[B14] 判断值是否在集合内
来源：http://hz.cheryme.top/gtzvrikccm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.bjfxy.top/gtpvickcsr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hywenlv.cn/gtyjzhqfzv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.fengsongda.top/gthjbxhwoe.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gthxihfqbc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xuetiantiany.cn/gtgvzcxfss.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.vqdsnc.cn/gtqhlieyyg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shangyingyoupin.top/gtgupojpyv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shanyushiyangtech.top/gtdiwqlmga.html

[B15] 布尔运算与取反
来源：http://hz.yueranfly.top/gthmgjaeou.html

Py:   a and b or not c
来源：http://hz.quarkkingdee.top/gtfhmijorx.html

PHP:  $a && $b || !$c
来源：http://hz.tanke756.top/gthzpbrwew.html

JS:   a && b || !c
来源：http://hz.dashuyun.cn/gtlsxnnwpe.html

TS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtvehoeenu.html

Java: a && b || !c
来源：http://hz.ivvv.top/gtugetzfpb.html

Go:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtyffqojax.html

Ruby: a && b || !c
来源：http://hz.zdqjudy.top/gtekphgthe.html

C#:   a && b || !c
来源：http://hz.hnqzz.top/gtnczxtfcj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gttuhyhcom.html

Py:   if not data: return
来源：http://hz.guannengcc.top/gthdhahprp.html

PHP:  if (!$data) { return; }
来源：http://hz.shuidangran.top/gtixyzevln.html

JS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtvfdeuosa.html

TS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtpkhtqubn.html

Java: if (data == null) return;
来源：http://hz.wangshuangyany.cn/gtllunklxv.html

Go:   if data == nil { return }
来源：http://hz.ybcxt.top/gtvwbaysgi.html

Ruby: return if data.nil?
来源：http://hz.jqgfzy.top/gtgkjkgyld.html

C#:   if (data == null) return;
来源：http://hz.tanke756.top/gtwetkiszc.html

================================================================================
来源：http://hz.hysaishi.cn/gtkveemeas.html

C. 函数与作用域
来源：http://hz.guowangkeji.top/gtgevlokuz.html

================================================================================
来源：http://hz.aizwys.cn/gtwaywsoan.html

[C01] 定义函数
来源：http://hz.feifeiyinyue.top/gtqboyemyt.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtkioaussj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtmlrfapch.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cucudq.cn/gttiophfir.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtgtvmxogo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtokofdyqi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ybcxt.top/gtmtybymgx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tianlin.xyz/gtmbtxwawp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtmmqupkdq.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtrsfnjqhe.html

Py:   def greet(name="World"): return name
来源：http://hz.mhx1999.top/gtnytubwca.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gotoacloud.top/gtnvdpxklu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtnkixyzgx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtxskkkqpd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.guowangkeji.top/gtncbfpqjg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gzhubu.top/gtpxpjzwgl.html

Ruby: def greet(name = "World") = name
来源：http://hz.nwbrower.top/gtdqtngzod.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.birdmap.top/gtkaioafgj.html

[C03] 可变参数
来源：http://hz.havefunace.top/gttronjczy.html

Py:   def total(*args): return sum(args)
来源：http://hz.fengsongda.top/gtikriqreu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shuidangran.top/gtpptvfylx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtaburdebr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtocmnzaal.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gtslormzhd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.svipenyu.cn/gtuwfrpevd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenzaomai.com/gtaokcubpu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yonumen.top/gtojmbyyqz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ybcxt.top/gtzlhuphsu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.52xcode.cn/gtrjhkfjxx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenlongwang.top/gtosrfeozu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtidebmlbv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.iojbl.cn/gthpeigsap.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ywan-chungtsiang.top/gtwiojvvqe.html

Go:   // 无：用配置结构体参数
来源：http://hz.yangfankeji.com/gtaqmklbkw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtolhdbnqc.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtpyahacnx.html

[C05] 返回多个值
来源：http://hz.xingfuxueyuan.xyz/gtwuxvnyhl.html

Py:   return a, b
来源：http://hz.aizwys.cn/gtujiixmno.html

PHP:  return [$a, $b];
来源：http://hz.yj20258.top/gtbmxpibrw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.0kj1m.cn/gtqihlanxn.html

TS:   return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtnquvpgut.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yangfankeji.com/gtymbpbela.html

Go:   return a, b
来源：http://hz.cdnleiting.top/gtdtvrqzyr.html

Ruby: return a, b
来源：http://hz.redwolf501.top/gtevzejnxr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gthlivlyhz.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtqrfucrrf.html

Py:   square = lambda x: x * x
来源：http://hz.9152youxi.cn/gtrknoopgm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cucudq.cn/gtqrumwwld.html

JS:   const square = x => x * x;
来源：http://hz.nwbrower.top/gtvjsnewvs.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shuidangran.top/gtqibputuy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hammf.cn/gtlaermwzh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gthnvzzvvx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yonumen.top/gtiwtptpgi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gtgnykzhgd.html

[C07] 把函数作为参数传入
来源：http://hz.xuetiantiany.cn/gtzggtelwc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinghuilouyu.cn/gtsoutyitv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yueranfly.top/gtkqdcbfal.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtuylygmni.html

TS:   arr.map(String)
来源：http://hz.yj202588.top/gtgiyxsmpy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guowangkeji.top/gtjsdlratk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tian-w.cn/gtoeqxumfo.html

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtytkihgzc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jiagoushi.top/gtcbbikwkp.html

[C08] 闭包
来源：http://hz.yanxiufei.cn/gtqkpztzjh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ppjwa.cn/gtlzhtoagk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.smart0.xyz/gtgafgohfi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtsvankide.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtigsajlyi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tianlin.xyz/gtbmmsxfbr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhongyouzk.top/gtcvdajtya.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhixingplan.top/gtcmzqyrbg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtlzgzdhqk.html

[C09] 递归
来源：http://hz.ydjk.org.cn/gtsqthocmi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtnbtbyvxb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.feifeiyinyue.top/gtlzordkur.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtnysayydl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtiirgebkp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aibaodan.cn/gtccbxjgqh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aizwys.cn/gtdgcmqyaj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fzhhl.top/gtalexwhgq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhiwuduotai.top/gtrkhoyvry.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtjwrldqtg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tian-w.cn/gtjvvhjhdq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daria6918.cn/gtcmgsvcfa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hywenlv.cn/gtxmmbsozv.html

TS:   同 JS
来源：http://hz.smart0.xyz/gtxrzesfyq.html

Java: 方法内为块级作用域
来源：http://hz.zhengqikj.top/gtztetazpt.html

Go:   花括号块级作用域
来源：http://hz.fzhhl.top/gtotogoncv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtcvxqiyvo.html

C#:   块级作用域
来源：http://hz.yonumen.top/gtlynbrsce.html

[C11] 模块导入与导出
来源：http://hz.0kj1m.cn/gtozwpcwau.html

Py:   from module import func
来源：http://hz.hysaishi.cn/gtxaqrqujf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.iojbl.cn/gtxdkkfllp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ppjwa.cn/gthhipicfa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ivvv.top/gtxwdjqxnp.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gtubgxcsmz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aibaodan.cn/gtcecoeoqe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tian-w.cn/gtjucbjexb.html

C#:   using System.Text;
来源：http://hz.yj20258.top/gtejurualc.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtqtyqetsm.html

Py:   (lambda: print("run"))()
来源：http://hz.quarkkingdee.top/gtyybisnld.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtqgcabusj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtpxsvktkh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtjwgwxnpk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtbsjwhutf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtiarqqfir.html

Ruby: -> { puts "run" }.call
来源：http://hz.xinyue.icu/gtrfyfkjlw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ywan-chungtsiang.top/gtwfdnqsqp.html

[C13] 类型声明 / 类型注解
来源：http://hz.birdmap.top/gtteuufhxg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuxming.cn/gteandnjtr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtjbrvwnbd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.wangshuangyany.cn/gtacyjzxur.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gttygxptqz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtcsptvuaq.html

Go:   func add(a, b int) int
来源：http://hz.svipenyu.cn/gtbmyninob.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shangyingyoupin.top/gtfzaibztr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtigzfpqfi.html

[C14] 泛型函数
来源：http://hz.yj20258888.top/gtqceykluk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtcwiwjvwb.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gtasljxsha.html

JS:   // 无泛型
来源：http://hz.guowangkeji.top/gtenovbkbj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtntlyipse.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuanzhike.top/gtaqcadrec.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtpgznnwpf.html

Ruby: # 无泛型
来源：http://hz.9152youxi.cn/gtplsqwvxh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tanke756.top/gtlfyoxbnh.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gtzrbcgezi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hammf.cn/gtpiexmfnu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gthpjafxee.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtuclfrohw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtyzwyjaiz.html

Java: // 无解构
来源：http://hz.hnqzz.top/gtkdzkdblw.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtmtatgllm.html

Ruby: a, b = pair
来源：http://hz.yvedp.cn/gtgqxzdyfk.html

C#:   var (a, b) = pair;
来源：http://hz.zhixingplan.top/gtannulcrw.html

[C16] 函数 / 方法重载
来源：http://hz.hnqzz.top/gtvgkkevey.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gogol.net.cn/gtlpuqegvj.html

PHP:  // 无重载
来源：http://hz.mhx1999.top/gtunvqvhvf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenlongwang.top/gteckhjwkw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fengsongda.top/gtlglgxuhz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtvjwgklwj.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtlwmqmfnd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xinyue.icu/gtofhlcnoh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj20258888.top/gtwjcxkeft.html

================================================================================
来源：http://hz.52xcode.cn/gtewqqigxv.html

D. 数组 / 列表 / 集合
来源：http://hz.quarkkingdee.top/gtjsmtrxvs.html

================================================================================
来源：http://hz.chenzaomai.com/gtbeifqubd.html

[D01] 创建数组 / 列表
来源：http://hz.sxryk.cn/gtvyxwvnhv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gthjqmgvch.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhengqikj.top/gthqqjkdcr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangkeji.top/gtrgfcfitj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinghuilouyu.cn/gtvngbqfvr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.wangdashe.top/gtaqlelmvo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gthhgkdijn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.52xcode.cn/gtqlonjplz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhiwuduotai.top/gtzdimcyln.html

[D02] 追加元素到末尾
来源：http://hz.cashguo.top/gtxctpwyqt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.316326.xyz/gtywplioae.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gtxkrnudfm.html

JS:   arr.push(4);
来源：http://hz.fzhhl.top/gtlmeoweka.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gtocuwionw.html

Java: list.add(4);
来源：http://hz.meibo888.top/gtjdqdwysg.html

Go:   arr = append(arr, 4)
来源：http://hz.zhaomingkeji.xyz/gtizvijopz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yonumen.top/gteitaxpxa.html

C#:   list.Add(4);
来源：http://hz.0kj1m.cn/gtlonhgtjk.html

[D03] 在指定位置插入元素
来源：http://hz.zhoulong.xyz/gtuvxvoomb.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtbtzpeaaf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.52xcode.cn/gtueoynsqz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtkjxrpbfz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sysykeji.top/gtueaxyjhy.html

Java: list.add(0, 0);
来源：http://hz.andypj.xyz/gtblxcjsrf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guannengcc.top/gtnelhqqpx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.316326.xyz/gtgsukmifu.html

C#:   list.Insert(0, 0);
来源：http://hz.ybcxt.top/gtyfmdrvhu.html

[D04] 删除元素
来源：http://hz.xylfe.cn/gtkpfusirk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.guannengcc.top/gthlulawgx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtevjntaaq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtvfayjkin.html

TS:   arr.splice(0, 1);
来源：http://hz.ybcxt.top/gthmdqgrcr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jqgfzy.top/gtyrmkkhzy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtqxncajgq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jianghu66.top/gtrcusvjxx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yueranfly.top/gtvrxkmbxc.html

[D05] 访问与修改元素
来源：http://hz.wangshuangyany.cn/gtrqnifafp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtvowixbbr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtauhmkcia.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtpwsnkbyf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sysykeji.top/gtmfwsqwwi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenlongwang.top/gtficyiimw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtirzneogc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtxwoieorw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jlsjyb.cn/gthnoqetuf.html

[D06] 数组长度
来源：http://hz.jianghu66.top/gtzewgoxrg.html

Py:   len(arr)
来源：http://hz.52xcode.cn/gttjauobnz.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtpcbnevea.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtumhlwvlg.html

TS:   arr.length
来源：http://hz.cashguo.top/gtausyjvie.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtenxepylb.html

Go:   len(arr)
来源：http://hz.bjfxy.top/gtyrrdccqd.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gtifutylce.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtsgoaingd.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtfjaejwbf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtzkyvbhmg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dashuyun.cn/gtzttellmh.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtlwlzoyuw.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtdzeczgje.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtograzsda.html

Go:   arr[1:4]
来源：http://hz.pycfn.com/gtbtqsoznz.html

Ruby: arr[1, 3]
来源：http://hz.xinyue.icu/gtfeynvdyq.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gtxkxysaoo.html

[D08] 合并两个数组
来源：http://hz.ydjk.org.cn/gtmsqgbbdz.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtoaxstbqs.html

PHP:  array_merge($a, $b);
来源：http://hz.fzhhl.top/gtqvqqtjir.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtqvczquwq.html

TS:   [...a, ...b];
来源：http://hz.pengpengdd.cyou/gttdvbnwgs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fengsongda.top/gtaceuknqc.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtyzlozhex.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fzhhl.top/gtakxotypm.html

C#:   a.Concat(b).ToList()
来源：http://hz.feifeiyinyue.top/gttnhaphrz.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtbmguqfmo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtmffsqmtk.html

PHP:  sort($arr);
来源：http://hz.gogol.net.cn/gtridaluxp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fzhhl.top/gtldpvvcfi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pycfn.com/gtazpcwfzn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtxmfyjefx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtljwimkbt.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtjjtfwaaq.html

C#:   list.Sort();
来源：http://hz.yanxiufei.cn/gtqahobmeg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.meibo888.top/gteeovbyba.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yueranfly.top/gtzdmwfuaw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtxzduoziv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtewojjuov.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtifdlywzl.html


<!-- 参考信息 -->