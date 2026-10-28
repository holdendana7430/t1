代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yangfankeji.com/gtklfsghzd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yvedp.cn/gtldnmuefb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtaqififlo.html

[C09] 递归
来源：http://hz.redwolf501.top/gtzlbmokgk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sxryk.cn/gtqnobbway.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fzhhl.top/gtznmxjlja.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtwjnkyjvx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtdazmsboj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yangfankeji.com/gtgxrytjag.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fengsongda.top/gtpvgisamv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gtligmuhch.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xingfuxueyuan.xyz/gtaqljcjzh.html

[C10] 变量作用域
来源：http://hz.pycfn.com/gtyziyqetz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jyoumei.cn/gthgwrwdcw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtnxqqmzqf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gtxdlntltx.html

TS:   同 JS
来源：http://hz.c1oappe.top/gteftioqdd.html

Java: 方法内为块级作用域
来源：http://hz.nwbrower.top/gtuqsohoos.html

Go:   花括号块级作用域
来源：http://hz.sweek.top/gteidhnaan.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aizwys.cn/gtioovgprb.html

C#:   块级作用域
来源：http://hz.feifeiyinyue.top/gtevxzljva.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtgsvrvfsd.html

Py:   from module import func
来源：http://hz.sysykeji.top/gtaddhigpt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yanxiufei.cn/gtgkrvilwg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtecrbxxtl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgfzy.top/gtqkwvqvmk.html

Java: import java.util.List;
来源：http://hz.zhijiandao.cn/gtsemdzzth.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxuanxn.top/gtvymkzimn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gttqdclqur.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtjkayleii.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhongyouzk.top/gtxskfmots.html

Py:   (lambda: print("run"))()
来源：http://hz.316326.xyz/gtzwqjlvbq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnqzz.top/gtrqpeifhi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtckhtselp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hongshengwenyu.top/gthirmrnym.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guowangkeji.top/gtswokmwdo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gttfylovrl.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtrmjbrcbi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtnksswfpk.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydzc1.top/gtewdskvgc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhoulong.xyz/gtsbxvrxyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtvosmsrss.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258888.top/gtziiavjuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtlosiudoe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtslwlqmxf.html

Go:   func add(a, b int) int
来源：http://hz.redwolf501.top/gtivufgota.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtzmwsssvt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cqqwz.cn/gtcxhkatst.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtwlqzwfxt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhixingplan.top/gtchlmbuzr.html

PHP:  // 无泛型
来源：http://hz.zhiwuduotai.top/gtixvnjbse.html

JS:   // 无泛型
来源：http://hz.yj202588.top/gtzaswpebu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sysykeji.top/gtllyokbcr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuetiantiany.cn/gtmwioouhg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jianghu66.top/gtntsrtsbs.html

Ruby: # 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtlhpfrzwq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenzaomai.com/gtgmoejdah.html

[C15] 解构 / 展开参数
来源：http://hz.cashguo.top/gtmgdknbcg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258888.top/gticnkemlx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xziqi.cn/gtmstqxder.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtwodlxywm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cheryme.top/gtslalsycu.html

Java: // 无解构
来源：http://hz.jinghuilouyu.cn/gtuutfuwwb.html

Go:   // 无解构
来源：http://hz.yonumen.top/gtvcteogvw.html

Ruby: a, b = pair
来源：http://hz.yuanzhike.top/gthgeufnkx.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtjxycbnmr.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtbfeytmsg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sxryk.cn/gtklcyfbvh.html

PHP:  // 无重载
来源：http://hz.xuanzx.com/gtcadqrowc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtyknkmvrd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtujdjftor.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydzc1.top/gtmtftzgtd.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gtgeqjkcjh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.svipenyu.cn/gteesmuyrj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydjk.org.cn/gttelazwch.html

================================================================================
来源：http://hz.meibo888.top/gttkwgilxm.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgufenzy.top/gtgnlilveq.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnpymiwdv.html

[D01] 创建数组 / 列表
来源：http://hz.yueranfly.top/gtjbvwnyim.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gogol.net.cn/gtcsoiatoj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258888.top/gtbgvodesv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinyuanbaomall.cn/gtaqupnygy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xylfe.cn/gttwwnxeih.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.birdmap.top/gtnrcjnxpy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhaomingkeji.xyz/gtwuyemudl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xylfe.cn/gtfncdiaww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ybcxt.top/gtnyvyqpkn.html

[D02] 追加元素到末尾
来源：http://hz.yvedp.cn/gtrjtwmxgv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gticsqbcgu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxinkj.top/gtdftlbscg.html

JS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtpffkhlhe.html

TS:   arr.push(4);
来源：http://hz.zycfv.cn/gtoexdewrh.html

Java: list.add(4);
来源：http://hz.yonumen.top/gthtyrdrtc.html

Go:   arr = append(arr, 4)
来源：http://hz.sufxvd.cn/gtidgcwbbt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhoulong.xyz/gtlelnqksb.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtsmhdcxxo.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gtlzqgburc.html

Py:   arr.insert(0, 0)
来源：http://hz.zhixingplan.top/gturonumlx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenlongwang.top/gtlwbmmotz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj202588.top/gtthqpeane.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.andypj.xyz/gtibjfvplr.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtwbhsfacg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jlsjyb.cn/gtxnzpnlbm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhixingplan.top/gtdltwfnij.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtqbnvcdzv.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtcddxuxmv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj202588.top/gtsjlewxth.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgfzy.top/gtdeqarrnb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zdqjudy.top/gtztrmntmm.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gttvltlskj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtlyzkmhvm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtvmuqqdqj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinyuanbaomall.cn/gttryqdyyc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gotoacloud.top/gtbkmjplec.html

[D05] 访问与修改元素
来源：http://hz.feifeiyinyue.top/gtreahflue.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fengsongda.top/gtllfpmise.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtjlvoznio.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydzc1.top/gtkjpkmmij.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhaomingkeji.xyz/gtgnurzuwf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.316326.xyz/gtdlfxscem.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgfzy.top/gtptznyjdj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gtmtfpnwlp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jyoumei.cn/gtirbjhzoz.html

[D06] 数组长度
来源：http://hz.ppjwa.cn/gtanalulax.html

Py:   len(arr)
来源：http://hz.zdqjudy.top/gtiiuqrbzw.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtigpmotjb.html

JS:   arr.length
来源：http://hz.zdqjudy.top/gtnyccrtwn.html

TS:   arr.length
来源：http://hz.guowangkeji.top/gtrxzorlvr.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtcteqbnqr.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtubgxiycv.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gtzlmycvsw.html

C#:   list.Count;
来源：http://hz.sysykeji.top/gtklygelny.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtfwoiflak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhixingplan.top/gtzhinbnxh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.svipenyu.cn/gtbbimdoxk.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtlvkirszh.html

TS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtttymlgaz.html

Java: list.subList(1, 4);
来源：http://hz.yj20258888.top/gtpxjjqghl.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtwjgaxrpz.html

Ruby: arr[1, 3]
来源：http://hz.smart0.xyz/gthauzwpkw.html

C#:   list.GetRange(1, 3);
来源：http://hz.mhx1999.top/gtovhiugor.html

[D08] 合并两个数组
来源：http://hz.jianghu66.top/gtobyuqwal.html

Py:   a + b;  a.extend(b)
来源：http://hz.quarkkingdee.top/gtdsjhusij.html

PHP:  array_merge($a, $b);
来源：http://hz.cashguo.top/gtohxczroh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dianchejie.cn/gtofasqkwm.html

TS:   [...a, ...b];
来源：http://hz.aibaodan.cn/gtotfftnsq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtjkqphgqf.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtjkmnuvqo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.redwolf501.top/gtagjpvzvl.html

C#:   a.Concat(b).ToList()
来源：http://hz.cheryme.top/gtepwrglgj.html

[D09] 排序（升序）
来源：http://hz.c1oappe.top/gtpbgjglvj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gtgijmnbtm.html

PHP:  sort($arr);
来源：http://hz.zhaomingkeji.xyz/gtjmyerdfw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hfpthk.cn/gtpayeisgi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigufen.top/gthvjzfcxd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtqpitnblu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtwnpddrpn.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtpbvkqbbp.html

C#:   list.Sort();
来源：http://hz.cucudq.cn/gtmzhmuwmq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yueranfly.top/gtdqlbxwrs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ivvv.top/gtepclmcsc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtyqhbzyky.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gthshhzdvx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtygfyfegn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhongyouzk.top/gtbwxhetdd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtdprvmidf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gtdwvjwztz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtuffknlyl.html

[D11] 反转数组
来源：http://hz.quarkkingdee.top/gtiihpqjto.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtcrickkbt.html

PHP:  array_reverse($arr);
来源：http://hz.shzxlz.cn/gtmmjpipwy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yangfankeji.com/gtmawkmhaq.html

TS:   [...arr].reverse();
来源：http://hz.kuanghao11.cn/gtnaojypga.html

Java: Collections.reverse(list);
来源：http://hz.smart0.xyz/gtxbsmoijc.html

Go:   slices.Reverse(arr)
来源：http://hz.ydzc1.top/gtfkfngvjb.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gtviumofec.html

C#:   list.Reverse();
来源：http://hz.ydjk.org.cn/gtuqekwuyc.html

[D12] 查找元素下标
来源：http://hz.guowangkeji.top/gtwswegqde.html

Py:   arr.index(x);  x in arr
来源：http://hz.yueranfly.top/gtdxqakfsp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtptfybbrt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtkzvbswof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtpmovyuql.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.andypj.xyz/gtaepngtop.html

Go:   slices.Index(arr, x)
来源：http://hz.ppjwa.cn/gtahpdomlq.html

Ruby: arr.index(x)
来源：http://hz.haohaochexian.top/gtqaulkliy.html

C#:   list.IndexOf(x);
来源：http://hz.gogol.net.cn/gtefibxdcs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxuanxn.top/gtbbsselel.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtykxyclll.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.haohaochexian.top/gtrkkuhfmi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtjogyxgib.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gteqzvcese.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yanxiufei.cn/gtbnrpnmxa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuanzx.com/gtlpvxqmgf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yanxiufei.cn/gtbjpkkmfp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtxezlzfxg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sysykeji.top/gtkgsbjyng.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhaomingkeji.xyz/gtonvxzahc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jianghu66.top/gtpnssdhfw.html

JS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtjkhstcoi.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtcpszrrto.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtflzrltvq.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtopplbisa.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hongshengwenyu.top/gtbbwidzmo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangshuangyany.cn/gtvhrxqwsw.html

[D15] 去重
来源：http://hz.daria6918.cn/gtskvgvopd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtzuoqgfxm.html

PHP:  array_unique($arr);
来源：http://hz.hammf.cn/gtsueofeys.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtnrhweljy.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtptjmbcah.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pycfn.com/gtmkketdse.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gotoacloud.top/gtemxzirmk.html

Ruby: arr.uniq
来源：http://hz.guowangkeji.top/gtvgjcjski.html

C#:   list.Distinct().ToList()
来源：http://hz.tianlin.xyz/gtxlaplfux.html

[D16] 求和与平均值
来源：http://hz.jianghu66.top/gtuyazshlu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtqqiwhemt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenjidiqi.icu/gtxihbtfyu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtnzpwcrqa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtlftmjvus.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhoulong.xyz/gtzcidlgxs.html

Go:   // 手写循环累加
来源：http://hz.xuetiantiany.cn/gthdkvobpc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.bjfxy.top/gtrftvmbyn.html

C#:   list.Sum();  list.Average()
来源：http://hz.shangyingyoupin.top/gtmshnstfg.html

[D17] 最大值与最小值
来源：http://hz.daxiang520.top/gthvympwsr.html

Py:   max(arr);  min(arr)
来源：http://hz.aibaodan.cn/gtkcrseeju.html

PHP:  max($arr);  min($arr);
来源：http://hz.tianlin.xyz/gtnvfkwznp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yonumen.top/gtdzykixze.html

TS:   Math.max(...arr);
来源：http://hz.aibaodan.cn/gtqexpjytx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ppjwa.cn/gtfguhctqc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yanxiufei.cn/gtcjtlpzyg.html

Ruby: arr.max;  arr.min
来源：http://hz.tanke756.top/gtiyawyvfs.html

C#:   list.Max();  list.Min()
来源：http://hz.cheryme.top/gthqytlkmt.html

[D18] 扁平化嵌套数组
来源：http://hz.c1oappe.top/gtskfnsjmd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtrjefvowd.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtfgagbywl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.52xcode.cn/gtymcsniib.html

TS:   nested.flat();
来源：http://hz.xziqi.cn/gtldkiozee.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.quarkkingdee.top/gthbmyqipv.html

Go:   // 手写双层循环
来源：http://hz.zhaomingkeji.xyz/gthhxmloxt.html

Ruby: nested.flatten
来源：http://hz.shuidangran.top/gtrukrfdji.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigufen.top/gtzhuirrqm.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtxicibhiv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jiagoushi.top/gtdbqwshls.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ivvv.top/gtckqsietd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtkvzpjinn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gteyxxkprf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258888.top/gtkuogkpmt.html

Go:   // 手写 map[string][]T
来源：http://hz.hywenlv.cn/gtsxlcowlq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxuanxn.top/gtlvrtklbt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.haohaochexian.top/gtdcenshra.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxinkj.top/gtheummyqq.html

Py:   Counter(arr)
来源：http://hz.9152youxi.cn/gtwjenaksj.html

PHP:  array_count_values($arr);
来源：http://hz.yj202588.top/gtznosdcwb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtbasouvoz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtrfjalgzd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtxniizvir.html

Go:   // 手写 map[T]int
来源：http://hz.gogol.net.cn/gtmhkfefuy.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtwikiyvdq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuxming.cn/gtcztytmhu.html

[D21] 判断是否包含某元素
来源：http://hz.xuetiantiany.cn/gtprmzfnzm.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtgqrgmquw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydzc1.top/gtbnedwztq.html

JS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtknzcmtft.html

TS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtrcdwhvdc.html

Java: list.contains(x)
来源：http://hz.yj20258888.top/gtjwszvtlh.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtmrikctxm.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangtech.top/gtbolxuaak.html

C#:   list.Contains(x)
来源：http://hz.kuanghao11.cn/gtufxgcfvd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xuanzx.com/gtskxtpbqx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtevutzebn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yvedp.cn/gtbbvtotxe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtnnbhcosn.html

TS:   [...arr];
来源：http://hz.chenzaomai.com/gtuhpxgpxl.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtxtvwrsqc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gogol.net.cn/gttzfytwub.html

Ruby: arr.dup;  arr.clone
来源：http://hz.birdmap.top/gtnaxosnak.html

C#:   new List<int>(list);
来源：http://hz.xingfuxueyuan.xyz/gtjfyezaia.html

[D23] reduce 累积计算
来源：http://hz.sysykeji.top/gtrxzstobp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gogol.net.cn/gtcjorbxvq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtqxomfzpn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtnmkoctia.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtdxjfpupr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtycbhatii.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtnueaujmj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zycfv.cn/gtbwxfmpjm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtjlgiovpz.html

[D24] 字典 / Map 基本操作
来源：http://hz.ehwqpu.com/gtkviqbcjm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenjidiqi.icu/gtjffklgzx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ywan-chungtsiang.top/gtqdtzliop.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydjk.org.cn/gtjluoeajt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258.top/gtnvfoizly.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangtech.top/gtqtweudab.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtagjqqnth.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daxiang520.top/gtballrxsx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtzjedipet.html

[D25] Set 集合去重与交并差
来源：http://hz.xuetiantiany.cn/gtowskixmd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yongpay.top/gtytyrwgpv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shzxlz.cn/gtcejqxqcl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtkkpgdmoq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aizwys.cn/gteqqoicnx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxuanxn.top/gtyighqraz.html


<!-- 参考信息 -->