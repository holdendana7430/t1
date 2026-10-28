代发 wailian999

Py:   return a, b
来源：http://hz.tianlin.xyz/gtgdmkwisz.html

PHP:  return [$a, $b];
来源：http://hz.birdmap.top/gtfcrrkfuy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jianghu66.top/gtqtonvbnf.html

TS:   return { a, b };
来源：http://hz.yuxming.cn/gtnotbdolg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pengpengdd.cyou/gthofgvxbi.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtsijbkpgv.html

Ruby: return a, b
来源：http://hz.xingfuxueyuan.xyz/gtjtqtjdvk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yangfankeji.com/gttjpnctac.html

[C06] 匿名函数 / lambda
来源：http://hz.hywenlv.cn/gthdwfnhfc.html

Py:   square = lambda x: x * x
来源：http://hz.sysykeji.top/gtthwokfoq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hammf.cn/gtspyvnbki.html

JS:   const square = x => x * x;
来源：http://hz.vqdsnc.cn/gtwyahdmml.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gtbnzmyoso.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cashguo.top/gtuqquwhxs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.svipenyu.cn/gtenxlpmck.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shangyingyoupin.top/gtksdevhaj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.aibaodan.cn/gttlknwzae.html

[C07] 把函数作为参数传入
来源：http://hz.redwolf501.top/gterfmdkcp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jyoumei.cn/gtavjouwga.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ybcxt.top/gtmchostse.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.kuanghao11.cn/gtrrfktdjr.html

TS:   arr.map(String)
来源：http://hz.pycfn.com/gtixlzqbjw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangshuangyany.cn/gtgmgexufl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtntoiwefa.html

Ruby: arr.map(&:upcase)
来源：http://hz.jqgufenzy.top/gtzrlzkwsq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydzc1.top/gtmffnhghi.html

[C08] 闭包
来源：http://hz.zhiwuduotai.top/gtfhppeibu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtbwjealyh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yvedp.cn/gthmoqvdce.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtmbvdhcgj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtdicjrggh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenjidiqi.icu/gtrzuosqcv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yangfankeji.com/gtfjathykd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xinyue.icu/gtvbdrrqra.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtykjmgrjc.html

[C09] 递归
来源：http://hz.dashuyun.cn/gtyzkmpnbs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj202588.top/gtxkitoibz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shangyingyoupin.top/gtcqyoorgz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtgteenipn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cashguo.top/gtpkdwwjvj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhengqikj.top/gteahjpsfq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.0kj1m.cn/gtylwusxwc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtbxayqpbi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnxiangtu.top/gtfnkdqbtp.html

[C10] 变量作用域
来源：http://hz.yj20258888.top/gtjnfllzak.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhiwuduotai.top/gthqfclgbt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.iojbl.cn/gtqjhyestb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tian-w.cn/gtskhfppkq.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gthhndtlix.html

Java: 方法内为块级作用域
来源：http://hz.dianchejie.cn/gththwnlem.html

Go:   花括号块级作用域
来源：http://hz.zdqjudy.top/gtlkiggiag.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydjk.org.cn/gtslsxwwin.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gtktzulmlt.html

[C11] 模块导入与导出
来源：http://hz.ybcxt.top/gtxrmgoygi.html

Py:   from module import func
来源：http://hz.chenlongwang.top/gtmfwcxcah.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hysaishi.cn/gttntthwai.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sweek.top/gtkmflhcph.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sweek.top/gtcdtveqfx.html

Java: import java.util.List;
来源：http://hz.chenjidiqi.icu/gtttqkmzge.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yongpay.top/gtfxrvtgsu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ppjwa.cn/gtridxnjga.html

C#:   using System.Text;
来源：http://hz.svipenyu.cn/gtsoghrddy.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtzrhgtltq.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtscpfxvda.html

PHP:  (function () { echo "run"; })();
来源：http://hz.52xcode.cn/gtxxzrohqk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtzwnuvoss.html

TS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gtpfcqkvgy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnqzz.top/gtjdtomulg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtxjyfdwqp.html

Ruby: -> { puts "run" }.call
来源：http://hz.haohaochexian.top/gtwyvbnipr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sxryk.cn/gtqulklwvp.html

[C13] 类型声明 / 类型注解
来源：http://hz.hywenlv.cn/gttigtjdcb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gtxvchhcwp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtmmgyzqzy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gaohongyu789.top/gthqtonccc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtpzgbfuus.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtoaclpprb.html

Go:   func add(a, b int) int
来源：http://hz.ydjk.org.cn/gtmzskwlch.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sxryk.cn/gtjjkyexts.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.havefunace.top/gtdbautblt.html

[C14] 泛型函数
来源：http://hz.shzxlz.cn/gtqowzspdl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.pycfn.com/gtpagjgdun.html

PHP:  // 无泛型
来源：http://hz.guannengcc.top/gtkioijgbl.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gtqtbumdcs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yvedp.cn/gthaavcvor.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dashuyun.cn/gtnipyvvlx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtystmgjew.html

Ruby: # 无泛型
来源：http://hz.wangdashe.top/gtadfoaxqx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yongpay.top/gtwpeajtef.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtqxvymnap.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtixxzkxkz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shangyingyoupin.top/gtxmpmlsjd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtqnsazfjr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtjkmprdhl.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gtabnxxqnv.html

Go:   // 无解构
来源：http://hz.nanxuanxn.top/gtqwydqppq.html

Ruby: a, b = pair
来源：http://hz.yj20258888.top/gtijgydsuh.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gtkewbsili.html

[C16] 函数 / 方法重载
来源：http://hz.yanxiufei.cn/gtzhkmpvfb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gaohongyu789.top/gtednmojxq.html

PHP:  // 无重载
来源：http://hz.zhiwuduotai.top/gtcppzwhjx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtqnoyzwen.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangshuangyany.cn/gtzwncdggr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xingfuxueyuan.xyz/gtdiomfvjk.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgfzy.top/gtwefxtwwq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangdashe.top/gtodofxxlq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.52xcode.cn/gtwpmycppa.html

================================================================================
来源：http://hz.yuxming.cn/gtlroculvj.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtpsqzqjox.html

================================================================================
来源：http://hz.xuanzx.com/gtbtncqfdl.html

[D01] 创建数组 / 列表
来源：http://hz.snrcjt.cn/gtsgqttshu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.0kj1m.cn/gtyeiethvb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.andypj.xyz/gtglnoctah.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sufxvd.cn/gtcafxzphe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.smart0.xyz/gtyeziuxmn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangkeji.top/gtnoyrlalw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenlongwang.top/gtjavoyosw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gttcvpgjnp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.vqdsnc.cn/gtanuunpxu.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gtajksqbca.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtmyppwkrc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.0kj1m.cn/gtfindnsvs.html

JS:   arr.push(4);
来源：http://hz.zhixingplan.top/gthnwfkqtc.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtlufsfwab.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gtmejaeera.html

Go:   arr = append(arr, 4)
来源：http://hz.daria6918.cn/gtiiynsgrf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jiagoushi.top/gtoqpntiuy.html

C#:   list.Add(4);
来源：http://hz.yonumen.top/gtcdkvtqha.html

[D03] 在指定位置插入元素
来源：http://hz.shuidangran.top/gtovvwsxuw.html

Py:   arr.insert(0, 0)
来源：http://hz.sufxvd.cn/gtgtifgynp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yvedp.cn/gtdnqzefge.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxuanxn.top/gtfafghlto.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.meibo888.top/gttngndknf.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gthulqgypo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.kuanghao11.cn/gtynlggsdb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cdnleiting.top/gtfnsmizqi.html

C#:   list.Insert(0, 0);
来源：http://hz.guowangkeji.top/gtuhabaube.html

[D04] 删除元素
来源：http://hz.shanyushiyangtech.top/gtsbsrcclr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gtsdlepkqf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shzxlz.cn/gtkmsqaath.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj20258888.top/gtqjrzxrga.html

TS:   arr.splice(0, 1);
来源：http://hz.zdqjudy.top/gtxwhjicsw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gthmgksuzk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtonjnngzz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jlsjyb.cn/gtvmhagwsx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cheryme.top/gtghyftyjo.html

[D05] 访问与修改元素
来源：http://hz.chenzaomai.com/gtgplulppf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtxdwoecnr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtoyygcsui.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.52xcode.cn/gtpchizfll.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gtkjefmjgs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.52xcode.cn/gtkwahqtrz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtngafesoh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gthcrypldc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtnekuizin.html

[D06] 数组长度
来源：http://hz.meibo888.top/gtnyghrazg.html

Py:   len(arr)
来源：http://hz.cheryme.top/gtcublkskd.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtvuhwewbo.html

JS:   arr.length
来源：http://hz.9152youxi.cn/gtypuykvdz.html

TS:   arr.length
来源：http://hz.ppjwa.cn/gtepqijekt.html

Java: list.size();
来源：http://hz.kuanghao11.cn/gtrhytadzn.html

Go:   len(arr)
来源：http://hz.ppjwa.cn/gtrfjtldrq.html

Ruby: arr.length; arr.size
来源：http://hz.c1oappe.top/gtadvbrwfc.html

C#:   list.Count;
来源：http://hz.yj20258.top/gtxzqnwwed.html

[D07] 切片 / 取子数组
来源：http://hz.chenlongwang.top/gtvhmrhzqc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ehwqpu.com/gtxdxblual.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhengqikj.top/gtylonczks.html

JS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtvlblavsp.html

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtlpewuuwm.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtuxyhmphu.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gtuqhcfgvc.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtbtoimkaf.html

C#:   list.GetRange(1, 3);
来源：http://hz.jyoumei.cn/gtinqowtrj.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtnedasmze.html

Py:   a + b;  a.extend(b)
来源：http://hz.ybcxt.top/gtyoewjzxp.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtfyoreewq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtzfcxklel.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtxhrjrbgb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhijiandao.cn/gtiazemlrj.html

Go:   append(a, b...)
来源：http://hz.xinyue.icu/gtdejtveuf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gtjybflooq.html

C#:   a.Concat(b).ToList()
来源：http://hz.shangyingyoupin.top/gtzcytzyah.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtjtbsrfxn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtjsqaymuw.html

PHP:  sort($arr);
来源：http://hz.daxiang520.top/gtizrdydbg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yongpay.top/gtvgklqvgi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.52xcode.cn/gtihqfuzvn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtqrjjyjup.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtsyxbeezm.html

Ruby: arr.sort
来源：http://hz.yj20258888.top/gtrmtzdtoy.html

C#:   list.Sort();
来源：http://hz.guowangkeji.top/gtfgevzaaj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xingfuxueyuan.xyz/gtdczglnch.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenzaomai.com/gtdhqgzxix.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtraxqvzgu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtstbwrwcb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtcdqsdwxh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fengsongda.top/gtfhcwvwyc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtaxrklzfj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtodxnmimq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigufen.top/gtgwwgpdct.html

[D11] 反转数组
来源：http://hz.dashuyun.cn/gtlgkvxxqi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtbmttbwoj.html

PHP:  array_reverse($arr);
来源：http://hz.shzxlz.cn/gtzpmxwrpj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hysaishi.cn/gtttoocivo.html

TS:   [...arr].reverse();
来源：http://hz.snrcjt.cn/gtbfeyzvky.html

Java: Collections.reverse(list);
来源：http://hz.kuanghao11.cn/gtdsdiatnl.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtubyxdhvt.html

Ruby: arr.reverse
来源：http://hz.9152youxi.cn/gtilnruqma.html

C#:   list.Reverse();
来源：http://hz.gaohongyu789.top/gthinfzkyt.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtxjcscfhg.html

Py:   arr.index(x);  x in arr
来源：http://hz.hammf.cn/gtyccogbwl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.0kj1m.cn/gtfkzvyzcq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtyejqczqc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gthzmnubhx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtuomwjlsv.html

Go:   slices.Index(arr, x)
来源：http://hz.bjfxy.top/gthtqewjbk.html

Ruby: arr.index(x)
来源：http://hz.haohaochexian.top/gtrqddnmcm.html

C#:   list.IndexOf(x);
来源：http://hz.jinyuanbaomall.cn/gtzrqchjpp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sxryk.cn/gtcyxwpgkj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenjidiqi.icu/gtiohiuavg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuanzhike.top/gtrxryjzyd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtjabkqpro.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtbmvuqyyw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtzntolpzo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnxiangtu.top/gthyyzaxqw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zdqjudy.top/gtyzqolkhm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nwbrower.top/gtffrwaltg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhijiandao.cn/gtdznjdfos.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtcvqhgqrb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gtqwasndak.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gttutpjkxb.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxinkj.top/gtmvchzivc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhongyouzk.top/gtamqbxzsi.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtasypndmc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guowangkeji.top/gtrbqbojtp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.vqdsnc.cn/gtnsbyzzva.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtvvpjrzzj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtmqpbkkqw.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gtxwpsrtdu.html

JS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtdtganwdd.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtajmgjiqz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtmxxektwq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jiagoushi.top/gtipwwyuvc.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtfioadzgj.html

C#:   list.Distinct().ToList()
来源：http://hz.andypj.xyz/gtsfdmdfjg.html

[D16] 求和与平均值
来源：http://hz.jqgfzy.top/gtbqtwkgrj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.svipenyu.cn/gtvkuepqzf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cucudq.cn/gtsnxkcqrk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtpitwurkj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtqyemtuqy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sysykeji.top/gtqyixhtlj.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtxfmoqhgk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gtbphybpnj.html

C#:   list.Sum();  list.Average()
来源：http://hz.daxiang520.top/gtfdhbljye.html

[D17] 最大值与最小值
来源：http://hz.jiagoushi.top/gtkdeqkudm.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtesdizvkl.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuanzx.com/gtmhggriwo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenzaomai.com/gtjaafniys.html

TS:   Math.max(...arr);
来源：http://hz.hammf.cn/gtwxmwhtdb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnxiangtu.top/gtbrbkbeja.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tian-w.cn/gtebruvgic.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gtbkxjjrmc.html

C#:   list.Max();  list.Min()
来源：http://hz.vqdsnc.cn/gtgjzhvzgv.html

[D18] 扁平化嵌套数组
来源：http://hz.9152youxi.cn/gtafpdipja.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gogol.net.cn/gtmkbcnyhs.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtlxoussaq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtnsxgbgbd.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gtjtimkuyt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yonumen.top/gtuacoisgz.html

Go:   // 手写双层循环
来源：http://hz.ivvv.top/gtjzznjkdd.html

Ruby: nested.flatten
来源：http://hz.bjfxy.top/gtbcqoeqmm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtqgoezadi.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtxvsrgdue.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pengpengdd.cyou/gtkkxeogfr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fengsongda.top/gtzkhoyxfr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.quarkkingdee.top/gtwurrdyyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinyuanbaomall.cn/gtajclsezq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aizwys.cn/gtqnxyukto.html

Go:   // 手写 map[string][]T
来源：http://hz.haohaochexian.top/gthtggifuv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pycfn.com/gtnlvywlos.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.kuanghao11.cn/gtdvzoihrq.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtviifurmu.html

Py:   Counter(arr)
来源：http://hz.yj20258888.top/gtryztrafe.html

PHP:  array_count_values($arr);
来源：http://hz.birdmap.top/gtfbyldiwo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtjpjzqgke.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtegvcpbwx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtopnjhagn.html

Go:   // 手写 map[T]int
来源：http://hz.snrcjt.cn/gtcjngswjq.html

Ruby: arr.tally
来源：http://hz.hywenlv.cn/gthzyozyxs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtlrmceyxs.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtrxzjlgkk.html

Py:   x in arr
来源：http://hz.ywan-chungtsiang.top/gtpuawhywx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuanzx.com/gtlhhbforu.html

JS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtzmcuqgjp.html

TS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gttvbpqwqs.html

Java: list.contains(x)
来源：http://hz.ydzc1.top/gtngdnuxlt.html

Go:   slices.Contains(arr, x)
来源：http://hz.smart0.xyz/gtqgisoprp.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gttqskpvwu.html

C#:   list.Contains(x)
来源：http://hz.wangdashe.top/gtvuxiplfg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gzhubu.top/gtxwntgyzm.html


<!-- 参考信息 -->