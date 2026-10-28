代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtxmvfxsji.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aibaodan.cn/gtxblttwbs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ybcxt.top/gtmzuclqyt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tianlin.xyz/gtxhfvsknx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.bjfxy.top/gtpokrqusv.html

[C07] 把函数作为参数传入
来源：http://hz.tanke756.top/gtzmplhwen.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinqigfzy.top/gtqlteiohd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jqgfzy.top/gtydvfqsat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tanke756.top/gtwcbvshpw.html

TS:   arr.map(String)
来源：http://hz.yueranfly.top/gtrrczvbwr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cucudq.cn/gtkqneqzgv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gaohongyu789.top/gtbarwdzum.html

Ruby: arr.map(&:upcase)
来源：http://hz.pengpengdd.cyou/gtcjpfwrqv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinghuilouyu.cn/gtwvncfbmh.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtqyxbosoc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtjewodkbs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtsdqxmexi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtuzxifozy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtirazdxbb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.mhx1999.top/gtcnetaben.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yanxiufei.cn/gttzwpgbni.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ywan-chungtsiang.top/gtdkkytnss.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtezrfywqz.html

[C09] 递归
来源：http://hz.fzhhl.top/gtxeknolsj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuxming.cn/gtezrdtfpf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ywan-chungtsiang.top/gtfcdzqeag.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtpyoetfkj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.svipenyu.cn/gtegyjrjyd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigfzy.top/gtkucldqyi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guowangkeji.top/gtayoogoct.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cdnleiting.top/gtwwmanjki.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jlsjyb.cn/gtqnybgxrf.html

[C10] 变量作用域
来源：http://hz.kuanghao11.cn/gtncrrctsm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hysaishi.cn/gtndrspqnf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gzhubu.top/gtsfoaimpp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yvedp.cn/gtuvrvzlso.html

TS:   同 JS
来源：http://hz.c1oappe.top/gtbpxxrbsf.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtjvlbglwm.html

Go:   花括号块级作用域
来源：http://hz.jianghu66.top/gtddnmdskp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.andypj.xyz/gthmlvkxrv.html

C#:   块级作用域
来源：http://hz.quarkkingdee.top/gtxbinaktu.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtronqbhjj.html

Py:   from module import func
来源：http://hz.mhx1999.top/gthxyveiph.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenzaomai.com/gtkktkhtal.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gaohongyu789.top/gtlihqjkvk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenjidiqi.icu/gtenbbbsbp.html

Java: import java.util.List;
来源：http://hz.gogol.net.cn/gttzeblyxt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gzhubu.top/gtyrrukeqn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj202588.top/gtkxxeviqq.html

C#:   using System.Text;
来源：http://hz.hnqzz.top/gtkyyrlann.html

[C12] 立即执行函数 IIFE
来源：http://hz.cucudq.cn/gthzipopdp.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gthjyziwhl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gthaqnklqb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gteqozchkn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtrqxvvwey.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtjaegxrff.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fengsongda.top/gtygodbiwm.html

Ruby: -> { puts "run" }.call
来源：http://hz.hfpthk.cn/gtnoznnoua.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hammf.cn/gtsyztzygt.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtzfnvdvwl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dashuyun.cn/gtgepqpkyz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtfpvmrakl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtxziewuvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtjsggferf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtjzdndxhn.html

Go:   func add(a, b int) int
来源：http://hz.meibo888.top/gtbtnalizs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuanzhike.top/gtphqpgwyi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.havefunace.top/gteggmexah.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtlefskizt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sysykeji.top/gtysgxigop.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtoxvoucxw.html

JS:   // 无泛型
来源：http://hz.nanxinkj.top/gtexbxqfbo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydzc1.top/gttqbioxoc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtpxhgdljl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtdxelhaae.html

Ruby: # 无泛型
来源：http://hz.cashguo.top/gtlihypkjg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cheryme.top/gtkxvegotm.html

[C15] 解构 / 展开参数
来源：http://hz.xinyue.icu/gtdtushylc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aibaodan.cn/gtrhlwxmes.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgfzy.top/gtfmaycdre.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtuzzhymcn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aizwys.cn/gtfokfxgdo.html

Java: // 无解构
来源：http://hz.hysaishi.cn/gtvxwfiydp.html

Go:   // 无解构
来源：http://hz.yuanzhike.top/gtvxusvjbt.html

Ruby: a, b = pair
来源：http://hz.aizwys.cn/gtjroobmyb.html

C#:   var (a, b) = pair;
来源：http://hz.ybcxt.top/gtppeehbqh.html

[C16] 函数 / 方法重载
来源：http://hz.shangyingyoupin.top/gtrzxvxjhp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.c1oappe.top/gtbjaeelbf.html

PHP:  // 无重载
来源：http://hz.fzhhl.top/gtqydnqiui.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtodircxql.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258.top/gtzhhzqcgm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.feifeiyinyue.top/gtejicpgjb.html

Go:   // 无重载：用不同函数名
来源：http://hz.hysaishi.cn/gthmhsaorg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.redwolf501.top/gthadjwohm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fengsongda.top/gtasavjzke.html

================================================================================
来源：http://hz.yvedp.cn/gtkxetfarz.html

D. 数组 / 列表 / 集合
来源：http://hz.aizwys.cn/gtincwxfxv.html

================================================================================
来源：http://hz.andypj.xyz/gtuoiitugm.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258.top/gtuqxwkekj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.pengpengdd.cyou/gtneyskfjl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.andypj.xyz/gtdbbbsovm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.andypj.xyz/gtgapkhtbz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.haohaochexian.top/gtmifchink.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nwbrower.top/gtxtqfhohn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gtigmgzvmr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gtvfzlcogf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yangfankeji.com/gtpibrsccg.html

[D02] 追加元素到末尾
来源：http://hz.gotoacloud.top/gtpyeduieu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gthaspllum.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.9152youxi.cn/gtwfsbjqij.html

JS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtyqidwvyb.html

TS:   arr.push(4);
来源：http://hz.316326.xyz/gtswcvmyxk.html

Java: list.add(4);
来源：http://hz.kuanghao11.cn/gtcylvwtwu.html

Go:   arr = append(arr, 4)
来源：http://hz.aizwys.cn/gtoixnygvz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtwzjyajuc.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtdxkgdmmn.html

[D03] 在指定位置插入元素
来源：http://hz.birdmap.top/gtvebjjowh.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgufenzy.top/gtrhybqqyc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.havefunace.top/gtglzzhqzl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtlyutrbej.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.iojbl.cn/gtawtdcrhh.html

Java: list.add(0, 0);
来源：http://hz.hnxiangtu.top/gttzsyzrdv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtvyuhzszn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zycfv.cn/gteoeiqrid.html

C#:   list.Insert(0, 0);
来源：http://hz.andypj.xyz/gtqrsuamrz.html

[D04] 删除元素
来源：http://hz.shuidangran.top/gtdpifcrbo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.redwolf501.top/gtfblguitt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtikqamizu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenzaomai.com/gtpiraajpd.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtxmlfxxwx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.c1oappe.top/gtxgeewjmm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhengqikj.top/gtlzqgkmuh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhoulong.xyz/gthpsekgqv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.haohaochexian.top/gtgwjodcem.html

[D05] 访问与修改元素
来源：http://hz.sysykeji.top/gtpvlyocwg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gttvodxnik.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shzxlz.cn/gtvsqfjvos.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.316326.xyz/gtglrdfpuo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258888.top/gtcwsasgca.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shuidangran.top/gtymuhfuhk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xinyue.icu/gtgpvcfqof.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtijirdmbg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shzxlz.cn/gtqhrwvhla.html

[D06] 数组长度
来源：http://hz.snrcjt.cn/gtduccstts.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtaaldyozb.html

PHP:  count($arr);
来源：http://hz.sufxvd.cn/gtifnckjos.html

JS:   arr.length
来源：http://hz.hongshengwenyu.top/gtjktvrjvk.html

TS:   arr.length
来源：http://hz.zhoulong.xyz/gtknkshfoe.html

Java: list.size();
来源：http://hz.meibo888.top/gtspkuzhgg.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtfnvlpppz.html

Ruby: arr.length; arr.size
来源：http://hz.xingfuxueyuan.xyz/gtrokbsgmv.html

C#:   list.Count;
来源：http://hz.316326.xyz/gtpjinkdpf.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gtsjdyeusg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dashuyun.cn/gtbrnrgewq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtypniwmmr.html

JS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtwkyhsxtv.html

TS:   arr.slice(1, 4);
来源：http://hz.xinyue.icu/gtjmtquybm.html

Java: list.subList(1, 4);
来源：http://hz.bjfxy.top/gttdlyqgfd.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gtxtbridwm.html

Ruby: arr[1, 3]
来源：http://hz.bjfxy.top/gtduyrwjng.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtunapkyzz.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gtncnqqxqa.html

Py:   a + b;  a.extend(b)
来源：http://hz.hongshengwenyu.top/gtiuermkcm.html

PHP:  array_merge($a, $b);
来源：http://hz.shangyingyoupin.top/gtakabrmrw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zdqjudy.top/gtwaydhctd.html

TS:   [...a, ...b];
来源：http://hz.jinghuilouyu.cn/gtglydtris.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtjwxsvtnx.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gtivaemsiy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sufxvd.cn/gtxiurlrzn.html

C#:   a.Concat(b).ToList()
来源：http://hz.iojbl.cn/gtmszhfnyf.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtfvcvodtn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtrdjgjhcs.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtxhexwawm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gtnrwteqoo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtolapdlgj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangshuangyany.cn/gtarddohko.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gteyhthxzo.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtarxkwxdq.html

C#:   list.Sort();
来源：http://hz.kuanghao11.cn/gtjjlhgyaa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aibaodan.cn/gtvkjkvbjf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnxiangtu.top/gtcwcijuxv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ivvv.top/gtrhclkbgb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtwuffwzmi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtkggkkgns.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtskmrotbv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gtwbhlbztr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtlwbmdwha.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.havefunace.top/gtfoleyjsk.html

[D11] 反转数组
来源：http://hz.jyoumei.cn/gtjdzclngy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtijbvgegd.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gtuhdhlpnk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhijiandao.cn/gtqhuvfhng.html

TS:   [...arr].reverse();
来源：http://hz.ppjwa.cn/gtfechrekj.html

Java: Collections.reverse(list);
来源：http://hz.hywenlv.cn/gtjglsjotr.html

Go:   slices.Reverse(arr)
来源：http://hz.tianlin.xyz/gtbglnsiyy.html

Ruby: arr.reverse
来源：http://hz.chenlongwang.top/gtcvwpxawi.html

C#:   list.Reverse();
来源：http://hz.shzxlz.cn/gtsaspoqly.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtjklbkyfh.html

Py:   arr.index(x);  x in arr
来源：http://hz.ybcxt.top/gtpjkvtukk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtjhdfulzt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtogylespw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtzuaxfsws.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tian-w.cn/gtxewufnix.html

Go:   slices.Index(arr, x)
来源：http://hz.xuetiantiany.cn/gtolxhwxwf.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gthmiocdsq.html

C#:   list.IndexOf(x);
来源：http://hz.gogol.net.cn/gtjyywosru.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gtnhihyxvx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gaohongyu789.top/gtkxghdrgb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.iojbl.cn/gtxeekjurs.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtxveklilp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtxpihttvl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangkeji.top/gtjrszopec.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cheryme.top/gtgeurdohm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.kuanghao11.cn/gttssuzvoq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hfpthk.cn/gtcjflasca.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtpcntqosp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtsokupugl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gtyjtsflwb.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtytfqrfzn.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtysypfjoq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.smart0.xyz/gttywyahri.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtktvecvej.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtfiuokinc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnqzz.top/gtjvgtrqgv.html

[D15] 去重
来源：http://hz.jinqigufen.top/gtweeepqpi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtbjcrpkmj.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtxtftlchl.html

JS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtrklkxytm.html

TS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtzeafplkx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gttrddjrpj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hysaishi.cn/gtdtneyuly.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtlipaggel.html

C#:   list.Distinct().ToList()
来源：http://hz.zhengqikj.top/gtkhqzbhnn.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gtzqpyuyun.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.316326.xyz/gtmapkqcdq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gtxmjfmlfq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtudobbpdt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtqjwbnasd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtlyktzsac.html

Go:   // 手写循环累加
来源：http://hz.redwolf501.top/gtspfvacyi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gtkrzbacul.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtyfakhkxp.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtwvebwrud.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtgseetddz.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gtccomqczj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gtugeeesde.html

TS:   Math.max(...arr);
来源：http://hz.smart0.xyz/gtxxllbcfj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtnrbfppsu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cqqwz.cn/gtixmnymwy.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangtech.top/gthraoxeue.html

C#:   list.Max();  list.Min()
来源：http://hz.yvedp.cn/gtzoruzpyk.html

[D18] 扁平化嵌套数组
来源：http://hz.ywan-chungtsiang.top/gtwqrafbjp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hammf.cn/gtjsvlpwgf.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtegvbiocn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gthbzxssfd.html

TS:   nested.flat();
来源：http://hz.ehwqpu.com/gtgcpybvzy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gotoacloud.top/gtjmhypafa.html

Go:   // 手写双层循环
来源：http://hz.sufxvd.cn/gtpsdlygtm.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gtasbsnzgn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtitasnlpx.html

[D19] 按字段分组
来源：http://hz.gotoacloud.top/gtczzpfvhv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cashguo.top/gtvxjpiqzb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnqzz.top/gthjiplpgu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hammf.cn/gtvsjipzwm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gtohspwnhj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sxryk.cn/gtyuqorrfi.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtglbgiaoe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuanzhike.top/gtkqmlhpso.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.redwolf501.top/gtxshfcxsb.html

[D20] 统计每个元素出现次数
来源：http://hz.birdmap.top/gtxpxtjxlh.html

Py:   Counter(arr)
来源：http://hz.tanke756.top/gtckqikgix.html

PHP:  array_count_values($arr);
来源：http://hz.birdmap.top/gtgptjughm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtgmuzqpuc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtikdljvkp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.smart0.xyz/gtmyftyrwa.html

Go:   // 手写 map[T]int
来源：http://hz.dashuyun.cn/gtmkilbdng.html

Ruby: arr.tally
来源：http://hz.cucudq.cn/gtvcdliesh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtepyrenud.html

[D21] 判断是否包含某元素
来源：http://hz.jlsjyb.cn/gtbisudvue.html

Py:   x in arr
来源：http://hz.nanxuanxn.top/gtqsrmobuj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gthetrvqbc.html

JS:   arr.includes(x)
来源：http://hz.c1oappe.top/gteqzckime.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtsovzgyaw.html

Java: list.contains(x)
来源：http://hz.yj20258888.top/gtjhhjtnpv.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtvuwyqthu.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtsgrmraon.html

C#:   list.Contains(x)
来源：http://hz.52xcode.cn/gtjvqtnbhc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtalxomftz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinghuilouyu.cn/gttvhyxcsw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangshuangyany.cn/gtucharjdz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xziqi.cn/gtnqupidzc.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtpivdomoh.html

Java: new ArrayList<>(list);
来源：http://hz.yuxming.cn/gtvcumikux.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.svipenyu.cn/gtzrhulnjt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhaomingkeji.xyz/gtvqqmlcko.html

C#:   new List<int>(list);
来源：http://hz.gaohongyu789.top/gtdfstidxq.html

[D23] reduce 累积计算
来源：http://hz.jinqigufen.top/gtptatowet.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gtuquytymm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhiwuduotai.top/gtjmdtmmuk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtzasualec.html


<!-- 参考信息 -->