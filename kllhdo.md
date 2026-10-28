代发 wailian999

[C10] 变量作用域
来源：http://hz.xingfuxueyuan.xyz/gtwootnhjd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ywan-chungtsiang.top/gtxtbimflg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yueranfly.top/gtjsympqjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtbiqrhyvq.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtnkmixioh.html

Java: 方法内为块级作用域
来源：http://hz.vqdsnc.cn/gtrdlbmwlx.html

Go:   花括号块级作用域
来源：http://hz.smart0.xyz/gtexqeqvjq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gthbrvievw.html

C#:   块级作用域
来源：http://hz.xylfe.cn/gtjlntxsji.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtjjlymzcs.html

Py:   from module import func
来源：http://hz.yuanzhike.top/gtvutiklfq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangshuangyany.cn/gtodtqcyub.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zycfv.cn/gtmrrgjoir.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhengqikj.top/gtizryfsuk.html

Java: import java.util.List;
来源：http://hz.hnqzz.top/gtooeukscs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258.top/gtypxzoiea.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sweek.top/gtyqmgullr.html

C#:   using System.Text;
来源：http://hz.ehwqpu.com/gtombfczzh.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhijiandao.cn/gtzqscllpp.html

Py:   (lambda: print("run"))()
来源：http://hz.guannengcc.top/gtfjaeuays.html

PHP:  (function () { echo "run"; })();
来源：http://hz.havefunace.top/gtugxeokvi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gtrwfcnoov.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shzxlz.cn/gtgnwtlamm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nwbrower.top/gtqplzfnvk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tianlin.xyz/gtvwyjahgc.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtenvksvnx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.iojbl.cn/gtvncfeuft.html

[C13] 类型声明 / 类型注解
来源：http://hz.jianghu66.top/gtaujwfhcz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtlwduhvkf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gttqxzvgxe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cdnleiting.top/gtygfvftpk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gtxweogfdb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gttfivoddy.html

Go:   func add(a, b int) int
来源：http://hz.316326.xyz/gtswhwbasx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.9152youxi.cn/gtnmfdrtph.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgfzy.top/gtxloycbbk.html

[C14] 泛型函数
来源：http://hz.pengpengdd.cyou/gtjxxzkcyc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gtrqskrgmb.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtxfpbqzip.html

JS:   // 无泛型
来源：http://hz.snrcjt.cn/gthpettsyl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gtkpkqmikj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.snrcjt.cn/gttdaueydk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenzaomai.com/gthmlanrpr.html

Ruby: # 无泛型
来源：http://hz.zycfv.cn/gththumykt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258.top/gttopnccxi.html

[C15] 解构 / 展开参数
来源：http://hz.cashguo.top/gtjxdpyvzz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cdnleiting.top/gtrqkftuvr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.redwolf501.top/gtstmhjduh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtsmygnffz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gttgsvpmuy.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gtoduseynv.html

Go:   // 无解构
来源：http://hz.jqgufenzy.top/gtylyhgcgs.html

Ruby: a, b = pair
来源：http://hz.feifeiyinyue.top/gtpvkqvxtf.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gtezmxaodd.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtetoihhiq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.bjfxy.top/gtahpkywsm.html

PHP:  // 无重载
来源：http://hz.tian-w.cn/gthfhruyku.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cashguo.top/gtslcwkujw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.havefunace.top/gtmhpwtbks.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangshuangyany.cn/gtcuowsmjl.html

Go:   // 无重载：用不同函数名
来源：http://hz.xylfe.cn/gtgkawjhpz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtfohyhcqt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ybcxt.top/gttkndouwm.html

================================================================================
来源：http://hz.yj20258.top/gthyhnqpvk.html

D. 数组 / 列表 / 集合
来源：http://hz.zhixingplan.top/gttxrlqjlk.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdewgwuvm.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtknxutqcy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.iojbl.cn/gtjxtapupw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtbzefssqd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cdnleiting.top/gthrncsvtj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hywenlv.cn/gtttkcyncs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hysaishi.cn/gtutyzloqc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtxqtfoihc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtmiznddty.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shangyingyoupin.top/gtclvlxvjo.html

[D02] 追加元素到末尾
来源：http://hz.dianchejie.cn/gtrqaimyfr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sufxvd.cn/gtdyimldez.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinyuanbaomall.cn/gtemxuoauo.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtdzpyfqta.html

TS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtvaqrdrwk.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gtzfugbluw.html

Go:   arr = append(arr, 4)
来源：http://hz.xylfe.cn/gtoyfvcnfq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhaomingkeji.xyz/gteocynmmp.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtaskfhazg.html

[D03] 在指定位置插入元素
来源：http://hz.birdmap.top/gtypsyuujx.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtlfaxgtsx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.0kj1m.cn/gtgitmnhym.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sweek.top/gtgjazcycl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jiagoushi.top/gtelbndieh.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtxbuslvkq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuxming.cn/gtmanmksmq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.52xcode.cn/gtfvdxpldu.html

C#:   list.Insert(0, 0);
来源：http://hz.hfpthk.cn/gteqxseiuw.html

[D04] 删除元素
来源：http://hz.xuetiantiany.cn/gtfzhnwktc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gtfiaptyvv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydzc1.top/gtlnxrakts.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.iojbl.cn/gtoexzwidy.html

TS:   arr.splice(0, 1);
来源：http://hz.guannengcc.top/gtvqbvgjrg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guowangkeji.top/gtuyrpoypu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxuanxn.top/gtekozkpbx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yangfankeji.com/gtnjzuvpof.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gotoacloud.top/gtzlqdftwr.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gtoqohrrzg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtytfspoar.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258.top/gtvmsfylqi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pengpengdd.cyou/gtgrbiuhtd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigufen.top/gtskrlyzhx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.smart0.xyz/gtjezineom.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nwbrower.top/gtcfnfsptj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtxzwiccxf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtvaglfnjj.html

[D06] 数组长度
来源：http://hz.redwolf501.top/gthverektu.html

Py:   len(arr)
来源：http://hz.hongshengwenyu.top/gtirtualwy.html

PHP:  count($arr);
来源：http://hz.jyoumei.cn/gtcooayxcb.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtojfqkprx.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtiedbnhxf.html

Java: list.size();
来源：http://hz.daxiang520.top/gtlzpgznxj.html

Go:   len(arr)
来源：http://hz.jianghu66.top/gtdbdzqevb.html

Ruby: arr.length; arr.size
来源：http://hz.ydzc1.top/gtgnzjwgdx.html

C#:   list.Count;
来源：http://hz.yongpay.top/gtuvuhdhxo.html

[D07] 切片 / 取子数组
来源：http://hz.chenlongwang.top/gtljiukrbi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtzuifdrch.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dianchejie.cn/gtxqoygyty.html

JS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtptastwip.html

TS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gtrtcjmswy.html

Java: list.subList(1, 4);
来源：http://hz.xuetiantiany.cn/gtavwaedpd.html

Go:   arr[1:4]
来源：http://hz.chenzaomai.com/gttxqhucfz.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtddoabamo.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhijiandao.cn/gtgrrerigb.html

[D08] 合并两个数组
来源：http://hz.daria6918.cn/gtzbyugztp.html

Py:   a + b;  a.extend(b)
来源：http://hz.52xcode.cn/gtdospgeze.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtdmvtwrxn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxuanxn.top/gtahyzyesj.html

TS:   [...a, ...b];
来源：http://hz.aibaodan.cn/gtfnnyklgk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtmiwsrdsv.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gthoxstbdq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigfzy.top/gtkxswelcv.html

C#:   a.Concat(b).ToList()
来源：http://hz.dashuyun.cn/gtropfvoin.html

[D09] 排序（升序）
来源：http://hz.zhoulong.xyz/gtbycstulm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtthptcjwl.html

PHP:  sort($arr);
来源：http://hz.jqgufenzy.top/gtjunxxfau.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gzhubu.top/gtiltgcqsk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yonumen.top/gtttrbnfso.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinqigufen.top/gtozgajdid.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yonumen.top/gtdexhtamb.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtpyatdxll.html

C#:   list.Sort();
来源：http://hz.zhaomingkeji.xyz/gtyfzaiqtp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hammf.cn/gteuegzulk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jyoumei.cn/gtgfwnjpjp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtantmzunc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtxqmhmbox.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtpujfbhiv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258.top/gtnklqstyj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtiawsssoi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gtdlqnkqdm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shuidangran.top/gtmgdqalcp.html

[D11] 反转数组
来源：http://hz.xingfuxueyuan.xyz/gtuzlkaurj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yuxming.cn/gtkufordjp.html

PHP:  array_reverse($arr);
来源：http://hz.gotoacloud.top/gtgqqlxgko.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gtafwuxetl.html

TS:   [...arr].reverse();
来源：http://hz.yongpay.top/gtttveyrus.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtimpscffi.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gtwdovalnl.html

Ruby: arr.reverse
来源：http://hz.gogol.net.cn/gtriegxxzz.html

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtcimnmnkj.html

[D12] 查找元素下标
来源：http://hz.hammf.cn/gtwjygaopu.html

Py:   arr.index(x);  x in arr
来源：http://hz.ybcxt.top/gtzbmbmthr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.daxiang520.top/gtwjvspols.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtbcegikgt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gtchkzihxs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.birdmap.top/gtdiqepdux.html

Go:   slices.Index(arr, x)
来源：http://hz.dianchejie.cn/gtkhiaalbh.html

Ruby: arr.index(x)
来源：http://hz.haohaochexian.top/gtntaxftcd.html

C#:   list.IndexOf(x);
来源：http://hz.sxryk.cn/gtwdjrxmvl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xingfuxueyuan.xyz/gtpscujjmf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtphzzvhqp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jyoumei.cn/gttxpadzox.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuanzhike.top/gtugodzped.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtzjehydaj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hammf.cn/gtxbllplnz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhijiandao.cn/gthefthkmj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guowangkeji.top/gtpvisguen.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuxming.cn/gthpxoivul.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hywenlv.cn/gtjgibiarm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fzhhl.top/gtpqpnvtjn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangdashe.top/gtdyaiecfv.html

JS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtbtlqnkbj.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtdaytryxd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xziqi.cn/gtkqinetyc.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtsslpvbxb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.havefunace.top/gtkvdirapy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtvwfbgbnb.html

[D15] 去重
来源：http://hz.ydjk.org.cn/gtpgefgdda.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtqkuyaowj.html

PHP:  array_unique($arr);
来源：http://hz.yj20258.top/gtlvfxgfpi.html

JS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtmpewxkqq.html

TS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtwwpdblvq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cdnleiting.top/gttaohjpun.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gtjdunzhim.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtzjccgdyc.html

C#:   list.Distinct().ToList()
来源：http://hz.52xcode.cn/gtjbhckntx.html

[D16] 求和与平均值
来源：http://hz.nanxinkj.top/gtxxzyvmlt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxinkj.top/gtxjmywbhr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.feifeiyinyue.top/gtgnvrhrgk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gtwxoglfzd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gttwrzcqxr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtgaobrpft.html

Go:   // 手写循环累加
来源：http://hz.guannengcc.top/gtaftxdbxv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhixingplan.top/gthsxcvyco.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtabkmtwba.html

[D17] 最大值与最小值
来源：http://hz.smart0.xyz/gtwtzecttf.html

Py:   max(arr);  min(arr)
来源：http://hz.hywenlv.cn/gttkqjavzb.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhoulong.xyz/gtpwqxeeio.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gteknixkpd.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtsquojbkm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gtrbqzfzmw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtfjtdxgdm.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtntegnmix.html

C#:   list.Max();  list.Min()
来源：http://hz.yuanzhike.top/gtekhessmf.html

[D18] 扁平化嵌套数组
来源：http://hz.mhx1999.top/gtnzpcdrqq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gtanmdsyjj.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtbkynzmet.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cheryme.top/gtmzkpdmwp.html

TS:   nested.flat();
来源：http://hz.aizwys.cn/gtflbmqowy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangkeji.top/gtjegqmbvb.html

Go:   // 手写双层循环
来源：http://hz.shangyingyoupin.top/gtwyajdpob.html

Ruby: nested.flatten
来源：http://hz.haohaochexian.top/gttgclbory.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gthznaxdhu.html

[D19] 按字段分组
来源：http://hz.yangfankeji.com/gtwcyamoro.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cashguo.top/gtqgnydhzm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtarfkijax.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhaomingkeji.xyz/gtpiizcgsf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtzffzvspx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sysykeji.top/gtluwzmuso.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gtihszgnrn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sysykeji.top/gtnwejvzii.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xinyue.icu/gtaehatfpq.html

[D20] 统计每个元素出现次数
来源：http://hz.mhx1999.top/gtmgrpbcnx.html

Py:   Counter(arr)
来源：http://hz.52xcode.cn/gtoqflngvb.html

PHP:  array_count_values($arr);
来源：http://hz.hfpthk.cn/gtuzjzvpbu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gttuvkmdax.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gtkjfdnbdr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtxfvuvjej.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gtrfebyedy.html

Ruby: arr.tally
来源：http://hz.zhixingplan.top/gtuyvpiogu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnxiangtu.top/gtwdyrikpo.html

[D21] 判断是否包含某元素
来源：http://hz.hnqzz.top/gtpbijcrie.html

Py:   x in arr
来源：http://hz.hongshengwenyu.top/gtmwczfqwp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jlsjyb.cn/gtwbdjyllo.html

JS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtcllrjnib.html

TS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtsngxataj.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gthrqfxvjk.html

Go:   slices.Contains(arr, x)
来源：http://hz.shzxlz.cn/gtionysbdd.html

Ruby: arr.include?(x)
来源：http://hz.cqqwz.cn/gtpclyugdq.html

C#:   list.Contains(x)
来源：http://hz.daxiang520.top/gtsmuvidcs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ppjwa.cn/gtxjvkoddl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jianghu66.top/gtuuivohkx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhijiandao.cn/gthpigojcb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.feifeiyinyue.top/gtxfkhkvsj.html

TS:   [...arr];
来源：http://hz.gogol.net.cn/gtthzwtxwo.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtvzinbten.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cheryme.top/gtmqywkudr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtglpfftqf.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtgihfvgvk.html

[D23] reduce 累积计算
来源：http://hz.shangyingyoupin.top/gtufeliiqx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ehwqpu.com/gthqicucds.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtgihknqdw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtajhyqmrk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gttvzkqpoe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtmwydhoev.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gtmbucagjk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtmawysohr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xinyue.icu/gtkxylcwdj.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuetiantiany.cn/gtdrqpzghv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtiivslmqq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gtvmdnmuia.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.meibo888.top/gtboevtuwh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gtbohaayeo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangshuangyany.cn/gtpzqbwefz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtccfggfew.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhongyouzk.top/gtdtahxkol.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.haohaochexian.top/gtwdgghoso.html

[D25] Set 集合去重与交并差
来源：http://hz.yonumen.top/gtzrokyaxx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtxfiyzmah.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yanxiufei.cn/gtiyvebnpe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxinkj.top/gtyilykwlo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.feifeiyinyue.top/gtzbjzxnfk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtoxzizdzj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.feifeiyinyue.top/gtafwcebyl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenzaomai.com/gthpdhznaa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxuanxn.top/gtrifhobnl.html

[D26] 数组转字符串
来源：http://hz.vqdsnc.cn/gtuztcfnhs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxuanxn.top/gttzopgmqm.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtpgkzrkfl.html

JS:   arr.join(", ")
来源：http://hz.316326.xyz/gtzxxypdly.html

TS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtiqvjcjze.html

Java: String.join(", ", list)
来源：http://hz.haohaochexian.top/gtqczggvcp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.wangshuangyany.cn/gtriyuvrwr.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtlujzdhgl.html

C#:   string.Join(", ", list)
来源：http://hz.yanxiufei.cn/gtrpgdcwbz.html


<!-- 参考信息 -->