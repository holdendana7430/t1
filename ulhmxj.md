代发 wailian999

Py:   return a, b
来源：http://hz.zhijiandao.cn/gtbhgueotz.html

PHP:  return [$a, $b];
来源：http://hz.jinyuanbaomall.cn/gteezrbmhc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jyoumei.cn/gtashbbnui.html

TS:   return { a, b };
来源：http://hz.sxryk.cn/gtatfyjivw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gtresgcylu.html

Go:   return a, b
来源：http://hz.chenlongwang.top/gttlvppmrq.html

Ruby: return a, b
来源：http://hz.jianghu66.top/gtitfclvyp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gtkvgncopt.html

[C06] 匿名函数 / lambda
来源：http://hz.zhongyouzk.top/gtkszzqgzq.html

Py:   square = lambda x: x * x
来源：http://hz.guowangkeji.top/gtojixmfbv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yonumen.top/gtvldlrfra.html

JS:   const square = x => x * x;
来源：http://hz.aibaodan.cn/gtzebnwnvm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtajtkuocv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.9152youxi.cn/gttangjnph.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nwbrower.top/gtnnuregyj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yongpay.top/gtiqprwhpf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gthbeogedt.html

[C07] 把函数作为参数传入
来源：http://hz.yuxming.cn/gtwnugbzju.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xinyue.icu/gtkeabvpip.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj20258888.top/gtfoazgpkz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gtzvnxszus.html

TS:   arr.map(String)
来源：http://hz.yangfankeji.com/gtzertunzr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yvedp.cn/gtapznbqjh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.feifeiyinyue.top/gtqgqevgce.html

Ruby: arr.map(&:upcase)
来源：http://hz.cucudq.cn/gthfmyppdh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.aibaodan.cn/gtarrubkcg.html

[C08] 闭包
来源：http://hz.cqqwz.cn/gtxykixlnz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ehwqpu.com/gtnbnguqrn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dashuyun.cn/gttlholedw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtcragukem.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtnvcptwgc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtfcslfojx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtvdvnzihy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yongpay.top/gtpqlstmxl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtryfcolip.html

[C09] 递归
来源：http://hz.dianchejie.cn/gthakrdaou.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.c1oappe.top/gttoxsmhom.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.meibo888.top/gtwviqoynk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtuuqugvzu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtoispzfdz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgufenzy.top/gtnogerqxs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jlsjyb.cn/gtmeodgzuh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtjgevswml.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.snrcjt.cn/gtbijvykje.html

[C10] 变量作用域
来源：http://hz.xuetiantiany.cn/gtttijvspk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gtckqwekzi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cashguo.top/gtrnevwsbn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnxiangtu.top/gtgmsfufeb.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtcqnpkjwa.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gtjbpvgtsn.html

Go:   花括号块级作用域
来源：http://hz.sweek.top/gtipcmwglt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtrsvwftmt.html

C#:   块级作用域
来源：http://hz.ehwqpu.com/gtnaazcsdb.html

[C11] 模块导入与导出
来源：http://hz.hysaishi.cn/gtpthjtiyu.html

Py:   from module import func
来源：http://hz.tianlin.xyz/gtjycyoxlj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jianghu66.top/gtyquangyl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sysykeji.top/gtcouvihay.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hysaishi.cn/gtwmdsaeto.html

Java: import java.util.List;
来源：http://hz.hongshengwenyu.top/gtkxqwqocc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cucudq.cn/gthmxwnijm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgfzy.top/gtgxeowdex.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gtzmsipamv.html

[C12] 立即执行函数 IIFE
来源：http://hz.yueranfly.top/gtmgconbqh.html

Py:   (lambda: print("run"))()
来源：http://hz.yongpay.top/gtpbqpsbou.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zycfv.cn/gtrdqxccjt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtkcndnoby.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtkleakxnt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.dashuyun.cn/gtpjclimbx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xinyue.icu/gthicfnklg.html

Ruby: -> { puts "run" }.call
来源：http://hz.52xcode.cn/gtajcrhtci.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.c1oappe.top/gtlitjlvsr.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtlgyuwnmp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pycfn.com/gtczfhrlck.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtiliagvfs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yanxiufei.cn/gtwjbvhdqg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtimfsoxws.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtvcwxqsbf.html

Go:   func add(a, b int) int
来源：http://hz.cheryme.top/gthdusevig.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtktpfzyti.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cheryme.top/gtufwlrwmr.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gtzsnlpjjm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtdxlatggf.html

PHP:  // 无泛型
来源：http://hz.tian-w.cn/gtdsuxxjgc.html

JS:   // 无泛型
来源：http://hz.yj20258.top/gtjswshoay.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtypampprg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ehwqpu.com/gtrsqmwvkr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinyuanbaomall.cn/gtrkmixkjw.html

Ruby: # 无泛型
来源：http://hz.hongshengwenyu.top/gtbnfveahf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yvedp.cn/gtawiinmji.html

[C15] 解构 / 展开参数
来源：http://hz.zycfv.cn/gtpowpkzmp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aizwys.cn/gtptlidhga.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tianlin.xyz/gtfhbewdan.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtchcyvyec.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.iojbl.cn/gthpjfejlm.html

Java: // 无解构
来源：http://hz.9152youxi.cn/gttkfcymsb.html

Go:   // 无解构
来源：http://hz.0kj1m.cn/gtjqfgajsx.html

Ruby: a, b = pair
来源：http://hz.ppjwa.cn/gtraifyhyq.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gtqzqmisat.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtfztnuxph.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gthqclxcaf.html

PHP:  // 无重载
来源：http://hz.shangyingyoupin.top/gtvxsjgcuc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cucudq.cn/gtdbllsbbd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ppjwa.cn/gteszziimo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daxiang520.top/gtkkfoqidj.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gtudivvtmq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.mhx1999.top/gteruqvfry.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.vqdsnc.cn/gtywjhzacf.html

================================================================================
来源：http://hz.hammf.cn/gtpsevxfsc.html

D. 数组 / 列表 / 集合
来源：http://hz.dashuyun.cn/gtkmbcwivo.html

================================================================================
来源：http://hz.yvedp.cn/gtpufaswwr.html

[D01] 创建数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gthqucmkxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.c1oappe.top/gtpupaaluc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gtchjiixdt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.redwolf501.top/gtodwpkgin.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258.top/gtuoftolde.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigufen.top/gttatzdvem.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtbvouklzd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtvlxfcbfj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gtcqqhhohc.html

[D02] 追加元素到末尾
来源：http://hz.sysykeji.top/gtisbbxvys.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nwbrower.top/gtcdzgcafz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxinkj.top/gtudkklscj.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtwlfopsva.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtnsmfudkn.html

Java: list.add(4);
来源：http://hz.cashguo.top/gtwzxvpszd.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtcehiswdd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenjidiqi.icu/gtmpmjuudt.html

C#:   list.Add(4);
来源：http://hz.yanxiufei.cn/gtuqiitscc.html

[D03] 在指定位置插入元素
来源：http://hz.meibo888.top/gtjftdyolp.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtbklzkbfo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.redwolf501.top/gtpkfoaetd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.haohaochexian.top/gtinepwsfc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhiwuduotai.top/gtqiwccrxs.html

Java: list.add(0, 0);
来源：http://hz.jlsjyb.cn/gtjubbezka.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtffeoyalv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.redwolf501.top/gtbfwplkza.html

C#:   list.Insert(0, 0);
来源：http://hz.cdnleiting.top/gtugmcritt.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gtpwvzssep.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xylfe.cn/gtzdltoskx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hysaishi.cn/gtzhjgyrpx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinyuanbaomall.cn/gtxblvrlar.html

TS:   arr.splice(0, 1);
来源：http://hz.ybcxt.top/gtthshzyel.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhaomingkeji.xyz/gtzrmkzkhr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zdqjudy.top/gtxiwxcfcd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yongpay.top/gtomqdvmdk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gtxwzfrukv.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtzubxuhsy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gthdosdukn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.c1oappe.top/gtftvrsjvo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtghjviisu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.smart0.xyz/gthktetovq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cucudq.cn/gtpzskflvw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.haohaochexian.top/gttmcewixg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtdszuiomw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtesnwlhgr.html

[D06] 数组长度
来源：http://hz.cheryme.top/gtpguspsqc.html

Py:   len(arr)
来源：http://hz.dianchejie.cn/gtjfnuethh.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtaekvrigk.html

JS:   arr.length
来源：http://hz.dashuyun.cn/gtijwbzqfn.html

TS:   arr.length
来源：http://hz.xinyue.icu/gtyrsbsiwk.html

Java: list.size();
来源：http://hz.zhengqikj.top/gtzdzhhcjx.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtbdykoekw.html

Ruby: arr.length; arr.size
来源：http://hz.dashuyun.cn/gtfnpbszah.html

C#:   list.Count;
来源：http://hz.svipenyu.cn/gtghmxhpbo.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtwkntijdl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cashguo.top/gtngxmlohg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtobtenaic.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtlhmhyffe.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtwzkgouit.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtrrczprln.html

Go:   arr[1:4]
来源：http://hz.sufxvd.cn/gtqficwale.html

Ruby: arr[1, 3]
来源：http://hz.jyoumei.cn/gtgunhrlon.html

C#:   list.GetRange(1, 3);
来源：http://hz.yangfankeji.com/gtludtcfhv.html

[D08] 合并两个数组
来源：http://hz.dianchejie.cn/gtdjjzywaq.html

Py:   a + b;  a.extend(b)
来源：http://hz.haohaochexian.top/gtbfzweqlg.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxinkj.top/gtpbknhhmx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhaomingkeji.xyz/gtsxuwlmcg.html

TS:   [...a, ...b];
来源：http://hz.xziqi.cn/gtgvqzaqyi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gtqkjofouq.html

Go:   append(a, b...)
来源：http://hz.dashuyun.cn/gtfwscwutn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.iojbl.cn/gtterdditi.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtavmhjwfj.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gtftsrcltl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtiuavhmch.html

PHP:  sort($arr);
来源：http://hz.aizwys.cn/gtkosmkmjh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gttburbfnn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yvedp.cn/gtnkhcwsij.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hammf.cn/gtluaqqpue.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gttatvkgiw.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtslqoqpdx.html

C#:   list.Sort();
来源：http://hz.jinyuanbaomall.cn/gtgabfztln.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.feifeiyinyue.top/gtotcnsjol.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtksjcasuc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtqiffujiz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtkypyywsl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtcspuoyzp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhoulong.xyz/gttqrkmchi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.iojbl.cn/gtorihoehn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gttodbfadx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daxiang520.top/gtknrirwfa.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gtrbnumytb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj202588.top/gtqrhwzkgm.html

PHP:  array_reverse($arr);
来源：http://hz.smart0.xyz/gtdhzagyac.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtfotkzzen.html

TS:   [...arr].reverse();
来源：http://hz.zhoulong.xyz/gtpafocnbc.html

Java: Collections.reverse(list);
来源：http://hz.havefunace.top/gtcwvmfzbt.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtuphmpjpi.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gtxevyxmma.html

C#:   list.Reverse();
来源：http://hz.yj20258.top/gtmylxngow.html

[D12] 查找元素下标
来源：http://hz.cqqwz.cn/gtlybvbtbh.html

Py:   arr.index(x);  x in arr
来源：http://hz.aibaodan.cn/gtjfxsaece.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gtphatlsgk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtcxsvznuc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtbjohlpzi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinyuanbaomall.cn/gtlnkffurv.html

Go:   slices.Index(arr, x)
来源：http://hz.dashuyun.cn/gtqnpslmtb.html

Ruby: arr.index(x)
来源：http://hz.zhixingplan.top/gtbivdgkwg.html

C#:   list.IndexOf(x);
来源：http://hz.shzxlz.cn/gtpochpoxs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.havefunace.top/gtogksiiav.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenlongwang.top/gtrptshufd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtrakfrnrg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtxizudrwx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtgihdwvuw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xziqi.cn/gtbctevicy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shzxlz.cn/gtwornunzq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.mhx1999.top/gtxbcrlyhs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgufenzy.top/gtbeefudxh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hywenlv.cn/gtghrfukja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.vqdsnc.cn/gtsmhecxmn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenzaomai.com/gtbbozyuyo.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtghkvvgnu.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtnfblhagu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtxtqztmbd.html

Go:   // 手写循环
来源：http://hz.nanxinkj.top/gtgmzhltij.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenjidiqi.icu/gtdgwzqdmy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.smart0.xyz/gtwcwsjbff.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtqoitsvrd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ybcxt.top/gtdlmbfizn.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtsxtjxrya.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtkkvhhoyt.html

TS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtwuwiopkp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtfdfpfvpd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.316326.xyz/gtpbgtekjy.html

Ruby: arr.uniq
来源：http://hz.sufxvd.cn/gtgmjughxk.html

C#:   list.Distinct().ToList()
来源：http://hz.xziqi.cn/gtldxlfhrr.html

[D16] 求和与平均值
来源：http://hz.snrcjt.cn/gtulstjsqo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gtttfksnkc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258888.top/gtrknkxuun.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtknfamiwg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtsrljfaql.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenlongwang.top/gtlkiorejq.html

Go:   // 手写循环累加
来源：http://hz.cashguo.top/gtkkiggmop.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yueranfly.top/gtyslfsamy.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gthbjrdojc.html

[D17] 最大值与最小值
来源：http://hz.wangshuangyany.cn/gtwmegmumm.html

Py:   max(arr);  min(arr)
来源：http://hz.xylfe.cn/gthoryijcl.html

PHP:  max($arr);  min($arr);
来源：http://hz.0kj1m.cn/gtzluutrbd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtqcfxpwvp.html

TS:   Math.max(...arr);
来源：http://hz.yonumen.top/gthirkxanl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhiwuduotai.top/gtprgjpjnr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shangyingyoupin.top/gtmnznaqfb.html

Ruby: arr.max;  arr.min
来源：http://hz.feifeiyinyue.top/gtjotkciri.html

C#:   list.Max();  list.Min()
来源：http://hz.guannengcc.top/gthdtaounn.html

[D18] 扁平化嵌套数组
来源：http://hz.sweek.top/gtxfpkcjyh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhijiandao.cn/gtojfpltux.html

PHP:  array_merge(...$nested);
来源：http://hz.xuanzx.com/gtluauvumc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.daria6918.cn/gtgskodcbr.html

TS:   nested.flat();
来源：http://hz.shanyushiyangkeji.top/gtosxzhkuq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.316326.xyz/gttyfnbjpw.html

Go:   // 手写双层循环
来源：http://hz.mhx1999.top/gtbcjnobde.html

Ruby: nested.flatten
来源：http://hz.cqqwz.cn/gtepigjjxj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.0kj1m.cn/gtxhsufoqi.html

[D19] 按字段分组
来源：http://hz.zycfv.cn/gtbywpbcjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hfpthk.cn/gtfqqggqhu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fengsongda.top/gtipozvmmh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.0kj1m.cn/gtglfpwfed.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtacwhzewa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtttxkhqqs.html

Go:   // 手写 map[string][]T
来源：http://hz.zhengqikj.top/gtqtaifkrh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.feifeiyinyue.top/gtvfuvjufn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.iojbl.cn/gtizviddqe.html

[D20] 统计每个元素出现次数
来源：http://hz.yueranfly.top/gtxhjjwvuo.html

Py:   Counter(arr)
来源：http://hz.nanxinkj.top/gtiztpiukz.html

PHP:  array_count_values($arr);
来源：http://hz.yuanzhike.top/gthnnbofnx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtluedaltu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtqjzuypwt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yangfankeji.com/gthmjdwfxc.html

Go:   // 手写 map[T]int
来源：http://hz.zhaomingkeji.xyz/gtmwelwudo.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtnqaacsmm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuetiantiany.cn/gtumkgznpt.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258.top/gtkgndmqwd.html

Py:   x in arr
来源：http://hz.zhaomingkeji.xyz/gttiporpmm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cqqwz.cn/gtpcltejtz.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtiageeztq.html

TS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtggmvbqoo.html

Java: list.contains(x)
来源：http://hz.wangdashe.top/gtjqnauibz.html

Go:   slices.Contains(arr, x)
来源：http://hz.yonumen.top/gtbionqjsh.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtygmqanby.html

C#:   list.Contains(x)
来源：http://hz.bjfxy.top/gtzkklxpqh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtmdymszaa.html


<!-- 参考信息 -->