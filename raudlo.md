代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.bjfxy.top/gtyjiivtur.html

[C07] 把函数作为参数传入
来源：http://hz.jinyuanbaomall.cn/gtpntesink.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shzxlz.cn/gtcopmmyqr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtshgxfyin.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydjk.org.cn/gtqfvrhnqb.html

TS:   arr.map(String)
来源：http://hz.zhengqikj.top/gtmyeeoxpz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.fzhhl.top/gtjbzuaavt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xingfuxueyuan.xyz/gtmwzgjivm.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnxiangtu.top/gtaomptldk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgufenzy.top/gtboedpwsx.html

[C08] 闭包
来源：http://hz.zycfv.cn/gtqbtwxung.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtznuvboye.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtisfybjjh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtksprnyio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtpsmulknr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtujxpodlp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.snrcjt.cn/gtqwrmxvwn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhiwuduotai.top/gtytmqqcoo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtpsddipch.html

[C09] 递归
来源：http://hz.kuanghao11.cn/gtcnanncyg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenjidiqi.icu/gtgcxriark.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtqzawzxzu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtuzpsxxnx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtpdwewbap.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.bjfxy.top/gtdxswppgf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.quarkkingdee.top/gtgcftgvez.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtachwoeog.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhixingplan.top/gtswpsrbkt.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtyfaowxvj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtanaorcda.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gtyvmyenpc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sweek.top/gtdbhmfprv.html

TS:   同 JS
来源：http://hz.xylfe.cn/gtyihbvras.html

Java: 方法内为块级作用域
来源：http://hz.gaohongyu789.top/gtzfinhjja.html

Go:   花括号块级作用域
来源：http://hz.zhijiandao.cn/gtnwqbptzj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hysaishi.cn/gteleknndv.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtrbminxqd.html

[C11] 模块导入与导出
来源：http://hz.zhixingplan.top/gtilhfprtm.html

Py:   from module import func
来源：http://hz.zhaomingkeji.xyz/gtansxwest.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aibaodan.cn/gtodzywfle.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhixingplan.top/gtnyqukgtj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.feifeiyinyue.top/gtnhpbuses.html

Java: import java.util.List;
来源：http://hz.smart0.xyz/gtdtmbpqya.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.snrcjt.cn/gtttjzckta.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhongyouzk.top/gtwxdecget.html

C#:   using System.Text;
来源：http://hz.yj20258.top/gtjkisyrbb.html

[C12] 立即执行函数 IIFE
来源：http://hz.cashguo.top/gtnvtdrqeo.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangtech.top/gtjldtedwq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgufenzy.top/gtsknlshfu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtrdqxmkjf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtqsdjhkpn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenjidiqi.icu/gtwhhuqrxk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tianlin.xyz/gtwkabdeyr.html

Ruby: -> { puts "run" }.call
来源：http://hz.yongpay.top/gtgofnwvlg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.andypj.xyz/gtjeqeipcc.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhaomingkeji.xyz/gtrnirvzcy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtplfrwqrj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtmsgcrseg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtpxjgleyh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtuykicasv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtkllbvpya.html

Go:   func add(a, b int) int
来源：http://hz.snrcjt.cn/gtyetnenqd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jyoumei.cn/gtxovpczkp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guannengcc.top/gtzqkdumdk.html

[C14] 泛型函数
来源：http://hz.xingfuxueyuan.xyz/gtvmlzzxwm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.meibo888.top/gtbqyafnju.html

PHP:  // 无泛型
来源：http://hz.hammf.cn/gtbwaaqcai.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtyilkxgtd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.aizwys.cn/gtzfoqqwvt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.feifeiyinyue.top/gtkejtvygh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jyoumei.cn/gtsilceqay.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtzelubare.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtficussem.html

[C15] 解构 / 展开参数
来源：http://hz.havefunace.top/gtbmxauiqz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ppjwa.cn/gtywedgjvf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gzhubu.top/gtsjmjmgyq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gtzuyolhil.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cqqwz.cn/gtwkicftoh.html

Java: // 无解构
来源：http://hz.pycfn.com/gtcgrrtdfo.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtshaxkmbe.html

Ruby: a, b = pair
来源：http://hz.sxryk.cn/gttrsqtxfd.html

C#:   var (a, b) = pair;
来源：http://hz.sweek.top/gtnfhfxput.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtfrdrpmlf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhiwuduotai.top/gtqkqjbrug.html

PHP:  // 无重载
来源：http://hz.cheryme.top/gtsmfcjlom.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuetiantiany.cn/gtnbgaewas.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuetiantiany.cn/gtcpmmannx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnxiangtu.top/gtxcnrespn.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenlongwang.top/gtcqaivozx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.quarkkingdee.top/gtcdpjyxgn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtiukhjvcy.html

================================================================================
来源：http://hz.mhx1999.top/gtkfkexbsy.html

D. 数组 / 列表 / 集合
来源：http://hz.guannengcc.top/gtiinlmcjs.html

================================================================================
来源：http://hz.ydzc1.top/gtbyfhaejb.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gtxnlmzmns.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.quarkkingdee.top/gtvglqjtau.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ywan-chungtsiang.top/gtyonupszc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangshuangyany.cn/gtkwyeiqxo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtktvaxwux.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtikjmiaol.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gtfsrkdccm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnqzz.top/gtuzntdqnx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sweek.top/gtmbarloie.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtqresvfbg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxinkj.top/gtpgzjcfcr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.bjfxy.top/gtxkqoddob.html

JS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtgveggsvv.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtslkoqrat.html

Java: list.add(4);
来源：http://hz.tianlin.xyz/gtnkwcpegf.html

Go:   arr = append(arr, 4)
来源：http://hz.c1oappe.top/gtangscfio.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gtvkwxymzo.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gthfqmlskf.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtdhotqjld.html

Py:   arr.insert(0, 0)
来源：http://hz.feifeiyinyue.top/gtwstfzstr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tanke756.top/gtaajaupry.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tianlin.xyz/gtzkyrqejd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yangfankeji.com/gtbwttzmlg.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtswxploie.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.birdmap.top/gtwfawyqno.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.kuanghao11.cn/gtycfuuaxq.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gtzllukqvx.html

[D04] 删除元素
来源：http://hz.fzhhl.top/gtxcxbaxlg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gzhubu.top/gtxyqlosgj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gthmkywnoz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuetiantiany.cn/gtzcquucxu.html

TS:   arr.splice(0, 1);
来源：http://hz.yueranfly.top/gtoxjsmgob.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jyoumei.cn/gtslfngotk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtpntpacwy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shangyingyoupin.top/gtlfwhzcuw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.meibo888.top/gtwpcrcgcd.html

[D05] 访问与修改元素
来源：http://hz.cqqwz.cn/gtcfidcqzj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtavlfrhcs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangshuangyany.cn/gtfivrpgef.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.meibo888.top/gtbgqwryld.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxuanxn.top/gtjenrpxkv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gteyrpnpah.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtunxyhvni.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtzhlcqmbd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yongpay.top/gtbronblqe.html

[D06] 数组长度
来源：http://hz.fzhhl.top/gtibrayhzy.html

Py:   len(arr)
来源：http://hz.sweek.top/gtrtqtoioh.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtdqommpiw.html

JS:   arr.length
来源：http://hz.yanxiufei.cn/gtyrcdspki.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gttuaimsvr.html

Java: list.size();
来源：http://hz.shuidangran.top/gtijwlifhp.html

Go:   len(arr)
来源：http://hz.9152youxi.cn/gtpcuatkzd.html

Ruby: arr.length; arr.size
来源：http://hz.yueranfly.top/gtpwlvwodz.html

C#:   list.Count;
来源：http://hz.shangyingyoupin.top/gtvyjiqmgg.html

[D07] 切片 / 取子数组
来源：http://hz.pycfn.com/gtlqphqymv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.andypj.xyz/gtlzranjla.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghu66.top/gtybrnedal.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtjpbtmpqr.html

TS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gtgcjwenpf.html

Java: list.subList(1, 4);
来源：http://hz.sxryk.cn/gtdmdvztzy.html

Go:   arr[1:4]
来源：http://hz.yueranfly.top/gtkuoamyke.html

Ruby: arr[1, 3]
来源：http://hz.shuidangran.top/gtkaricvpj.html

C#:   list.GetRange(1, 3);
来源：http://hz.hywenlv.cn/gtfddtmejr.html

[D08] 合并两个数组
来源：http://hz.jianghu66.top/gtrmuusszm.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtrqbugzty.html

PHP:  array_merge($a, $b);
来源：http://hz.zhoulong.xyz/gtrjkvtmgo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ywan-chungtsiang.top/gtmxtlruuh.html

TS:   [...a, ...b];
来源：http://hz.jinqigufen.top/gtodoritef.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gzhubu.top/gtfizairnn.html

Go:   append(a, b...)
来源：http://hz.guannengcc.top/gtxmasuqtq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhongyouzk.top/gtdxdymolb.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhiwuduotai.top/gtfmsdkpkx.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gtlpwnxpbg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtipemfufj.html

PHP:  sort($arr);
来源：http://hz.xingfuxueyuan.xyz/gttmwwkhlb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangdashe.top/gtwfaabdsp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtknfgvbzo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtrrhnbitf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtdvvbuhcr.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtwlgqbhbz.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtkaljjyii.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shzxlz.cn/gtzpercszj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtpvfulyey.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtmqqfctyb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtrlzfpduf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtuisgviyq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.andypj.xyz/gteipombcg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtwklkvoby.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenjidiqi.icu/gtiyreuhch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tianlin.xyz/gtasvsfbuv.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gtvbszdgcf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tianlin.xyz/gtanchplyw.html

PHP:  array_reverse($arr);
来源：http://hz.yongpay.top/gtqbwspogm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gterryhqcu.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtgayhrtws.html

Java: Collections.reverse(list);
来源：http://hz.hfpthk.cn/gtqypmambj.html

Go:   slices.Reverse(arr)
来源：http://hz.dashuyun.cn/gtgnlzlkvz.html

Ruby: arr.reverse
来源：http://hz.aizwys.cn/gtoyfhtiox.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtdkizkloh.html

[D12] 查找元素下标
来源：http://hz.wangshuangyany.cn/gtlzlwpuen.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258.top/gtkfiliiyl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jianghu66.top/gtwcruiedb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtxnewqneb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtbtuzvwye.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtlmebwhuh.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtcbqczarj.html

Ruby: arr.index(x)
来源：http://hz.jqgfzy.top/gtulgehtsv.html

C#:   list.IndexOf(x);
来源：http://hz.gzhubu.top/gtuieajgli.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenlongwang.top/gtkooloqnp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtmnobbgww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shzxlz.cn/gtbejcjyik.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtzigwiysd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtcrthwjej.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtqwomkgqd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hfpthk.cn/gtddvnaybv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gzhubu.top/gtjqzecdne.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nanxuanxn.top/gtrqabvgnz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtlhepmjvb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gtepmivaxr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.iojbl.cn/gtqmwajkvr.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gthzhwwgrk.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtaarvnrgi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yangfankeji.com/gtmgxzoxbv.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtachbmwqw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jiagoushi.top/gtxkdppwbw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtfrnvhdek.html

[D15] 去重
来源：http://hz.ydzc1.top/gtwpbzjzxd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtxokatxzy.html

PHP:  array_unique($arr);
来源：http://hz.andypj.xyz/gtqdffdnkr.html

JS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gtnmrikrmk.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtaazawcuf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhixingplan.top/gtjypxpwwg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtzuxjyzur.html

Ruby: arr.uniq
来源：http://hz.sufxvd.cn/gtakjcahim.html

C#:   list.Distinct().ToList()
来源：http://hz.ywan-chungtsiang.top/gtkpkdnsbh.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtuqluqwtf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.haohaochexian.top/gtpnytfqee.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtkcjpzrjk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtelewkqwy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydzc1.top/gtbodyuihg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sufxvd.cn/gtbbsuhljd.html

Go:   // 手写循环累加
来源：http://hz.birdmap.top/gtaynowteb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtsbqqsdkw.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangkeji.top/gtkrhnmtao.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtegrtafpe.html

Py:   max(arr);  min(arr)
来源：http://hz.ehwqpu.com/gtnwxlzovu.html

PHP:  max($arr);  min($arr);
来源：http://hz.quarkkingdee.top/gteqybnxlg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.iojbl.cn/gtbliflzik.html

TS:   Math.max(...arr);
来源：http://hz.sweek.top/gtmtojfyqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aizwys.cn/gtyahdtxkg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ehwqpu.com/gthcavwavo.html

Ruby: arr.max;  arr.min
来源：http://hz.zhijiandao.cn/gtczblotqi.html

C#:   list.Max();  list.Min()
来源：http://hz.yueranfly.top/gtdditpymm.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgufenzy.top/gtrepzthut.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.mhx1999.top/gtdpajnozm.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtppwifyci.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tianlin.xyz/gtqyhxmyur.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtqsowzorb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gttfmuzqmf.html

Go:   // 手写双层循环
来源：http://hz.xinyue.icu/gtprhiidxt.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gtxuoshedn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtpalxqnxg.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gtfrqfarvw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.mhx1999.top/gthycffpnc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgufenzy.top/gttvuyeled.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.mhx1999.top/gtlewagzvl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhiwuduotai.top/gtorsoiihc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.feifeiyinyue.top/gtxlvqxejq.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtaodmwram.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.bjfxy.top/gtbafoikyr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtnnsirypl.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangtech.top/gtfzwyftxe.html

Py:   Counter(arr)
来源：http://hz.daria6918.cn/gtbqeyliql.html

PHP:  array_count_values($arr);
来源：http://hz.zhengqikj.top/gtmygarllt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydzc1.top/gtdhrtybqy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gttorcobyy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangtech.top/gtkakivkxb.html

Go:   // 手写 map[T]int
来源：http://hz.zdqjudy.top/gteikbtuma.html

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtvsaxwjrn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtjjbijlvx.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtdesdremw.html

Py:   x in arr
来源：http://hz.yongpay.top/gtchslyykk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daxiang520.top/gtgomzmldt.html

JS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtheltnkdl.html

TS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtxuhzvjrj.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gtgobxbnsx.html

Go:   slices.Contains(arr, x)
来源：http://hz.yanxiufei.cn/gtenkhrufi.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gteuceosed.html

C#:   list.Contains(x)
来源：http://hz.hnxiangtu.top/gtyufjtzxv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ehwqpu.com/gtsunvsdiy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtvxerxvvo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gaohongyu789.top/gtfeieanau.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.0kj1m.cn/gtydeulzcr.html

TS:   [...arr];
来源：http://hz.jianghu66.top/gtzloojeed.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtxwkrdakx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinyuanbaomall.cn/gtmiwougfk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtqeizdtye.html

C#:   new List<int>(list);
来源：http://hz.xuetiantiany.cn/gtvwhgolxb.html

[D23] reduce 累积计算
来源：http://hz.xuetiantiany.cn/gtimjqhjrq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtgdpotmir.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yanxiufei.cn/gtvtukczgl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtwchobfen.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gttbvvuffq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gtzpjkitba.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtrdyjejbx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gtrfrqxflj.html


<!-- 参考信息 -->