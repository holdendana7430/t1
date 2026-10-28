代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.nanxinkj.top/gtddtjvnxs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtwxxyvrho.html

[C08] 闭包
来源：http://hz.gzhubu.top/gtxzrdfgks.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhoulong.xyz/gtqwkhxjxq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guannengcc.top/gtwunmutuv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtvrirmpcw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtdnbnmqlg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cheryme.top/gtltmqdqqw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gtxqjbvbay.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ybcxt.top/gthgdmuocl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtvvxpakox.html

[C09] 递归
来源：http://hz.svipenyu.cn/gtsduipteg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zycfv.cn/gtokoypozx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gtqfaksdfw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtzpfvzpze.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtevhgqnvy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258888.top/gtjgvyxcjh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtzenuxjbg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtqbzkvsny.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jlsjyb.cn/gtzmgtmrzc.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gtjibqhsnx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.wangdashe.top/gtntjlxnhh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gtgrlpgdxn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.kuanghao11.cn/gtlawrdzsg.html

TS:   同 JS
来源：http://hz.pycfn.com/gtxaskerkt.html

Java: 方法内为块级作用域
来源：http://hz.jlsjyb.cn/gtxqlhowwv.html

Go:   花括号块级作用域
来源：http://hz.nanxinkj.top/gtunepzqij.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xziqi.cn/gtuplnbzbz.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtvkzvvaml.html

[C11] 模块导入与导出
来源：http://hz.feifeiyinyue.top/gtycseqazg.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gtbxssfdej.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtctbciiec.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtrepqjjdy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.havefunace.top/gtrzqqhqaw.html

Java: import java.util.List;
来源：http://hz.hywenlv.cn/gtwfhzvytu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.havefunace.top/gtyfvbhysk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jianghu66.top/gtagxcztgu.html

C#:   using System.Text;
来源：http://hz.hywenlv.cn/gtyinlwxav.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhongyouzk.top/gtzrakgmsw.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gtiicqbucw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhengqikj.top/gtbvoonfbj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtbwvlgpaq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gtuvstkdsh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtlpijmhbb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhijiandao.cn/gthnnrsumu.html

Ruby: -> { puts "run" }.call
来源：http://hz.redwolf501.top/gtykdhkaqj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gaohongyu789.top/gtawuzwhmp.html

[C13] 类型声明 / 类型注解
来源：http://hz.shuidangran.top/gtehznghjc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ppjwa.cn/gtxmvhsuxp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xinyue.icu/gtvcufgfkt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.andypj.xyz/gtjoiwbtwn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtjmorgxfk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtojcmwefc.html

Go:   func add(a, b int) int
来源：http://hz.gaohongyu789.top/gtstjmvjiv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtjnaigics.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ivvv.top/gthejubjho.html

[C14] 泛型函数
来源：http://hz.hysaishi.cn/gtrdcqcefe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhiwuduotai.top/gtiycqhxgk.html

PHP:  // 无泛型
来源：http://hz.tianlin.xyz/gtitloaert.html

JS:   // 无泛型
来源：http://hz.cheryme.top/gtzkdubruj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtivoxamwf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuetiantiany.cn/gtoatfswbf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnqzz.top/gtqzwthobf.html

Ruby: # 无泛型
来源：http://hz.yuxming.cn/gtzygczavk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gtnjlstyus.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigufen.top/gtqvorhywl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtghdapalf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.smart0.xyz/gtowmuokhr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtxtpzvmte.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tanke756.top/gtixqaalgk.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gtyiewzvxm.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gtzfdigxfo.html

Ruby: a, b = pair
来源：http://hz.kuanghao11.cn/gtjbtddrvx.html

C#:   var (a, b) = pair;
来源：http://hz.zhijiandao.cn/gtrpfsurgf.html

[C16] 函数 / 方法重载
来源：http://hz.jqgfzy.top/gtpbnfrmlm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.9152youxi.cn/gtafflojzf.html

PHP:  // 无重载
来源：http://hz.zhiwuduotai.top/gtxbzqumqx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ehwqpu.com/gttaeqaolp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtkvyeeewn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtdpsrqzap.html

Go:   // 无重载：用不同函数名
来源：http://hz.cqqwz.cn/gtggdssjew.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fengsongda.top/gtvtamhipb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gtccuvmflw.html

================================================================================
来源：http://hz.yvedp.cn/gtntimfygg.html

D. 数组 / 列表 / 集合
来源：http://hz.daria6918.cn/gtkhthsvzi.html

================================================================================
来源：http://hz.redwolf501.top/gtafilcgal.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtvycfjjfc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtpmufxbnq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cashguo.top/gtwqnmnsja.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shuidangran.top/gtjfttbkbd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hammf.cn/gtlnczsioz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yonumen.top/gtccvwbges.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtctgbcsdo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shzxlz.cn/gtscytcour.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gthuuxiinr.html

[D02] 追加元素到末尾
来源：http://hz.0kj1m.cn/gteelyoenc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuanzhike.top/gtcxchfkvx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtongytezz.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtaopkcrkk.html

TS:   arr.push(4);
来源：http://hz.ivvv.top/gtqrprykmk.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtosybouvg.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtdjpnksed.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daria6918.cn/gttdlscyxq.html

C#:   list.Add(4);
来源：http://hz.zhoulong.xyz/gtnvfnecrl.html

[D03] 在指定位置插入元素
来源：http://hz.haohaochexian.top/gtyvivfuxk.html

Py:   arr.insert(0, 0)
来源：http://hz.yueranfly.top/gtmbqaxgbf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtjitxwcsd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtllfypwnk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hywenlv.cn/gtuiomhdrp.html

Java: list.add(0, 0);
来源：http://hz.hnxiangtu.top/gtjgijmikg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuanzhike.top/gtwipohvyg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj202588.top/gtajycasko.html

C#:   list.Insert(0, 0);
来源：http://hz.svipenyu.cn/gtjkvvefmt.html

[D04] 删除元素
来源：http://hz.gaohongyu789.top/gtftdehlxg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hfpthk.cn/gtlvvuwucn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gttgidifbe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hywenlv.cn/gtqtauspke.html

TS:   arr.splice(0, 1);
来源：http://hz.aizwys.cn/gtbhdjnhrw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangshuangyany.cn/gtvlascxkm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuanzx.com/gthfhznwmz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgfzy.top/gtxnyicibt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yueranfly.top/gtwnzqrmki.html

[D05] 访问与修改元素
来源：http://hz.9152youxi.cn/gttoaezusu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtbgsseojm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shzxlz.cn/gtiiauwypg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxinkj.top/gtruitvddi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenlongwang.top/gtmcqzqeva.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtrwrgmjqm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtthoownak.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtkrovgflx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258.top/gtuhkyfpyb.html

[D06] 数组长度
来源：http://hz.meibo888.top/gttqvgwogp.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtrnjrchjt.html

PHP:  count($arr);
来源：http://hz.hywenlv.cn/gtjolqzwoz.html

JS:   arr.length
来源：http://hz.ehwqpu.com/gtxlnpnhcn.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtcjwzmvhr.html

Java: list.size();
来源：http://hz.jyoumei.cn/gturnsobop.html

Go:   len(arr)
来源：http://hz.gotoacloud.top/gtrcgxcvfe.html

Ruby: arr.length; arr.size
来源：http://hz.cqqwz.cn/gtykpllykg.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtxdmmovcf.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtmrjavvmd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtcstcthpl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxuanxn.top/gtqdrixvjz.html

JS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtztxgoxxv.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtmcxntbej.html

Java: list.subList(1, 4);
来源：http://hz.daxiang520.top/gthetfvven.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gtgycpqomw.html

Ruby: arr[1, 3]
来源：http://hz.ydzc1.top/gtmhifdljv.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtfshakrpr.html

[D08] 合并两个数组
来源：http://hz.pycfn.com/gtxjtydoxx.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gthxqwflio.html

PHP:  array_merge($a, $b);
来源：http://hz.yj202588.top/gtwzrecuoc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xinyue.icu/gtixadgyrz.html

TS:   [...a, ...b];
来源：http://hz.zycfv.cn/gtcauugrdr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.iojbl.cn/gtvhqilecw.html

Go:   append(a, b...)
来源：http://hz.jiagoushi.top/gtvtuwkxcl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yvedp.cn/gttmtvttsf.html

C#:   a.Concat(b).ToList()
来源：http://hz.yanxiufei.cn/gtixicwcdq.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gtxssjwgyk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gtzneccrcr.html

PHP:  sort($arr);
来源：http://hz.yueranfly.top/gtjibigayf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.redwolf501.top/gtgfmxggno.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhoulong.xyz/gthbldsegj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtwiusulyd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtzefirdoy.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtiirsgjly.html

C#:   list.Sort();
来源：http://hz.hysaishi.cn/gtqytrmaej.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aizwys.cn/gtntoigupc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhoulong.xyz/gtzgpjishj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gthqrjwkoy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gtabhvvgzv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtflukshfr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daria6918.cn/gtgvcybirx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gtsytdaczy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hammf.cn/gtahjpwxkd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yueranfly.top/gtnbuxqier.html

[D11] 反转数组
来源：http://hz.shuidangran.top/gtxkibcrdx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangdashe.top/gtcpxmpowu.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gtjtlgkcfb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jqgufenzy.top/gtjytgafgu.html

TS:   [...arr].reverse();
来源：http://hz.zhongyouzk.top/gttaniflyy.html

Java: Collections.reverse(list);
来源：http://hz.shangyingyoupin.top/gtjuakhlmw.html

Go:   slices.Reverse(arr)
来源：http://hz.hysaishi.cn/gtdrsburzm.html

Ruby: arr.reverse
来源：http://hz.tianlin.xyz/gteyswdhpc.html

C#:   list.Reverse();
来源：http://hz.cashguo.top/gtmkywyrys.html

[D12] 查找元素下标
来源：http://hz.hfpthk.cn/gtsqobownm.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gtjlotuwxc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.0kj1m.cn/gtydshdgui.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtsveqxtqd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.haohaochexian.top/gtavfywigm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.feifeiyinyue.top/gttyvgwdua.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtlvzuqgwu.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtmoewilse.html

C#:   list.IndexOf(x);
来源：http://hz.svipenyu.cn/gtrffwbipn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shuidangran.top/gtjvzlqwbn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtvzmcuqzs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ybcxt.top/gtvwlsybih.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gtlahtrvsv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtlybpqzbe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigfzy.top/gtcvxnhipk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jiagoushi.top/gtcxybllds.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.kuanghao11.cn/gtndbkqbxe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuxming.cn/gtvkttmsnh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ivvv.top/gtnvstkwzw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tian-w.cn/gtacmdzqpn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtvqvhcznv.html

JS:   arr.map(x => x * 2)
来源：http://hz.tian-w.cn/gtvohwtopr.html

TS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtajifbhhy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtesvbbeag.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtgdtfjofl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtalmjllun.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gtwiarntll.html

[D15] 去重
来源：http://hz.yuxming.cn/gtjsyvxkzk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtxvihznvh.html

PHP:  array_unique($arr);
来源：http://hz.zhixingplan.top/gtspbnebcy.html

JS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtaosfnvis.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtjilzvoga.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtoeuebbzm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtsznevlpj.html

Ruby: arr.uniq
来源：http://hz.hnxiangtu.top/gtwgtlhhve.html

C#:   list.Distinct().ToList()
来源：http://hz.smart0.xyz/gtjxqfuobk.html

[D16] 求和与平均值
来源：http://hz.iojbl.cn/gtirtlwmna.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gogol.net.cn/gtacnaitnb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinghuilouyu.cn/gtvcdlrcum.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gttaghukmw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtibahhiav.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtppdvsgkb.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangtech.top/gtqrrawbay.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gtukoshqzv.html

C#:   list.Sum();  list.Average()
来源：http://hz.aibaodan.cn/gtiwtfhfgi.html

[D17] 最大值与最小值
来源：http://hz.iojbl.cn/gtmmiodljz.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gtyntiglhz.html

PHP:  max($arr);  min($arr);
来源：http://hz.9152youxi.cn/gteypgfxdc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtzkbyoaam.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gthzaglvsp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhiwuduotai.top/gtslcuurhf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhiwuduotai.top/gtajokvqth.html

Ruby: arr.max;  arr.min
来源：http://hz.c1oappe.top/gturiftflf.html

C#:   list.Max();  list.Min()
来源：http://hz.xuanzx.com/gtghlmzmba.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtcohxvjun.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cheryme.top/gtkfetdihz.html

PHP:  array_merge(...$nested);
来源：http://hz.svipenyu.cn/gthfxtkcsx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhengqikj.top/gtcfrcrlzo.html

TS:   nested.flat();
来源：http://hz.cucudq.cn/gtuifeamtt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daria6918.cn/gtyoveraqc.html

Go:   // 手写双层循环
来源：http://hz.cdnleiting.top/gtgdkrkarx.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gtbeboipkj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtapxznrhy.html

[D19] 按字段分组
来源：http://hz.ppjwa.cn/gtphuxwjmk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258.top/gtbfgklvsy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtlkpedvsv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtqphoezoc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtdiitsapf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guannengcc.top/gtpthxzbiq.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtslznrtna.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yanxiufei.cn/gtzwspuhic.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sufxvd.cn/gthhmphxhm.html

[D20] 统计每个元素出现次数
来源：http://hz.haohaochexian.top/gtkowzrnmj.html

Py:   Counter(arr)
来源：http://hz.hywenlv.cn/gtfqajmggm.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigfzy.top/gtaaajffco.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtuxhqogej.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtwzzigyul.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guannengcc.top/gtuvpigxoi.html

Go:   // 手写 map[T]int
来源：http://hz.ppjwa.cn/gtsrluvyne.html

Ruby: arr.tally
来源：http://hz.ivvv.top/gtfqzovxqj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gtsuozmdxp.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtdgxdsevo.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gtqaukvkdq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhoulong.xyz/gtqbynzbvk.html

JS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtmbkolont.html

TS:   arr.includes(x)
来源：http://hz.316326.xyz/gtijsawocg.html

Java: list.contains(x)
来源：http://hz.pengpengdd.cyou/gtymjwhiop.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgfzy.top/gtlnwdvvyl.html

Ruby: arr.include?(x)
来源：http://hz.guannengcc.top/gtnkyrxqfr.html

C#:   list.Contains(x)
来源：http://hz.tanke756.top/gtnwfrboyj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guannengcc.top/gtodrrunar.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xuanzx.com/gtgmsxqdbi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtcrovsgix.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aibaodan.cn/gtdmdmxeml.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtzrydsiww.html

Java: new ArrayList<>(list);
来源：http://hz.havefunace.top/gtkmwzfiuc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj202588.top/gtqzldeyrj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gtisfjpqjj.html

C#:   new List<int>(list);
来源：http://hz.yj202588.top/gtfyxrcrwl.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtcxeikiwk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtsczxtrzs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daxiang520.top/gtletxqgki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuanzx.com/gticecpqyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtxofxrxvu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangtech.top/gttibfusga.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtakwqsddb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtnrssliqg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhijiandao.cn/gtppusniju.html

[D24] 字典 / Map 基本操作
来源：http://hz.feifeiyinyue.top/gtgrwvnfpj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xziqi.cn/gtezndbpdk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.haohaochexian.top/gtrugidvwt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.iojbl.cn/gttnwvpnnb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhiwuduotai.top/gtllnizxty.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnqzz.top/gtozyilxvg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cashguo.top/gtpmatupxo.html


<!-- 参考信息 -->