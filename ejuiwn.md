代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.daria6918.cn/gtfdkfhogj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigufen.top/gtwgeihldx.html

[C08] 闭包
来源：http://hz.nanxinkj.top/gtskojtefp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shuidangran.top/gttxrzhdnm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yuanzhike.top/gtylqcrhoe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtvtuyvfhl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtmssojrnr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.svipenyu.cn/gtpjvzchlk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gtlbvoewkp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pengpengdd.cyou/gtxyrgwjnr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtyqbfmyum.html

[C09] 递归
来源：http://hz.tian-w.cn/gtntqzqtxh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtolaqgoms.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtehzrameh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtvucqgssx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtxpksiiex.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jlsjyb.cn/gtxuvmqakn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hywenlv.cn/gttoipppgz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ivvv.top/gtyhaerpxh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhengqikj.top/gtguowxhrl.html

[C10] 变量作用域
来源：http://hz.zhongyouzk.top/gtjrqawtsb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aibaodan.cn/gtbibnsjvv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigfzy.top/gtpbkdzimn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.havefunace.top/gtfndnscls.html

TS:   同 JS
来源：http://hz.tanke756.top/gtcxerkkbq.html

Java: 方法内为块级作用域
来源：http://hz.svipenyu.cn/gtxfibfbxq.html

Go:   花括号块级作用域
来源：http://hz.jinghuilouyu.cn/gtorzzqebq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydzc1.top/gtxklwdrrv.html

C#:   块级作用域
来源：http://hz.fzhhl.top/gtnbedaooc.html

[C11] 模块导入与导出
来源：http://hz.gaohongyu789.top/gtkpgdlhkl.html

Py:   from module import func
来源：http://hz.feifeiyinyue.top/gthjbjokqk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gthxjhzdyv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuxming.cn/gtcwoqyvbu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tianlin.xyz/gtprfgnoho.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtjdtgcqxq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.snrcjt.cn/gtlmffmkab.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtrsfkvcvc.html

C#:   using System.Text;
来源：http://hz.gogol.net.cn/gtwcdyfdxh.html

[C12] 立即执行函数 IIFE
来源：http://hz.52xcode.cn/gtbvdtvsir.html

Py:   (lambda: print("run"))()
来源：http://hz.havefunace.top/gtvbbdxtes.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuxming.cn/gtlixiyiyc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtpblptdcx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtyifvcear.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhongyouzk.top/gtlndeegwg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258.top/gtrlfttduz.html

Ruby: -> { puts "run" }.call
来源：http://hz.ywan-chungtsiang.top/gtydbribjc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtayqbftxu.html

[C13] 类型声明 / 类型注解
来源：http://hz.yangfankeji.com/gtqtwfobhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.svipenyu.cn/gtwjzqqtcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtwajmehii.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj202588.top/gtcwrsvlas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtxooqwhrj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtlnjkjvhr.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gtcmdhxmsq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.9152youxi.cn/gtnlkauorw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gtwytquieo.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtjcyserxj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhaomingkeji.xyz/gtledaqcou.html

PHP:  // 无泛型
来源：http://hz.fengsongda.top/gtnasdzmud.html

JS:   // 无泛型
来源：http://hz.zhiwuduotai.top/gtudfrrolc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangtech.top/gtgieptmpt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nanxinkj.top/gtmichfxvn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.c1oappe.top/gtnypichgz.html

Ruby: # 无泛型
来源：http://hz.ivvv.top/gtqpzkfvef.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenjidiqi.icu/gtnhcbasgr.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangkeji.top/gtwlkxxcue.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhijiandao.cn/gtkifwtdli.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangtech.top/gthbsvaecg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtrekhudrh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gtxaqxrbxx.html

Java: // 无解构
来源：http://hz.cheryme.top/gtygkhlihp.html

Go:   // 无解构
来源：http://hz.shanyushiyangtech.top/gtovihhoxg.html

Ruby: a, b = pair
来源：http://hz.ybcxt.top/gtibtuwght.html

C#:   var (a, b) = pair;
来源：http://hz.pengpengdd.cyou/gtahnngotv.html

[C16] 函数 / 方法重载
来源：http://hz.dashuyun.cn/gtaqvhgllu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtmktmwidq.html

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gtfkqrrfnn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtpjjsaoju.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj202588.top/gtgzgcoits.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.52xcode.cn/gtrtauerwa.html

Go:   // 无重载：用不同函数名
来源：http://hz.gaohongyu789.top/gtjxuzxrdv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.52xcode.cn/gttkhbssos.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gtnefjdgvu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpkmcjyjm.html

D. 数组 / 列表 / 集合
来源：http://hz.zhixingplan.top/gtutelmhxy.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpdkmrlqa.html

[D01] 创建数组 / 列表
来源：http://hz.dashuyun.cn/gtfxxutmia.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cqqwz.cn/gtdjqnxgqt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gtrgakyqiy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenlongwang.top/gtlhszzhxz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.birdmap.top/gtotdliroy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.feifeiyinyue.top/gtocmwfjow.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenzaomai.com/gtuusvqtpx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhongyouzk.top/gtquwilibn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtardpstpv.html

[D02] 追加元素到末尾
来源：http://hz.xuetiantiany.cn/gtffpndenr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.birdmap.top/gtjhpogkrg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guannengcc.top/gtmmjrqqhy.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtfippydfx.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtmslrnkec.html

Java: list.add(4);
来源：http://hz.ivvv.top/gtqczszcar.html

Go:   arr = append(arr, 4)
来源：http://hz.zdqjudy.top/gtakypbihi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.wangshuangyany.cn/gtbtmtiljj.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gtdhyxijqh.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtbxkxqhjy.html

Py:   arr.insert(0, 0)
来源：http://hz.ydzc1.top/gtzunooggf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtqgwjsiqo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258.top/gtmlvhdzcq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.dashuyun.cn/gtnndtsnxt.html

Java: list.add(0, 0);
来源：http://hz.havefunace.top/gtpiewcgyb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gtydbfejwq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtzelemaud.html

C#:   list.Insert(0, 0);
来源：http://hz.vqdsnc.cn/gtziibeziz.html

[D04] 删除元素
来源：http://hz.daxiang520.top/gtykwdodzb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhiwuduotai.top/gtzcyhltkm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xziqi.cn/gthdzjgnqu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gtalfrzcac.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtlkqkezgh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gtzdxcswra.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cashguo.top/gtqgeskmnx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.316326.xyz/gtyeojnxok.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtxwckiycf.html

[D05] 访问与修改元素
来源：http://hz.cashguo.top/gtwrnlsipb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtayhidivy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtjqkiojik.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cdnleiting.top/gtnfquanne.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigufen.top/gtpdnljlqh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258.top/gtpygafzwl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fzhhl.top/gtrwqiakdp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtqahxtneq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pycfn.com/gtkchlsydj.html

[D06] 数组长度
来源：http://hz.cheryme.top/gtwdnmsjkr.html

Py:   len(arr)
来源：http://hz.shuidangran.top/gttbeqaxvi.html

PHP:  count($arr);
来源：http://hz.gogol.net.cn/gtmxwjmbao.html

JS:   arr.length
来源：http://hz.hongshengwenyu.top/gtbqunnmza.html

TS:   arr.length
来源：http://hz.316326.xyz/gtsdiahxcl.html

Java: list.size();
来源：http://hz.jinqigfzy.top/gthfrreser.html

Go:   len(arr)
来源：http://hz.hnxiangtu.top/gttwuemtxp.html

Ruby: arr.length; arr.size
来源：http://hz.zycfv.cn/gtkspdobxm.html

C#:   list.Count;
来源：http://hz.redwolf501.top/gtaopgjqkr.html

[D07] 切片 / 取子数组
来源：http://hz.fengsongda.top/gtajsjkmgv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hywenlv.cn/gtzbghmrny.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnqzz.top/gtsbzrafix.html

JS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtcmeedfcd.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gteushyhrc.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtaunjbilz.html

Go:   arr[1:4]
来源：http://hz.hysaishi.cn/gtumgtcocf.html

Ruby: arr[1, 3]
来源：http://hz.yanxiufei.cn/gtmplerdbx.html

C#:   list.GetRange(1, 3);
来源：http://hz.gotoacloud.top/gtsnfqiage.html

[D08] 合并两个数组
来源：http://hz.jiagoushi.top/gtgnaxkfeb.html

Py:   a + b;  a.extend(b)
来源：http://hz.xylfe.cn/gttckflgus.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigufen.top/gtoidhqrlk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinyuanbaomall.cn/gtsijlzzmo.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtyflfpscg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gthhcaymos.html

Go:   append(a, b...)
来源：http://hz.havefunace.top/gtsjdtuqzo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.vqdsnc.cn/gtapnfuuyj.html

C#:   a.Concat(b).ToList()
来源：http://hz.sysykeji.top/gtcogcggnp.html

[D09] 排序（升序）
来源：http://hz.sweek.top/gtkvfuvyni.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gthkbvjhua.html

PHP:  sort($arr);
来源：http://hz.yangfankeji.com/gtndydotum.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhixingplan.top/gttkrbwakw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nanxinkj.top/gtecmyxqcf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtizgrquky.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gaohongyu789.top/gtjsnfegrq.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtsgihmznk.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gteccfxshl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xinyue.icu/gtwqnelwwz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cqqwz.cn/gtbeppjkwj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtixfthkoi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gturkgwmrh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtkeziytrk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cashguo.top/gtxrafdrel.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.haohaochexian.top/gtgjdbwuxu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtbvicaaqu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuanzhike.top/gtejhjbheo.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gttmavnqqa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtynfsduig.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtdeyptbpy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.316326.xyz/gtqmbwdpqi.html

TS:   [...arr].reverse();
来源：http://hz.zhiwuduotai.top/gttvrovvgq.html

Java: Collections.reverse(list);
来源：http://hz.wangdashe.top/gtarzugvge.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgufenzy.top/gtpksoukjt.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtmgrolrtu.html

C#:   list.Reverse();
来源：http://hz.daxiang520.top/gtiphbljpe.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtnbpntlal.html

Py:   arr.index(x);  x in arr
来源：http://hz.aibaodan.cn/gtwfynujph.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.0kj1m.cn/gtqnsxfnzs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtimxjrlrf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gteucqwgdd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gtkqkemwjl.html

Go:   slices.Index(arr, x)
来源：http://hz.vqdsnc.cn/gtclobxwmi.html

Ruby: arr.index(x)
来源：http://hz.9152youxi.cn/gtpgvwhola.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtspmfncsv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gtknxzsuar.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtzcymwyyp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gogol.net.cn/gtkmsskbda.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gthbkoovcn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtaofyalsx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.meibo888.top/gtgmxasxju.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnqzz.top/gttxjpqykk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtqwujgykn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nanxuanxn.top/gtpfqtorib.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtpdsmzacw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.iojbl.cn/gtxtnufjjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtrlslfnnl.html

JS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtnlldlqgi.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtubdjfpny.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hysaishi.cn/gtjzzdqkyo.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtmokjbwfd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.c1oappe.top/gtmgljlkbd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sweek.top/gthlpwphic.html

[D15] 去重
来源：http://hz.sysykeji.top/gtfsuxetjg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gthwrzwnpj.html

PHP:  array_unique($arr);
来源：http://hz.chenjidiqi.icu/gtbfkrcpxy.html

JS:   [...new Set(arr)]
来源：http://hz.cqqwz.cn/gtparyrtun.html

TS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtzkbnpwdf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.bjfxy.top/gtxukfhoja.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pycfn.com/gtejuvftss.html

Ruby: arr.uniq
来源：http://hz.pycfn.com/gtoxhusxbl.html

C#:   list.Distinct().ToList()
来源：http://hz.haohaochexian.top/gtxzrquifh.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gtjulotxwf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.kuanghao11.cn/gtnlqeybsi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtmhvbkbdp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtezuimmim.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtpyqtnrjg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.mhx1999.top/gttwgwnqqo.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtpgtufjxa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtkxicomjo.html

C#:   list.Sum();  list.Average()
来源：http://hz.sweek.top/gtxyvutpta.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gtxufdbler.html

Py:   max(arr);  min(arr)
来源：http://hz.zhixingplan.top/gtcbyyhdmv.html

PHP:  max($arr);  min($arr);
来源：http://hz.hnxiangtu.top/gtuhsakjit.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daria6918.cn/gtbkhfxvev.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtlctbeyox.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtkyawrfiw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhongyouzk.top/gtcjckpuje.html

Ruby: arr.max;  arr.min
来源：http://hz.ppjwa.cn/gtucnrzgml.html

C#:   list.Max();  list.Min()
来源：http://hz.bjfxy.top/gtsolputuc.html

[D18] 扁平化嵌套数组
来源：http://hz.zhengqikj.top/gtolseuyaf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydjk.org.cn/gtznouoont.html

PHP:  array_merge(...$nested);
来源：http://hz.yvedp.cn/gtpqobcohq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gtrmwwnmcj.html

TS:   nested.flat();
来源：http://hz.gogol.net.cn/gtqihfuxxy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fengsongda.top/gtiaaqfkwb.html

Go:   // 手写双层循环
来源：http://hz.ppjwa.cn/gtajwnzfrd.html

Ruby: nested.flatten
来源：http://hz.cucudq.cn/gtzqbydrkc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cdnleiting.top/gtmxauxchk.html

[D19] 按字段分组
来源：http://hz.zhixingplan.top/gtnnyqpmhz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtrznhrfqv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtxerxgkfi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxinkj.top/gteycgzvnr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtqanlkfuk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gtactaiian.html

Go:   // 手写 map[string][]T
来源：http://hz.sxryk.cn/gtpxjffwfh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtlivwjqao.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tianlin.xyz/gtfavifikn.html

[D20] 统计每个元素出现次数
来源：http://hz.mhx1999.top/gtjvdbefqk.html

Py:   Counter(arr)
来源：http://hz.hammf.cn/gtkzvkbmtd.html

PHP:  array_count_values($arr);
来源：http://hz.hysaishi.cn/gtadkgzubg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtzszlpihp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtcvanpqaf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtccltnsye.html

Go:   // 手写 map[T]int
来源：http://hz.xingfuxueyuan.xyz/gttjivoyyz.html

Ruby: arr.tally
来源：http://hz.shanyushiyangtech.top/gtqrljxdcu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtfzkpbzrn.html

[D21] 判断是否包含某元素
来源：http://hz.ydzc1.top/gtsvgddbgk.html

Py:   x in arr
来源：http://hz.cheryme.top/gtpxlvsbtw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxinkj.top/gtztcflbch.html

JS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtszoscdhb.html

TS:   arr.includes(x)
来源：http://hz.ivvv.top/gtiqcnadsu.html

Java: list.contains(x)
来源：http://hz.wangdashe.top/gtzhitgigt.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtzojrengu.html

Ruby: arr.include?(x)
来源：http://hz.ppjwa.cn/gtqsoauzeg.html

C#:   list.Contains(x)
来源：http://hz.hnxiangtu.top/gtocvwvfcz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258.top/gtfxsnuchw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangkeji.top/gtheytxpqh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gtaxznzkud.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangshuangyany.cn/gtoiwfnlum.html

TS:   [...arr];
来源：http://hz.gzhubu.top/gtuzzmilkc.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258.top/gtghgafyjb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258888.top/gtczwuazvo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sxryk.cn/gtmhkhmmfm.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangkeji.top/gtvsfwsvpo.html

[D23] reduce 累积计算
来源：http://hz.nanxuanxn.top/gtqifoyqua.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gaohongyu789.top/gtocjvcwnz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtjcmjvlwo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtukkgyisi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtkknmdpfr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.smart0.xyz/gthbdaacih.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtcnqnfmyk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gtjkizprxd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gttvldgoqy.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhijiandao.cn/gtfclifwqu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj202588.top/gticxpokkp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtodvzkwif.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shzxlz.cn/gtvmikmwra.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtgxxydnmc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ppjwa.cn/gttgmsznav.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydzc1.top/gtkqbtwhfw.html


<!-- 参考信息 -->