代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.xuanzx.com/gtafmwtxxy.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtcqfmnnwc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtlgwgzgbs.html

JS:   const square = x => x * x;
来源：http://hz.jyoumei.cn/gtremnyltb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jlsjyb.cn/gtmdixwafp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.andypj.xyz/gtpamsfhfw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtjodwvytl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.52xcode.cn/gtkkuocxdw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.fengsongda.top/gtqhdvyoqb.html

[C07] 把函数作为参数传入
来源：http://hz.hongshengwenyu.top/gtpqpfsshv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhaomingkeji.xyz/gtoaoedolm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgfzy.top/gtadvpnmcu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yanxiufei.cn/gtthnbvtzt.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gtjzkbmszg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangkeji.top/gthdhcfvjo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangdashe.top/gthybcugmp.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtcjlninmu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.redwolf501.top/gtqonvuati.html

[C08] 闭包
来源：http://hz.dianchejie.cn/gttvrptgxc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtqioayhhd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.snrcjt.cn/gtnqkxzpmy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtvmgezsku.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtfuqtlook.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gtyybczael.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jlsjyb.cn/gtfxuhuttw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtydjydrjm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtgakqsafz.html

[C09] 递归
来源：http://hz.fengsongda.top/gtinatjism.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gthpsijxln.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhaomingkeji.xyz/gtdrxwfcew.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtmljbvkga.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtiftujqkj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.daria6918.cn/gtgdqslnyv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ivvv.top/gtkjlmhoil.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtzchmvgxq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cucudq.cn/gtixgjuavm.html

[C10] 变量作用域
来源：http://hz.wangdashe.top/gtkukmvceb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.vqdsnc.cn/gtfjdaysds.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.kuanghao11.cn/gtzqaujamw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.0kj1m.cn/gtlywvdbzi.html

TS:   同 JS
来源：http://hz.chenjidiqi.icu/gtootllhfj.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gtjuyunbvd.html

Go:   花括号块级作用域
来源：http://hz.sxryk.cn/gtauymckcf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cucudq.cn/gtipxxelub.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gthqfzqdgr.html

[C11] 模块导入与导出
来源：http://hz.yanxiufei.cn/gtjsaylwla.html

Py:   from module import func
来源：http://hz.316326.xyz/gtpefmuzai.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtyrdajiem.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yonumen.top/gtehuinnan.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtcukaqdee.html

Java: import java.util.List;
来源：http://hz.fengsongda.top/gtxjgsixqr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtbltemdsn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhaomingkeji.xyz/gtcbulvsik.html

C#:   using System.Text;
来源：http://hz.wangdashe.top/gtpitjcprm.html

[C12] 立即执行函数 IIFE
来源：http://hz.jyoumei.cn/gteilcxxpd.html

Py:   (lambda: print("run"))()
来源：http://hz.andypj.xyz/gtdlatmuqr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.havefunace.top/gtvnosajhk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gthwhpeoiq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtjncxkcrm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.9152youxi.cn/gtpdoevxju.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hammf.cn/gtbaivbwst.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuetiantiany.cn/gtacgskplo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtwcnposco.html

[C13] 类型声明 / 类型注解
来源：http://hz.sufxvd.cn/gtngyackds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtfascmcmn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtdllqgxuz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gtxqiqdyok.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gtntdeizuq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtyrbfddxs.html

Go:   func add(a, b int) int
来源：http://hz.jqgufenzy.top/gtihtkbsaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sweek.top/gtlfwnmuwx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jianghu66.top/gtsjmlbxgm.html

[C14] 泛型函数
来源：http://hz.xziqi.cn/gteflqhvmm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtfmzfjfvd.html

PHP:  // 无泛型
来源：http://hz.ppjwa.cn/gtgibkjpnd.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtqcgtgiso.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xylfe.cn/gtqjsumako.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhoulong.xyz/gtdpmmylzw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnxiangtu.top/gtgeesyfux.html

Ruby: # 无泛型
来源：http://hz.zycfv.cn/gtywlxlbip.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gotoacloud.top/gtmyhczurj.html

[C15] 解构 / 展开参数
来源：http://hz.feifeiyinyue.top/gtytkyuxjw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.dashuyun.cn/gtdnekmnnd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gtwqzlqbcs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtabwpqhxm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhongyouzk.top/gtfiofgqqo.html

Java: // 无解构
来源：http://hz.ivvv.top/gtuvluctim.html

Go:   // 无解构
来源：http://hz.daxiang520.top/gthfmppwab.html

Ruby: a, b = pair
来源：http://hz.zhongyouzk.top/gtirizjddd.html

C#:   var (a, b) = pair;
来源：http://hz.yanxiufei.cn/gtpxobachv.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gtfoszmsyb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtgdoniwzx.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtkvfpifru.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.havefunace.top/gtqesducjt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zycfv.cn/gtsamvxfbd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gtlsphwwnp.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtadgiakor.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj20258.top/gtveflkauk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigfzy.top/gtfmflrrps.html

================================================================================
来源：http://hz.sxryk.cn/gttbrucsvq.html

D. 数组 / 列表 / 集合
来源：http://hz.dashuyun.cn/gtdtrcljhk.html

================================================================================
来源：http://hz.gaohongyu789.top/gttwfrfctd.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtpsogiuze.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhaomingkeji.xyz/gtcrwszjyd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hywenlv.cn/gtdiqqqums.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.andypj.xyz/gtefdtguad.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hongshengwenyu.top/gtbkgponsb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ivvv.top/gtnrtwcdxu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shuidangran.top/gtiavmzopk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yueranfly.top/gthhhhzljk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.snrcjt.cn/gtwpvghkaw.html

[D02] 追加元素到末尾
来源：http://hz.chenjidiqi.icu/gtzlmwklkp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhijiandao.cn/gtyakrjnls.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangshuangyany.cn/gtwztjytch.html

JS:   arr.push(4);
来源：http://hz.jyoumei.cn/gtogabhkau.html

TS:   arr.push(4);
来源：http://hz.xuanzx.com/gtshykupdr.html

Java: list.add(4);
来源：http://hz.shanyushiyangkeji.top/gtzlwmfsgo.html

Go:   arr = append(arr, 4)
来源：http://hz.ydzc1.top/gttxkhxgxg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.c1oappe.top/gtmacxjjkd.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gttnvqogqw.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258.top/gtqxccjnxl.html

Py:   arr.insert(0, 0)
来源：http://hz.zhaomingkeji.xyz/gtepnetgnf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigfzy.top/gtfkhkjgrc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yueranfly.top/gtiyfbyvti.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yonumen.top/gttagialup.html

Java: list.add(0, 0);
来源：http://hz.guowangkeji.top/gtpcsbwopw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydjk.org.cn/gtqkcsyiud.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hfpthk.cn/gtmjrxhiax.html

C#:   list.Insert(0, 0);
来源：http://hz.tanke756.top/gtxgfcgfmm.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtlkcstzvi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.snrcjt.cn/gtcctvypyc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtmyybskwz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhiwuduotai.top/gtxpvzdlob.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangkeji.top/gtterjwaxk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhijiandao.cn/gtbouwouie.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.bjfxy.top/gtxevrzxkz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgufenzy.top/gtykhvuwbf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shangyingyoupin.top/gtivdhpezk.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtpphhaogp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtadozemtr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tianlin.xyz/gtfsmxjvjd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtnxfynbap.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hywenlv.cn/gtwqhgoeqa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtrjzqdhfb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258888.top/gtlctroqqh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtirzplpcc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.316326.xyz/gtaulzvkzr.html

[D06] 数组长度
来源：http://hz.guannengcc.top/gtllmotily.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gtkuejszqd.html

PHP:  count($arr);
来源：http://hz.zdqjudy.top/gtigfvteke.html

JS:   arr.length
来源：http://hz.pengpengdd.cyou/gtiboeocpa.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtxwkglszc.html

Java: list.size();
来源：http://hz.xziqi.cn/gtjjqcvvia.html

Go:   len(arr)
来源：http://hz.shuidangran.top/gtrwldhvso.html

Ruby: arr.length; arr.size
来源：http://hz.jqgfzy.top/gtbrxmrllw.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtzjwmsjtf.html

[D07] 切片 / 取子数组
来源：http://hz.dashuyun.cn/gtfsxbathb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtzxpschsx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghu66.top/gtnhuebnwp.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtzksfksij.html

TS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtpiscwxek.html

Java: list.subList(1, 4);
来源：http://hz.sxryk.cn/gtwfrpnttm.html

Go:   arr[1:4]
来源：http://hz.dashuyun.cn/gtnwqpgecb.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangtech.top/gtixgpqdvl.html

C#:   list.GetRange(1, 3);
来源：http://hz.feifeiyinyue.top/gtibchelww.html

[D08] 合并两个数组
来源：http://hz.shzxlz.cn/gtrcnretnq.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtssvspfra.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtixixxcnv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gttppnjnok.html

TS:   [...a, ...b];
来源：http://hz.hammf.cn/gtjnnsxapj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.52xcode.cn/gtpzurutoc.html

Go:   append(a, b...)
来源：http://hz.cheryme.top/gtcbmcnhgp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gtanljhqws.html

C#:   a.Concat(b).ToList()
来源：http://hz.gzhubu.top/gtbhuaonlc.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtzhmpyweg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtjscxzjkz.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtxglwwxox.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.snrcjt.cn/gtyussgukm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtmhygnghp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tanke756.top/gthnbtnzmz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jianghu66.top/gtyihdthia.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gttrfmyqxl.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gtelpuchkb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtptrdyqko.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jqgufenzy.top/gtsoagfidn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gthvngcsny.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtzjzqszhe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtblxreyjy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtjsypmosn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tanke756.top/gtuwrlkydf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.meibo888.top/gtvpgxkrqe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtqlbywlrd.html

[D11] 反转数组
来源：http://hz.yvedp.cn/gtvyznfiel.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenzaomai.com/gtraygelne.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gtkxjeiasf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.9152youxi.cn/gtkxsbkorf.html

TS:   [...arr].reverse();
来源：http://hz.zhixingplan.top/gttdavwhbb.html

Java: Collections.reverse(list);
来源：http://hz.bjfxy.top/gtivvzteae.html

Go:   slices.Reverse(arr)
来源：http://hz.tianlin.xyz/gtxeyrkdqi.html

Ruby: arr.reverse
来源：http://hz.sufxvd.cn/gtboimjopg.html

C#:   list.Reverse();
来源：http://hz.redwolf501.top/gtkacoapjj.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtnyagvkwk.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gtpjjsouzy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxinkj.top/gtaerlvhuo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtuvrrihyw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtbmyejlga.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtwekeeewd.html

Go:   slices.Index(arr, x)
来源：http://hz.hammf.cn/gtzhhadgwz.html

Ruby: arr.index(x)
来源：http://hz.c1oappe.top/gtgjftokzd.html

C#:   list.IndexOf(x);
来源：http://hz.ydzc1.top/gtegtwvwff.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yueranfly.top/gttfvdhbti.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nwbrower.top/gtrnrluyau.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangkeji.top/gtkspvfkkh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtztesiprm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtisaznmec.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenlongwang.top/gtklqflsss.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigufen.top/gtmqufkhrv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cashguo.top/gtwwyciegp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtcwxxfsgo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cheryme.top/gtgyiprdsh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtxokkiqlp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhixingplan.top/gtplafpbai.html

JS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtdabjfexs.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtkkeuvyyc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinyuanbaomall.cn/gtnzmtzcxh.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtdsjsjfku.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jiagoushi.top/gtwmdoavce.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtxpymamej.html

[D15] 去重
来源：http://hz.sysykeji.top/gtuvoyyori.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtvpupbkfx.html

PHP:  array_unique($arr);
来源：http://hz.cheryme.top/gtenxntspk.html

JS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtzxphtiqk.html

TS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtkfafyqgn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gtnuxlishh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgufenzy.top/gtrkmfoary.html

Ruby: arr.uniq
来源：http://hz.yj202588.top/gtieqohktk.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258.top/gteujigmrk.html

[D16] 求和与平均值
来源：http://hz.xziqi.cn/gtnxjbyson.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gtouutynze.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xziqi.cn/gtlhsrwjai.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtttwjdufq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtvhupztro.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258888.top/gthyqqwudf.html

Go:   // 手写循环累加
来源：http://hz.gzhubu.top/gtzpfmxrlg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yueranfly.top/gtvunoanrg.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtncycuupa.html

[D17] 最大值与最小值
来源：http://hz.yuxming.cn/gttarucqfr.html

Py:   max(arr);  min(arr)
来源：http://hz.zhijiandao.cn/gtxoprlfsc.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtemumqlki.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zycfv.cn/gtudfpwgvd.html

TS:   Math.max(...arr);
来源：http://hz.sysykeji.top/gthwwanspu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtqpwikfxh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigfzy.top/gtdzoblnns.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gtgmmoitbj.html

C#:   list.Max();  list.Min()
来源：http://hz.yj202588.top/gtusfihndk.html

[D18] 扁平化嵌套数组
来源：http://hz.jlsjyb.cn/gtzwsbxiwx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.mhx1999.top/gtlztcmhjd.html

PHP:  array_merge(...$nested);
来源：http://hz.mhx1999.top/gtifykwoww.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gtlzpemrof.html

TS:   nested.flat();
来源：http://hz.hfpthk.cn/gtqxnfkkmx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxinkj.top/gtoanzztfh.html

Go:   // 手写双层循环
来源：http://hz.iojbl.cn/gttceewynt.html

Ruby: nested.flatten
来源：http://hz.tianlin.xyz/gtfjnxgdiv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sysykeji.top/gtviagyhuv.html

[D19] 按字段分组
来源：http://hz.feifeiyinyue.top/gtjzptvfgt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydjk.org.cn/gttqqaofvg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.birdmap.top/gtzhnmakck.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigufen.top/gtkguggaqo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtuygrnppp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gtfkztpmhi.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gtowvkzvot.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuxming.cn/gtfbxgtgvr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shzxlz.cn/gteiqzojoj.html

[D20] 统计每个元素出现次数
来源：http://hz.iojbl.cn/gthbppexlx.html

Py:   Counter(arr)
来源：http://hz.bjfxy.top/gtswifiwlo.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtkjrnnqsi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtkxtobijq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtrsvuenjv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gogol.net.cn/gtdwvpdhvg.html

Go:   // 手写 map[T]int
来源：http://hz.yongpay.top/gtnungeujf.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtawpnksph.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gteungslck.html

[D21] 判断是否包含某元素
来源：http://hz.xingfuxueyuan.xyz/gtrljwpxcd.html

Py:   x in arr
来源：http://hz.cashguo.top/gtlrhetaiv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydzc1.top/gtrshrxsdv.html

JS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtsanzqoec.html

TS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtshmllimm.html

Java: list.contains(x)
来源：http://hz.yvedp.cn/gtkrfbrflj.html

Go:   slices.Contains(arr, x)
来源：http://hz.ehwqpu.com/gtklhkfsru.html

Ruby: arr.include?(x)
来源：http://hz.cdnleiting.top/gthxqzxulw.html

C#:   list.Contains(x)
来源：http://hz.ehwqpu.com/gtuyczefrm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.redwolf501.top/gtjfedfhax.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gtduphbpwp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuanzhike.top/gtolexchpy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnqzz.top/gtpxvdtlrl.html

TS:   [...arr];
来源：http://hz.ybcxt.top/gtgrcsoyzp.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtjdcymagz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.birdmap.top/gtdzxzscrb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cheryme.top/gtikihomtu.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtrzbpihjb.html


<!-- 参考信息 -->