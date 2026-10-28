代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.xuanzx.com/gtqlesabdd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dianchejie.cn/gtkjhpxugh.html

[C08] 闭包
来源：http://hz.hongshengwenyu.top/gtmbbtwlfh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhiwuduotai.top/gtbxkuestx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aizwys.cn/gtlsidrpfp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtmcegatla.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtexwspvaf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigfzy.top/gtwwlqjctu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtswnvrmfv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ivvv.top/gthbwiooir.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtlgrfypjb.html

[C09] 递归
来源：http://hz.sxryk.cn/gtwxhmrhfv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtqoxxmexz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fengsongda.top/gttghernfw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtpsootqhv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gtqshdbnfd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.redwolf501.top/gtehxtozfg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.quarkkingdee.top/gtyritnmfl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daria6918.cn/gtapmfzskp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtnhgtnhki.html

[C10] 变量作用域
来源：http://hz.sxryk.cn/gtwblusuzy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jlsjyb.cn/gtnatolppg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtgoyguizy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.0kj1m.cn/gtjodcjqcu.html

TS:   同 JS
来源：http://hz.hongshengwenyu.top/gtmxgciuca.html

Java: 方法内为块级作用域
来源：http://hz.cqqwz.cn/gtjtktldfk.html

Go:   花括号块级作用域
来源：http://hz.wangdashe.top/gtjuusuzfi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aibaodan.cn/gtyoiokddp.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtfgdpiyue.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtrofbsmqt.html

Py:   from module import func
来源：http://hz.jinqigfzy.top/gtogdlggyy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.feifeiyinyue.top/gtrfyxtasm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yangfankeji.com/gthdjqvleo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jianghu66.top/gtxoxbpahq.html

Java: import java.util.List;
来源：http://hz.jqgufenzy.top/gtlbvxzbju.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hysaishi.cn/gtnsjrmzev.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.guannengcc.top/gtdlomhwic.html

C#:   using System.Text;
来源：http://hz.iojbl.cn/gthgmfxmjk.html

[C12] 立即执行函数 IIFE
来源：http://hz.wangdashe.top/gtevuihmbk.html

Py:   (lambda: print("run"))()
来源：http://hz.zdqjudy.top/gtrhnfoqkt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtbinnweta.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtpatouhnu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gteyylzgne.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangtech.top/gtvuyznykz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtfajuudfb.html

Ruby: -> { puts "run" }.call
来源：http://hz.iojbl.cn/gtfakavpkt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtbuekjvdg.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gttryvrgcc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ydjk.org.cn/gtpgwlcrxu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtxpksrecm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtbiynyptc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.52xcode.cn/gtbyiivljk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtbxwdedhn.html

Go:   func add(a, b int) int
来源：http://hz.jqgufenzy.top/gtzatuuvcw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.snrcjt.cn/gtpbfaccny.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgufenzy.top/gtcwmymcak.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtecaaczmg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtiytawzyl.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtirxrpvvf.html

JS:   // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtlzgpysbi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhongyouzk.top/gtetzkqczf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guannengcc.top/gtiirhpkbw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guannengcc.top/gtmbjkxczu.html

Ruby: # 无泛型
来源：http://hz.shzxlz.cn/gteakfrcrb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtorgxlpsh.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gtwemzvenh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jyoumei.cn/gtuttprslq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.vqdsnc.cn/gtdlnrzuvp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtoeamhfag.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhixingplan.top/gtnuanwhdl.html

Java: // 无解构
来源：http://hz.yj202588.top/gtlnhlkmbu.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gtvqvxuklb.html

Ruby: a, b = pair
来源：http://hz.havefunace.top/gtioqaldat.html

C#:   var (a, b) = pair;
来源：http://hz.daxiang520.top/gtilubwrzb.html

[C16] 函数 / 方法重载
来源：http://hz.nanxuanxn.top/gtxxgwyubv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.snrcjt.cn/gtzzcdolut.html

PHP:  // 无重载
来源：http://hz.9152youxi.cn/gtvegtojmm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sweek.top/gtrjoitugy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yangfankeji.com/gtdirkvvjk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtnltcellu.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gtpkhdtfay.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhiwuduotai.top/gtqnciowfi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daxiang520.top/gtqskvwejj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfqosbdch.html

D. 数组 / 列表 / 集合
来源：http://hz.gzhubu.top/gtnwgzduro.html

================================================================================
来源：http://hz.hywenlv.cn/gtbambnhrm.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gtthxntmfr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.316326.xyz/gtnlzpvibn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuxming.cn/gtuokpbcnp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hysaishi.cn/gtdtitiint.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gzhubu.top/gtzjqpxsib.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ivvv.top/gtlnrhnavz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hongshengwenyu.top/gtnuohcpov.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tanke756.top/gtgyimqsbb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtwiafesbf.html

[D02] 追加元素到末尾
来源：http://hz.zhixingplan.top/gtawypjlpn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuanzhike.top/gtddesmaxr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gtwixbujfb.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gtvcmnpfby.html

TS:   arr.push(4);
来源：http://hz.chenzaomai.com/gttncpkhwe.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtxfcrpddr.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangtech.top/gtuziknmxn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtbnnnegcm.html

C#:   list.Add(4);
来源：http://hz.yj202588.top/gtynoomxeg.html

[D03] 在指定位置插入元素
来源：http://hz.zdqjudy.top/gtgdyzogdj.html

Py:   arr.insert(0, 0)
来源：http://hz.yj202588.top/gtjxbckxeu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtqraeaqow.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shangyingyoupin.top/gtaimjynux.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtpmsfjfit.html

Java: list.add(0, 0);
来源：http://hz.havefunace.top/gtqtnypvkv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.daria6918.cn/gtrkvypjap.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj202588.top/gttiwupnly.html

C#:   list.Insert(0, 0);
来源：http://hz.52xcode.cn/gtvsvdptyx.html

[D04] 删除元素
来源：http://hz.guannengcc.top/gtvuabcyui.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258.top/gtdcqqbdft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guowangkeji.top/gtggulfzee.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.havefunace.top/gtxrvuwggk.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gthuixahyc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtxpiqjhfk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sxryk.cn/gtldonfzwb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhoulong.xyz/gtzadimoup.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aizwys.cn/gtamyzvpnd.html

[D05] 访问与修改元素
来源：http://hz.snrcjt.cn/gtkaqvhnhl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtipylzegn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ehwqpu.com/gttyqbsdax.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tian-w.cn/gtpmpdplmj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cashguo.top/gtlvjnwrfq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtrleueuqt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtahjqwppj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtjwkuzwgd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtjiktjerx.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtrykudoow.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtosbvjiok.html

PHP:  count($arr);
来源：http://hz.ydzc1.top/gtsayrnzgn.html

JS:   arr.length
来源：http://hz.pycfn.com/gtcocjhwqh.html

TS:   arr.length
来源：http://hz.sysykeji.top/gtehuutvsw.html

Java: list.size();
来源：http://hz.zycfv.cn/gtbpkcdsft.html

Go:   len(arr)
来源：http://hz.hongshengwenyu.top/gttmycylqm.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gthcwuxarq.html

C#:   list.Count;
来源：http://hz.ehwqpu.com/gtumezuhbg.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtfcqvmijp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnxiangtu.top/gtwmmoskcd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gtahfifjuy.html

JS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtkbgmptga.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtkmioogif.html

Java: list.subList(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtuoduzgxc.html

Go:   arr[1:4]
来源：http://hz.hywenlv.cn/gtovzigred.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtcnkkfkmb.html

C#:   list.GetRange(1, 3);
来源：http://hz.andypj.xyz/gtubkipqyl.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangkeji.top/gtwydntawd.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigfzy.top/gtxeiggfjr.html

PHP:  array_merge($a, $b);
来源：http://hz.chenzaomai.com/gtquwergur.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtdyrpcpwm.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtoatwibgf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtqgkmhkgy.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtmptqfhax.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhixingplan.top/gtctifokzg.html

C#:   a.Concat(b).ToList()
来源：http://hz.ywan-chungtsiang.top/gtmlxhwsni.html

[D09] 排序（升序）
来源：http://hz.mhx1999.top/gtakbfejip.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtfzjlynls.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangkeji.top/gtgcbmepve.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhaomingkeji.xyz/gtxpqsfkot.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gtnffcomvz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtpngucexu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtezjxeams.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtmiecgaze.html

C#:   list.Sort();
来源：http://hz.andypj.xyz/gtkyivkfzs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangdashe.top/gtqabpblfj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtnnbzvdsx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtgxvalrvc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtwyhkmlsa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtmhwozqyx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pycfn.com/gtyzdjbuej.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hysaishi.cn/gtiahozuqx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daxiang520.top/gtyoiyzcen.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangkeji.top/gtjbqnmdxu.html

[D11] 反转数组
来源：http://hz.daria6918.cn/gtitxyxrcu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtsoyvsfze.html

PHP:  array_reverse($arr);
来源：http://hz.yangfankeji.com/gtxamxcgqx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhengqikj.top/gtmtflmuxr.html

TS:   [...arr].reverse();
来源：http://hz.gaohongyu789.top/gtsvbmuzeu.html

Java: Collections.reverse(list);
来源：http://hz.jqgfzy.top/gtwsouluqq.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigufen.top/gtxawutgvy.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtsfmvebdt.html

C#:   list.Reverse();
来源：http://hz.redwolf501.top/gtmkuetjwo.html

[D12] 查找元素下标
来源：http://hz.ywan-chungtsiang.top/gtdrgewznn.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtzlpiyccm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtwhcfmpmv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtkuentpyu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtdblflphb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hnxiangtu.top/gtfnpafvrf.html

Go:   slices.Index(arr, x)
来源：http://hz.wangshuangyany.cn/gtcdkoalra.html

Ruby: arr.index(x)
来源：http://hz.wangdashe.top/gtmnxeeacr.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtvelpakay.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guannengcc.top/gtmyqpvvtv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gaohongyu789.top/gtlrzgctkt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.redwolf501.top/gtkiozwvek.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gthdwyacle.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenzaomai.com/gtpcnqiucs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aibaodan.cn/gtmmanhrrj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuanzx.com/gtnvlifgqw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtyqrikzaz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.haohaochexian.top/gtiazatmsy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhijiandao.cn/gtuobrkxef.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.svipenyu.cn/gtqcdnuzya.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.kuanghao11.cn/gtuposuida.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtvpksyhrh.html

TS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtoedazgqm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtbcvgsamx.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gttejzaswt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhoulong.xyz/gtfbhnsyvl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yj202588.top/gtajswidud.html

[D15] 去重
来源：http://hz.c1oappe.top/gtmmbhjgcg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gtplhrrlhj.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtgittgmht.html

JS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gthebbpojb.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtlojdhsnf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yueranfly.top/gtthydtpzk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtmzbxszaf.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtunbifzbs.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258.top/gtripsgwex.html

[D16] 求和与平均值
来源：http://hz.pengpengdd.cyou/gtprzqildj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydjk.org.cn/gtcamewrwc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.haohaochexian.top/gtcpqdriac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gttqlnmohb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenjidiqi.icu/gtrgysdbuw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.bjfxy.top/gtxmuiefth.html

Go:   // 手写循环累加
来源：http://hz.cashguo.top/gtjttnmmos.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gtnhiveafu.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhoulong.xyz/gtcrsmnhzp.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gthxhmlfei.html

Py:   max(arr);  min(arr)
来源：http://hz.cashguo.top/gtztqqxkvk.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigufen.top/gtksostrxh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtpsqczsbg.html

TS:   Math.max(...arr);
来源：http://hz.daria6918.cn/gtfvowkmfd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cdnleiting.top/gtszciqwbe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtblcobmbe.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gttavjcksc.html

C#:   list.Max();  list.Min()
来源：http://hz.bjfxy.top/gtfoifxjco.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtwcqepjws.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sxryk.cn/gttfmahnrf.html

PHP:  array_merge(...$nested);
来源：http://hz.zdqjudy.top/gtqqbicmhh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangshuangyany.cn/gtpjcvydjb.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtvkopgwgr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xylfe.cn/gtmpycpdyh.html

Go:   // 手写双层循环
来源：http://hz.jiagoushi.top/gtzheoosqd.html

Ruby: nested.flatten
来源：http://hz.tian-w.cn/gtmppkbpir.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtvyyzehyn.html

[D19] 按字段分组
来源：http://hz.xuanzx.com/gtetfdqolr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuxming.cn/gtvxjaaikx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zdqjudy.top/gtujdsrzdb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xingfuxueyuan.xyz/gtqhwflylu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtolyaroko.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shuidangran.top/gtrhtoxbdb.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gthoverkhg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtaufwxeff.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtumkbsdfo.html

[D20] 统计每个元素出现次数
来源：http://hz.zycfv.cn/gtmsivchft.html

Py:   Counter(arr)
来源：http://hz.chenzaomai.com/gtdkieddvz.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gthseyhoke.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtypyznrdp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtatlfkqaq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtleijfpfp.html

Go:   // 手写 map[T]int
来源：http://hz.hnqzz.top/gtctbxbgbm.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtrppmggzu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtbawcsuke.html

[D21] 判断是否包含某元素
来源：http://hz.redwolf501.top/gttqipcyop.html

Py:   x in arr
来源：http://hz.shzxlz.cn/gtwiltkpca.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtsuaepmpg.html

JS:   arr.includes(x)
来源：http://hz.sxryk.cn/gthjrotzlc.html

TS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtzgpucmtu.html

Java: list.contains(x)
来源：http://hz.cdnleiting.top/gtctspyxbn.html

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtygvzibza.html

Ruby: arr.include?(x)
来源：http://hz.cheryme.top/gtjohgmpyl.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gtnpuhczxn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gtlmxsalqi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dianchejie.cn/gtktpyrqxe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gtqknholyt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj202588.top/gtdpdytrez.html

TS:   [...arr];
来源：http://hz.cdnleiting.top/gtqxkexcto.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtqqopmctk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pengpengdd.cyou/gtutnxtueh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ppjwa.cn/gtvhxxjrdz.html

C#:   new List<int>(list);
来源：http://hz.ydzc1.top/gttpzkxpwb.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gttmjnklux.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gtgteslybs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtqjxpgpcg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtapiborag.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gteyiijjfh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.fzhhl.top/gtwzswjrle.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtqosmherl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ppjwa.cn/gteyetvrjc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtesrqkfdi.html

[D24] 字典 / Map 基本操作
来源：http://hz.feifeiyinyue.top/gtgvrckoae.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jyoumei.cn/gtoggrwpsl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jyoumei.cn/gtyrejzqgv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangdashe.top/gtvtbfqryq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtfifjitmn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangtech.top/gtsjsdaccx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shuidangran.top/gtbzomfmhn.html


<!-- 参考信息 -->